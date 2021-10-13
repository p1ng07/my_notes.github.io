---
title: Aula 1 de calculo 1
header-includes:
  - \usepackage{xcolor}
---
# Multiplicação

$$ A . B $$ só é possível quando $$ An = Bm $$. \\
O processo é multiplicar todas as linhas de $$A$$ pelas colunas de $$B$$.

$$
\begin{bmatrix}
\color{red}1 & \color{red}2 & \color{red}3 \\
\color{green}{-1} & \color{green}{0} & \color{green}{1} \\
1 & 2 & -1 \\
\end{bmatrix}
\times
\begin{bmatrix}
\color{red}5 & \color{green}{-1}  \\
0 & 2\\
1 & 3\\
\end{bmatrix}
=
\begin{bmatrix}
\color{red}8 & \color{green}{12}  \\
-4 & 4 \\
4 & 0 \\
\end{bmatrix}
\\
\begin{pmatrix}
\color{red}{1\times5+2\times0+3\times1} & \color{green}{-1+2\times2+3\times3}\\
-5+0\times5+1 & 1+0+3 \\
1\times5+2\times0+1\times1 & -1+4-3 \\
\end{pmatrix}
$$

## Pontência de uma matriz

A exponênciação de uma matriz é apenas a multiplicação da matriz por si mesma.  

$$
A = \begin{bmatrix}
1 & 2 \\
2 & 3 \\
\end{bmatrix}

A^2 = \begin{bmatrix}
1 & 2 \\
2 & 3 \\
\end{bmatrix}
\times
\begin{bmatrix}
1 & 2 \\
2 & 3 \\
\end{bmatrix}
=
\begin{bmatrix}
 5 & 8 \\
 8 & 13 \\
\end{bmatrix}
$$

# Comutáveis

Duas matrizes dizem-se comutáveis se $$ AB = BA$$.
