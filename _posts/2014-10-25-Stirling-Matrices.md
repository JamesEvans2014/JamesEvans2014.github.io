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
\begin {align}
p\_1(x) & = 2,\\\
p\_2(x) & = 1+x,\\\
p\_3(x) & = \frac {1}{2}(4-x+x^2),\\\
p\_4(x) & = \frac {1}{6}(18-14x+9x^2-x^3),\\\
p\_5(x) & = \frac {1}{24}(144-206x+141x^2-34x^3+3x^4),\\\
p\_6(x) & = \frac {1}{120}(1800-3496x+2730x^2-987x^3+150x^4-9x^5),\\\
p\_7(x) & = \frac {1}{720}(27360-61548x+53732x^2-22515x^3+4925x^4-537x^5+23x^6).
\end {align}
\\]

