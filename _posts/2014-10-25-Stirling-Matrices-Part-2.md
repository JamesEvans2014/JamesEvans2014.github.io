---
layout    : post
title     :  "Stirling Matrices Part 2"
date      :   2014-10-25 15:47:43
categories: Stirling Numbers Matrices
---

This is a continuation of the discussion in the previous post found here: [Sterling Matrices Part 1](http://jamesevans2014.github.io/stirling/numbers/matrices/2014/10/25/Stirling-Matrices.html)

The inverse of the matrix \\(A\_n\\) defined in the previous post will be called the Sterling matrix of order \\(n\\). 
It will be denoted \\(\tilde {A}\_n\\) and its \\((i-j)\\)th entry \\(\tilde {a}\_{ij}^n\\).

Although time consuming and costly, inverting the matrix \\(A_n\\) unveils some interesting number patterns. The first few Sterling matrices are given for reference:
\\[
\tilde {A}\_1=1,\ \ \ \tilde {A}\_2=\begin {pmatrix} -1 & 1\\ 2 & -1 \end {pmatrix},\ \ \ \tilde {A}\_3=\frac {1}{2}\begin {pmatrix} 1 & -2 & 1 \\ -5 & 8 & -3 \\ 6 & -6 & 2 \end {pmatrix},
\\]
\\[
\tilde {A}\_4=\frac {1}{6}\begin {pmatrix} -1 & 3 & -3 & 1 \\ 9 & -24 & 21 & -6 \\ -26 & 57 & -42 & 11 \\ 24 & -36 & 24 & -6 \end {pmatrix},\ \ \ 
\tilde {A}\_5=\frac {1}{24}\begin {pmatrix} 1 & -4 & 6 & -4 & 1 \\ -14 & 52 & -72 & 44 & -10 \\ 71 & -236 & 294 & -164 & 35 \\ -154 & 428 & -468 & 244 & -50 \\ 120 & -240 & 240 & -120 & 24 \end {pmatrix},
\\]
\\[
\tilde {A}_6=\frac {1}{120}\begin {pmatrix} -1 & 5 & -10 & 10  & -5 & 1 \\ 20 & -95 & 180 & -170 & 80 & -15 \\ -155 & 685 & -1210 & 1070 & -475 & 85 \\ 580 & -2305 & 3720 & -3070 & 1300 & -225 \\ -1044 & 3510 & -5080 & 3960 & -1620 & 274 \\ 720 & -1800 & 2400 & -1800 & 720 & -120 \end {pmatrix},
\\]
\\[
\tilde {A}_7=\frac {1}{720}\begin {pmatrix} 1 & -6 & 15 & -20 & 15 & -6 & 1 \\ -18 & 156 & -375 & 480  & -345 & 132 & -21\\ 295 & -1620 & 3705 & -4520 & 3105 & -1140 & 175 \\ -1665 & 8520 & -18285 & 21120 & -13875 & 4920 & -735 \\ 5104 & -23574 & 46680 & -50900 & 32160 & -11064 & 1624 \\ -8028 & 31644 & -56940 & 59040 & -36180 & 12228 & -1764 \\ 5040 & -15120 & 25200 & -25200 & 15120 & -5040 & 720 \end {pmatrix}.
\\]




