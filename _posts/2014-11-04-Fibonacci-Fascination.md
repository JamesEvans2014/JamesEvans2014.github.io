---
layout    : post
title     :  "Fibonacci Fascination"
date      :   2014-11-04 10:32:56
categories: Fibonacci Numbers 
---

I was reading something the other day that caught my eye with relation to the Fibonacci numbers. If you're unfamiliar with the sequence construction, it goes as follows:

Let \\(F\_n\\) represent the \\(n\\)th Fibonacci number with is obtained from the sequence relation
\\[
F\_{n+2}=F\_{n+1}+F\_n,\ \ \ F\_0=1,\ F\_1=1.
\\]
The sequence therefore is:
\\[
1,1,2,3,5,8,13,21,34,55,89,\dots
\\]
This sequence has been well documented and well studied over it's vast history but there is one particular property I wish to lok at (and prove) which I came across. That property is thus:

Let \\(F\_n\\) represent the \\(n\\)th Fibonacci number. Define the sequence \\(a\_n\\) to be 
\\[
a\_n=\frac {F\_n}{10^{n+2}}.
\\]
Then
\\[
\frac {1}{100}\sum\_{n=0}^\infty\frac {F\_n}{10^n}=\frac {1}{89}.
\\]
