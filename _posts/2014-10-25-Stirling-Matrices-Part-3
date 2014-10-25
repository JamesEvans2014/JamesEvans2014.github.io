---
layout    : post
title     :  "Stirling Matrices Part 3"
date      :   2014-10-25 15:47:43
categories: Stirling Numbers Matrices
---

This is a continuation of the previous post. See the following link: [Sterling Matrices Part 2](http://jamesevans2014.github.io/stirling/numbers/matrices/2014/10/25/Stirling-Matrices-Part-2.html)

In this post, several propositions are formulated with regard to the triangular arrays established in the previous post.

\\[
T\_1(n,m)=\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix}.
\\]

\\[
T\_2(n,m)=\Big [ s(n,n-1)+(n-m)\Big ]\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix},
\\]
where \\(s(i,j)\\) is a Stirling number of the first kind (see below).
Moreover, the following formulae hold true also:
\\[
\begin {aligned}
T\_3(n,m) & =\Big [s(n,n-2)+(n-m)\Big ( s(n,n-1)-m\Big )\Big ]\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix},\\\
T\_4(n,m) & =\Big [s(n,n-3)+(n-m)\Big (s(n,n-2) -s(n,n-1)m+m^2\Big )\Big ]\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix}.
\end {aligned}
\\]

Hence the following theorem is conjectured:

\\[
T\_k(n,m)=\Big [s(n,n-k+1)+(n-m)\sum\_{l=0}^{k-2}(-1)^ls(n,n-k+l+2)m^l\Big ]\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix}.
\\]
When \\(k=1\\) in the above formula, the sum on the right is zero.

Let \\(\tilde {a}^n\_{km}\\) denote the entries of the associated matrix \\(\tilde {A}\_n\\). Then
\\[
\begin {equation}
\tilde {a}^n\_{km}=\frac {(-1)^{n+k+m-1}}{(n-1)!}T\_k(n,m),\ \ \ 1\leq k,m\leq n.
\end {equation}
\\]

The pressing question of course is what is the goal of this work? 
The hope would be that since the Stirling matrix is the inverse of a matrix with known structure that it 
may be possible to derive an expressions or recurrence relations for a certain subclass of the 
Stirling numbers of the first kind given the formula above.
