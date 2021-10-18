---
title: Matrizes em escada, sistemas de equações lineares, método de gauss
header-includes:
  - \usepackage{asmath}
  - \usepackage{xcolor}
---


1. [Operações elementares](#operações-elementares)
2. [Caraterística](#caraterística)
3. [Matriz ampliada](#matriz-ampliada)
   * [Teoremas](#teoremas)
   * [Grau de indeterminanção](#grau-de-indeterminanção)
4. [Método de eliminação de Gauss](#método-de-eliminação-de-gauss)

# Matrizes em escada 

Diz-se que uma matriz $$A_{m\times n}$$, é uma matrize em escada se:
- Por baixo do primeiro elemento de não nulo de coada linha da matriz e por
baixo dos elementos anteriores da mesma linha, todas as entradas são 
iguais a zero.
- Não existem linhas totalmente nulas seguidas de linhas nulas.

$$
A = \begin{bmatrix}
1 & 2 & 3 & 0 \\
0 & 0 & 4 & 5 \\
0 & 0 & 0 & 4 \\
0 & 0 & 0 & 0 \\
\end{bmatrix}
$$

A é uma matriz em escada.

## Operações elementares

Seja $$A$$ uma matriz.Chamamos __operações elementares__ sobre $$A$$ a uma 
operação dos seguintes tipos:
- Troca entre si de duas linhas ou colunas, $$L_{j} <-> L_{i},C_{j} <-> C_{i}$$.
- Multiplicar uma linha ou coluna por um __escalar__, $$\alpha L_{i},
\alpha C_{i}$$.
- __Adicionar__ a uma linha ou coluna, entrada a entrada, uma outra linha ou coluna
__multiplicada por um escalar não nulo__, $$\alpha L_{i} + L_{j}$$ a nova linha
será $$j$$.

## Caraterística 

Seja $$A$$ uma matriz e $$B$$ uma matriz em escada de linhas obtida de $$A$$ 
através de operações elementares sobre $$A$$.
A __caraterística__ de $$A$$ é o número de linhas não nulas da matriz $$B$$. A 
caraterística de A denota-se $$r(A) $$ ou $$ r_{A}$$.

$$
A = \begin{bmatrix}
1 & 2 & 3 & 0 \\
0 & 0 & 4 & 5 \\
0 & 0 & 0 & 4 \\
0 & 0 & 0 & 0 \\
\end{bmatrix}
$$ 

$$
r(A) = 3
$$

# Sistemas de equações lineares, Resolução usando o método de Gauss.

Um sistema de equações lineares (todas as equações são de primeiro grau) é:
- __Impossível__ se não tem solução;
- __Possível determinado__ se tem uma única solução;
- __Possível indeterminado__ se tem mais do que uma solução;

Exemplos de sistema de equações lineares:

Impossível:
$$
\begin{equation}
    \begin{cases}
        x + y = 1\\
        x + y = 2\\
    \end{cases}
\end{equation}
$$

Possível determinado:
$$
\begin{equation}
    \begin{cases}
        x + y = 2\\
        x - y = 0
    \end{cases}
\end{equation}
$$

Possível indeterminado:
$$
\begin{equation}
    \begin{cases}
        x+y=1\\
        2x+2y=2
    \end{cases}
\end{equation}
$$

Dado o __sistema__ $$m$$:

$$
\begin{equation}
    \begin{cases}
        a_{11}x_{1} = b_{1}\\
        a_{m\times n}x_{n} = b_{m}
    \end{cases}
\end{equation}
$$

Chamamos __forma matricial__ do sistema à igualdade de matrizes:

$$ AX = B $$

$$ 
A = \begin{bmatrix}
a_{11} & ... & a_{1n} \\
a_{21} & ... & a_{2n} \\
a_{n1} & ... & a_{mn}
\end{bmatrix}
$$

$$
X = \begin{bmatrix}
x_{1}\\
x_{2}\\
x_{n}
\end{bmatrix}
$$

$$
B=\begin{bmatrix}
b_{1}\\
b_{2}\\
b_{n}
\end{bmatrix}
B=\begin{bmatrix}
b_{1}\\
b_{2}\\
b_{n}
\end{bmatrix}
$$

Dizemos que $$A$$ é a __matriz dos coeficientes__, $$X$$ é a matriz das 
incógnitas, e $$B$$ é a __matriz dos termos independentes__.

$$
\begin{equation}
\color{red}{2}\color{green}x + \color{green}y = \color{blue}1
\end{equation}
\\
\color{red}{\text{Coeficiente}} \\ 
\color{green}{\text{incógnita}} \\ 
\color{blue}{\text{termo independente}} \\
$$

## Matriz ampliada 

Chamamos à matriz 

$$
[A|B] = \left[ 
\begin{array}{cccc|c}
a_{11} & a_{12} & ... & a_{1n} & b_1 \\
... & ... & ... & \vdots & b_{2} \\
a_{n1} & a_{n1} & ... & a_{mn} & b_n
\end{array} 
\right]
$$

A __matriz ampliada do sistema__.

### Teoremas

Seja $$A$$ uma matriz de ordem $$k\times n$$. Considere um sistema $$AX=B$$.  
Seja $$m=r([A|B])$$ o sistema considerado é:
- Impossível se $$r(A)=m$$;
- Possível determinado se $$r(A)=m=n$$;
- Possível indeterminado se $$r(A)=m<n$$;

$$ n = \text{Número de incógnitas}$$

__Impossível__: 

$$
\left[
\begin{array}{cc|c}
1 & 1 & 1 \\
1 & 1 & 2
\end{array} 
\right]
\xrightarrow{-L_1+L_2}
\left[
\begin{array}{cc|c}
1 & 1 & 1 \\
0 & 0 & 1
\end{array} 
\right]
\\
r(A) < r([A|B])
$$

__Possível determinado__: 

$$
\left[
\begin{array}{cc|c}
1 & 1 & 1 \\
1 & -1 & 0
\end{array} 
\right]
\xrightarrow{-L_1+L_2}
\left[
\begin{array}{cc|c}
1 & 1 & 2 \\
0 & -2 & -2
\end{array} 
\right]
\\
r(A) = r([A|B])
$$

__Possível indeterminado__: 

$$
\left[
\begin{array}{cc|c}
1 & 1 & 1 \\
2 & 2 & 2
\end{array} 
\right]
\xrightarrow{-L_1+L_2}
\left[
\begin{array}{cc|c}
1 & 1 & 1 \\
0 & 0 & 0
\end{array} 
\right]
\\
r(A) < r([A|B])
$$

### Grau de indeterminanção

O grau de indeterminação de um sistema é dado por: $$n-r(A)$$

## Método de eliminação de Gauss

É um processo de resolução de equações lineares $$AX=B$$ que começa pela 
__transformação da matriz ampliada do sistema__ $$[A|B]$$ numa matriz $$[A'|B]$$ 
__em escada de linhas__, através das operações elementares.  
Depois tentamos __transformar numa matriz diagonal__ para conseguir 
as variáveis.  
O professor recomenda __usar só transformações de linhas e não colunas__.
