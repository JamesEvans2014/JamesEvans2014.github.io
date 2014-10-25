---
layout    : post
title     :  "Stirling Matrices"
date      :   2014-10-25 15:47:43
categories: Stirling Numbers Matrices
---
This is an idea that I've had floating around for a while now. The idea came about during a conference held at Cardiff University
not so long ago. The idea is simple; what are the coefficients of a polynomial of degree \\(n\\) which go through the first \\(n+1\\) prime numbers? 

Prime polynomials may have a different definition, but for the purposes of the following discussion, the definition below is what is understood.

A prime polynomial \\(p\_n(x)\\) is a polynomial of \\((n-1)\\)th order satisfying \\(p\_n(i)=p\_i\\) where \\(p\_i\\) is the \\(i\\)th prime number, \\(i=1,2,\dots , n\\).

The first few polynomials are given for reference:
\\[ 
\begin {aligned}
p\_1(x) & = 2,\\\
p\_2(x) & = 1+x,\\\
p\_3(x) & = \frac {1}{2}(4-x+x^2),\\\
p\_4(x) & = \frac {1}{6}(18-14x+9x^2-x^3),\\\
p\_5(x) & = \frac {1}{24}(144-206x+141x^2-34x^3+3x^4),\\\
p\_6(x) & = \frac {1}{120}(1800-3496x+2730x^2-987x^3+150x^4-9x^5),\\\
p\_7(x) & = \frac {1}{720}(27360-61548x+53732x^2-22515x^3+4925x^4-537x^5+23x^6).
\end {aligned}
\\]

Initially,the interest was in being able to determine the coefficients of such polynomials for the finite \\(k\\)th order prime polynomials. The following construction would be one possible way of achieving such coefficients. 

Let \\(p\_n(x)\\) be the \\((n-1)\\)th order polynomial passing through the first \\(n\\) primes with the coeffcient of \\(x^m\\) being \\(c\_m\\), \\(m=0,1,\dots n-1\\), i.e.,
\\[
\begin {equation}
\begin {cases}
p\_n(x) & =c\_{n-1}x^{n-1}+c\_{n-2}x^{n-2}+\dots +c\_1x+c_0,\\\
p\_n(i) & =p\_i,\ \ \ 1\leq i\leq n.
\end {cases}
\end {equation}
\\]

Then by simply plugging in the relevant values into the polynomial, the following system holds:
\\[
\begin {equation}
\begin {cases}
c\_{n-1}+c\_{n-2}+\dots +c\_1+c\_0=2,\\\
2^{n-1}c\_{n-1}+2^{n-2}c\_{n-2}+\dots +2c\_1+c\_0=3,\\\
\ \ \ \ \ \vdots \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \vdots \\\
n^{n-1}c\_{n-1}+n^{n-2}c\_{n-2}+\dots +nc\_1+c\_0=p_n,
\end {cases}
\end {equation}
\\]

In matrix notation, this can clearly be written as
\\[
\begin {equation}
A\_n\bsl {c}\_n=\bsl {p}\_n,
\end {equation}
\\]
where
\\[
\bsl {c}\_n=\begin {pmatrix}
c\_{n-1}\\\ c\_{n-2}\\\ \vdots \\\ c\_1 \\\ c\_0
\end {pmatrix},\ \ \ \ \ \bsl {p}\_n=\begin {pmatrix}
2 \\\ 3 \\\ \vdots \\\ p\_{n-1}\\\ p\_{n}
\end {pmatrix},
\\]
and
\\[
A_n=\begin {pmatrix}
1 & 1 & \dots & 1 & 1 \\\
2^{n-1} & 2^{n-2} & \dots & 2 & 1 \\\
\vdots & \vdots & & \vdots & \vdots & \\\
n^{n-1} & n^{n-2} & \dots & n & 1 
\end {pmatrix},\ \ \ a_{ij}=i^{n-j}.
\\]
