---
layout    : post
title     :  "Stirling Matrices Part 2"
date      :   2014-10-25 15:47:43
categories: Stirling Numbers Matrices
---

This is a continuation of the discussion in the previous post found here: [Stirling Matrices Part 1](http://jamesevans2014.github.io/stirling/numbers/matrices/2014/10/25/Stirling-Matrices.html)

The inverse of the matrix \\(A\_n\\) defined in the previous post will be called the Stirling matrix of order \\(n\\). 
It will be denoted \\(\tilde {A}\_n\\) and its \\((i-j)\\)th entry \\(\tilde {a}\_{ij}^n\\).

Although time consuming and costly, inverting the matrix \\(A_n\\) unveils some interesting number patterns. The first few Stirling matrices are given for reference:
\\[
\tilde {A}\_1=1,\ \ \ \tilde {A}\_2=\begin {pmatrix} -1 & 1\\\ 2 & -1 \end {pmatrix},\ \ \ \tilde {A}\_3=\frac {1}{2}\begin {pmatrix} 1 & -2 & 1 \\\ -5 & 8 & -3 \\\ 6 & -6 & 2 \end {pmatrix},
\\]
\\[
\tilde {A}\_4=\frac {1}{6}\begin {pmatrix} -1 & 3 & -3 & 1 \\\ 9 & -24 & 21 & -6 \\\ -26 & 57 & -42 & 11 \\\ 24 & -36 & 24 & -6 \end {pmatrix},\ \ \ 
\tilde {A}\_5=\frac {1}{24}\begin {pmatrix} 1 & -4 & 6 & -4 & 1 \\\ -14 & 52 & -72 & 44 & -10 \\\ 71 & -236 & 294 & -164 & 35 \\\ -154 & 428 & -468 & 244 & -50 \\\ 120 & -240 & 240 & -120 & 24 \end {pmatrix},
\\]
\\[
\tilde {A}_6=\frac {1}{120}\begin {pmatrix} -1 & 5 & -10 & 10  & -5 & 1 \\\ 20 & -95 & 180 & -170 & 80 & -15 \\\ -155 & 685 & -1210 & 1070 & -475 & 85 \\\ 580 & -2305 & 3720 & -3070 & 1300 & -225 \\\ -1044 & 3510 & -5080 & 3960 & -1620 & 274 \\\ 720 & -1800 & 2400 & -1800 & 720 & -120 \end {pmatrix},
\\]
\\[
\tilde {A}_7=\frac {1}{720}\begin {pmatrix} 1 & -6 & 15 & -20 & 15 & -6 & 1 \\\ -18 & 156 & -375 & 480  & -345 & 132 & -21\\\ 295 & -1620 & 3705 & -4520 & 3105 & -1140 & 175 \\\ -1665 & 8520 & -18285 & 21120 & -13875 & 4920 & -735 \\\ 5104 & -23574 & 46680 & -50900 & 32160 & -11064 & 1624 \\\ -8028 & 31644 & -56940 & 59040 & -36180 & 12228 & -1764 \\\ 5040 & -15120 & 25200 & -25200 & 15120 & -5040 & 720 \end {pmatrix}.
\\]

In view of the first few Stirling matrices, the following are proposed:

Let \\(\tilde {A}_n\\) be an Stirling matrix of order \\(n\\). Then
\\[
\det (\tilde {A}\_n)=(-1)^{\frac {n(n-1)}{2}}\Big ( \prod\_{r=1}^n(r-1)!\Big )^{-1}.
\\]
The product is known as the superfactorial.

Let \\(\tilde {a}^n\_{ij}\\) denote the entries of the Stirling matrix \\(\tilde {A}_n\\). Then
\\[
\begin {equation}
\sum\_{j=1}^n\tilde {a}\_{ij}= \begin {cases} 0,\ \ \ 1\leq i\leq n-1,\\\ 1,\ \ \ i=n.\end {cases},\ \ \ 
\sum\_{i=1}^n\tilde {a}\_{ij}= \begin {cases} 0,\ \ \ 2\leq j\leq n,\\\ 1,\ \ \ j=1.\end {cases}.
\end {equation}
\\]

Considering the rows (or columns) of the Stirling matrices formed into triangular arrays leads to some interesting number patterns emerging. 

A positive Stirling matrix will be denoted \\(\tilde {A}^+\_n\\) and its entries are defined by the relation
\\[
(\tilde {A}^+\_n)\_{ij}=(n-1)!|\tilde {a}\_{ij}|.
\\]

Let \\(T\_k(n,m)\\) denote the triangular array constructed by fixing \\(k\\) and placing the \\(k\\)th row of each positive Stirling matrix in descending order with \\(n\\) corresponding to the order of the positive Stirling matrix \\(\tilde {A}^+\_n\\) and \\(j\\) to the column number. Since for \\(n<k\\) the Stirling matrix has no row, zeros will be placed in their stead.

The first few triangles are provided for reference:

\\(k=1\\)
\\[1\\]\\[1\ \ \ 1\\]\\[1\ \ \ 2\ \ \ 1\\]\\[1 \ \ \ 3\ \ \ 3\ \ \ 1\\]\\[1\ \ \ 4\ \ \ 6\ \ \ 4\ \ \ 1\\]
\\(k=2\\)
\\[0\\]\\[2\ \ \ 1\\]\\[5\ \ \ 8\ \ \ 3\\]\\[9 \ \ \ 24\ \ \ 21\ \ \ 6\\]\\[14\ \ \ 52\ \ \ 72\ \ \ 44\ \ \ 10\\]\\[20\ \ \ 95\ \ \ 180\ \ \ 170\ \ \ 80\ \ \ 15\\]
\\(k=3\\)
\\[0\\]\\[0\ \ \ 0\\]\\[6\ \ \ 6\ \ \ 2\\]\\[26 \ \ \ 57\ \ \ 42\ \ \ 11\\]\\[71\ \ \ 236\ \ \ 294\ \ \ 164\ \ \ 35\\]\\[155\ \ \ 685\ \ \ 1210\ \ \ 1070\ \ \ 475\ \ \ 85\\]\\[295\ \ \ 1620\ \ \ 3705\ \ \ 4520\ \ \ 3105\ \ \ 1140\ \ \ 175\\]
\\(k=4\\)
\\[0\\]\\[0\ \ \ 0\\]\\[0\ \ \ 0\ \ \ 0\\]\\[24\ \ \ 36\ \ \ 24\ \ \ 6\\]\\[154\ \ \ 428\ \ \ 468\ \ \ 244\ \ \ 50\\]\\[580\ \ \ 2305\ \ \ 3720\ \ \ 3070\ \ \ 1300\ \ \ 225\\]\\[1665\ \ \ 8520\ \ \ 18285\ \ \ 21120\ \ \ 13875\ \ \ 4920\ \ \ 735\\]

Clearly the first triangular array \\(T\_1(n,m)\\) is simply Pascal\'s triangle but what of the other arrays? Down the right-hand side of \\(T\_2(n,m)\\), it is observed that the triangle numbers progress and moreover, it can be seen that a particular set of the Stirling numbers of the first kind are progressing down the right-hand side of the triangular array \\(T\_3(n,m)\\) and indeed for the triangle \\(T\_4(n,m)\\) Stirling numbers of the first kind appear down the right-hand side also.

In the next post, the patterns seen in the above triangles will be explored.
