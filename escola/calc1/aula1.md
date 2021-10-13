---
title: Aula 1 de calculo 1
header-includes:
  - \usepackage{xcolor}
---

# Matriz


1. [Noção de matriz](#noção-de-matriz)
   * [Representação de uma matriz](#representação-de-uma-matriz)
   * [Diagonais de uma matriz](#diagonais-de-uma-matriz)
2. [Tipos de matrizes](#tipos-de-matrizes)
   * [Triangular superior](#triangular-superior)
   * [Triangular inferior](#triangular-inferior)
   * [Diagonal](#diagonal)
   * [Identidade](#identidade)
3. [Operações com matrizes](#operações-com-matrizes)
   * [Transposição](#transposição)
   * [Adição e multiplicação por escalar](#adição-e-multiplicação-por-escalar)
   * [Traço](#traço)
   * [Multiplicação](#multiplicação)
4. [Teoremas](#teoremas)

## Noção de matriz

Uma matriz é qualquer tabela com __$$ mxn $$ elementos__, $$ m $$  sendo linhas
, e $$ n $$ sendo colunas.

Exemplo de __matriz__:

$$
A = \begin{bmatrix}
1 & 3 & 5 \\
2 & 7 & 6 \\
4 & 0 & 8 \\
\end{bmatrix}
$$

### Representação de uma matriz

Uma matriz é representada por $$ A = [aij]mxn $$ ou $$ A = (aij)mxn $$.  
Em caso de dimensão subentendida: $$ A = [aij] $$ 

Duas matrizes dizem-se iguais quandos têm as mesmas entradas nas mesmas posições.

### Diagonais de uma matriz

$$
A = \begin{bmatrix}
\color{green}{1} & 3 & \color{red}{5} \\
2 & \color{yellow}{7} & 6 \\
\color{red}{4} & 0 & \color{green}{8} \\
\end{bmatrix}
\\
\color{green}{Diagonal Principal} \\ 
\color{Red}{Diagonal Secundária} \\ 
$$

## Tipos de matrizes

Dada matriz $$ A = [aij]mxn $$:

- A é linha se $$ m = 1 $$;
- A é coluno se $$ n = 1 $$;
- A é quadrada se $$ m = n $$, dizemos que é matriz de ordem $$ n $$;
- A é retangular se $$ m \neq n $$;

### Triangular superior

Dizemos que A é __triangular superior__ se, $$ aij = 0, i > j $$.

$$
A = \begin{bmatrix}
1 & 3 & 5 \\
\color{red}{0} & 7 & 6 \\
\color{red}{0} & \color{red}{0} & 8 \\
\end{bmatrix}
$$

### Triangular inferior

Dizemos que A é __triangular inferior__ se, $$ aij = 0, i < j $$.

$$
A = \begin{bmatrix}
1 & \color{red}{0} & \color{red}{0} \\
2 & 7 & \color{red}{0} \\
4 & 0 & 8 \\
\end{bmatrix}
$$

### Diagonal

Dizemos que A é __diagonal__ se $$a[ij] = 0, i \neq j$$.

$$
A = \begin{bmatrix}
1 & \color{red}{0} & \color{red}{0} \\
\color{red}{0} & 7 & \color{red}{0} \\
\color{red}{0} & \color{red}{0} & 8 \\
\end{bmatrix}
$$

### Identidade

Dizemos que A é __identidade__ se $$aij=1, i=j$$.

$$
A = \begin{bmatrix}
\color{green}{1} & 4 & 5 \\
5 & \color{green}{1} & 6 \\
7 & 9 & \color{green}{1} \\ 
\end{bmatrix}
$$

## Operações com matrizes

### Transposição
Chama-se __transposta__ A à matriz que se obtém de A __trocando as linhas pelas
colunas, $$A^T$$.__

Exemplos:

$$
B = \begin{bmatrix}
2 & 1 & 5 \\
1 & 0 & 4 \\
5 & 4 & 6 \\
\end{bmatrix}

B^T = \begin{bmatrix}
2 & 1 & 5 \\
1 & 0 & 4 \\
5 & 4 & 6 \\
\end{bmatrix}
$$

$$
C = \begin{bmatrix}
0 & 3 & -5 \\
-3 & 0 & 4 \\
5 & 4 & 6 \\
\end{bmatrix}

C^T = \begin{bmatrix}
0 & -3 & 5 \\
3 & 0 & -4 \\
-5 & -4 & 0 \\
\end{bmatrix}
$$

Diz-se que $$ B $$ é __simétrico__ pois $$ B=B^T $$. \\
Diz-se que $$ C $$ é __antisimétrico__ pois $$ C=-C^T $$. \\

### Adição e multiplicação por escalar

$$ A + B = [aij + bij] $$

$$ \alpha A = [\alpha . aji]mxn $$ 

### Traço 

Chama-se __traço__ à soma de entradas da diagonal principal, $$ tr(A) $$.

$$
A = \begin{bmatrix}
\color{green}{1} & 3 & -5 \\
-3 & \color{green}{2} & 4 \\
5 & -4 & \color{green}{3} \\
\end{bmatrix} 
\\
\color{green}{tr(A)} = 1+2+3 = 6\\
$$

## Teoremas 

- __Comutatividade de adição__, $$A+B=B+A$$  
- __Associatividade da adição__, $$A+(B+C) + (A+B)+C$$  
- __Matriz nula__, $$ A+0 = 0+A = A$$
- __Existência de simétricos__, simétrica de $$ A + (-A) = 0 $$


Sejam $$ \alpha $$ e $$ \beta $$ escalares:
- $$ \alpha (A+B) = \alpha A+\alpha B$$ e $$ (\alpha + \beta)A = \alpha A + \beta A $$
- $$ \alpha (\beta A) = (\alpha \beta) A $$
- $$ A = A \alpha $$ 

Desde que as operações sejam possíveis:
- $$ (A+B)^T = A^T + B^T $$
- $$ (\alpha A)^T = \alpha (A^T) $$
- $$ (A^T)^T = A $$

Sejam $$ A $$ e $$ B $$ quadradas de ordem n e K então:
- $$ tr(A+B) = tr(A)+tr(B) $$ 
- $$ tr(kA)=ktr(A) $$ 
- $$ tr(A^T) = tr(A) $$
 
