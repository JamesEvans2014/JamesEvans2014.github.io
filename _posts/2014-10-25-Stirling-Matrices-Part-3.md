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
where \\(s(i,j)\\) is a \\(\textbf {Stirling number of the first kind}\\) (see below).
Moreover, the following formulae hold true also:
\\[
\begin {aligned}
T\_3(n,m) & =\Big [s(n,n-2)+(n-m)\Big ( s(n,n-1)-m\Big )\Big ]\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix},\\\
T\_4(n,m) & =\Big [s(n,n-3)+(n-m)\Big (s(n,n-2) -s(n,n-1)m+m^2\Big )\Big ]\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix}.
\end {aligned}
\\]

Hence the following theorem is conjectured:

\\( \textbf {Theorem}\\)

\\[
T\_k(n,m)=\Big [s(n,n-k+1)+(n-m)\sum\_{l=0}^{k-2}(-1)^ls(n,n-k+l+2)m^l\Big ]\begin {pmatrix} n-1 \\\ m-1 \end {pmatrix}.
\\]
When \\(k=1\\) in the above formula, the sum on the right is zero.

\\(\textbf {Corollary}\\)

Let \\(\tilde {a}^n\_{km}\\) denote the entries of the Stirling matrix \\(\tilde {A}\_n\\). Then
\\[
\begin {equation}
\tilde {a}^n\_{km}=\frac {(-1)^{n+k+m-1}}{(n-1)!}T\_k(n,m),\ \ \ 1\leq k,m\leq n.
\end {equation}
\\]

The pressing question of course is what is the goal of this work? 
The hope would be that since the Stirling matrix is the inverse of a matrix with known structure that it 
may be possible to derive an expressions or recurrence relations for a certain subclass of the 
Stirling numbers of the first kind given the formula above.
The reason for placing this work on this blog is simple, it is all conjecture. I have no proofs for any of the statements above and any insight into this would be greatly appreciated.

#Appendix: Stirling Numbers of the First Kind

The Stirling Numbers, named after James Stirling (1692-1770) come in two varieties traditionally called the Stirling numbers of the first kind and the Stirling numbers of the second kind. This appendix will be devoted to a discussion on the Stirling numbers of the first kind which will be denoted \\(s(n,k)\\). Stirling numbers, like binomial coefficients can be constructed into triangular arrays. The array for \\(s(n,k)\\) is given for reference:
\\[1\\]\\[0\ \ \ 1\\]\\[0\ \ \ 1\ \ \ \ 1\\]\\[0\ \ \ 2\ \ \ 3\ \ \ 1\\]\\[0\ \ \ 6\ \ \ 11\ \ \ 6\ \ \ 1\\]\\[0\ \ \ 24\ \ \ 50\ \ \ 35\ \ \ 10\ \ \ 1\\]\\[0\ \ \ 120\ \ \ 274\ \ \ 225\ \ \ 85\ \ \ 15\ \ \ 1\\]
The Sterling numbers of the first kind show up in many different places. It is of note that \\(s(n,k)\\) is the number of ways to arrange \\(n\\) objects into \\(k\\) cycles. A cycle is a cyclic arrangement linked in a necklace fashion. For example, if \\([A,B,C,D]\\) is a cycle, it is understood that
\\[[A,B,C,D]=[B,C,D,A]=[C,D,A,B]=[D,A,B,C].\\]
Stirling numbers \\(s(n,k)\\) also show up in the consideration of the rising factorial defined as 
\\[x^{\overline {m}}=x(x+1)\dots(x+m-1),\ \ \ m\geq 0.\\]
Indeed, it can be shown that
\\[x^{\overline {m}}=\sum\_{k=0}^ms(n,k)x^k.\\]
For convenience, some of the properties relating to Stirling numbers of the first kind are listed below:
\\[s(n+1,k)=ns(n,k)+s(n,k-1)\\]
\\[s(n,0)=0,\ \ \ s(n,1)=(n-1)!\ \ \ s(n,n)=1,\ \ \ s(n,k)=0\ \ \ \forall n >0, k>n.\\]
\\[s(n,n-1)= \begin {pmatrix} n \\\ 2 \end {pmatrix}\\]
\\[s(n+1,m+1)=\sum_{k=0}^ns(n,k)\begin {pmatrix} k \\\ m \end {pmatrix},\ \ \ \forall m,n \geq 0.\\]
Interestingly, there is no explicit formula for the Stirling numbers.
