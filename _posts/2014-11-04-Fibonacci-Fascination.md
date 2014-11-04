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
\sum\_{n=0}^\infty a\_n=\frac {1}{100}\sum\_{n=0}^\infty\frac {F\_n}{10^n}=\frac {1}{89}.
\\]

As I say, I think this is a fascinating result which has a fairly straightforward proof. It can be seen that if you have a sequence defined in such a way as the Fibonacci sequence, of the form
\\[
a\_{f(n+2)}=a\_{f(n+1)}+a\_{f(n)},
\\]
then by setting \\(a\_n=\lambda^n\\) that the solution can be found explicitly. For the case of the Fibonacci sequence, it can be found that
\\[
F\_n=a\left (\frac {1+\sqrt {5}}{2}\right )^n+b\left (\frac {1-\sqrt {5}}{2}\right )^n,
\\]
where \\(a,\ b\\) are found using the intial values \\(F\_0=1,\ F\_1=1\\).
