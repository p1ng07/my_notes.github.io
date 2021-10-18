---
title: Matriz inversa, método Gauss-Jordan
header-includes:
  - \usepackage{asmath}
  - \usepackage{xcolor}
---

# Matriz inversa

Seja $$A$$ uma matriz de ordem $$n$$. A __inversa de $$A$$__ (quando existe) é
representada por $$A^{-1}$$ e é uma matriz de ordem $$n$$ tal que $$AA^{-1}
=A^{-1}A=I_n$$, onde $$I_n$$ é a matriz __identidade__.

Exemplo:

$$
B = \begin{bmatrix}
1 & 3 \\
2 & 7 
\end{bmatrix}

C = \begin{bmatrix}
7 & -3 \\
-2 & 1 
\end{bmatrix}
$$

B é a inversa de C, pois

$$
BC = \begin{bmatrix}
1 & 0 \\ 
0 & 1 \\ 
\end{bmatrix}
= I^2
\\
CB = \begin{bmatrix}
1 & 0 \\ 
0 & 1 \\ 
\end{bmatrix}
= I^2
$$

Quando uma matriz $$A$$:
- __tem inversa__, $$A$$ diz-se __inversível__ e __não singular__;
- __não tem inversa__, diz-se __não inversível__ e __singular__;

## Método de Gauss-Jordan

Um dos métodos possíveis para __descobrir a matriz inversa__ de dada matriz.  

Definição:  

Seja $$A$$ uma matriz inversível($$r(A)=n$$). Aplicamos operações elementares
sobre as __linhas,as colunas não podem ser afetadas,__ da matriz $$[A|I_n]$$,
até $$A=I_n$$. A matriz que se obtém à direita é a __matriz inversa__.

Esquematicamente:

$$ [A|I] -> ... -> [I|A^{-1}] $$

## Teoremas

- Seja $$A$$ uma matriz quadrada de ordem $$n$$, $$A$$ é __inversível quando
e só quando__ $$r(A)=n$$;
- Seja $$A$$ uma matriz $$mn$$. Então $$I_mA=A \text{e} AI_n=A$$. Em particular,
sendo B uma matriz de ordem $$n$$ tem-se que $$BI_n=I_nB=B$$.

