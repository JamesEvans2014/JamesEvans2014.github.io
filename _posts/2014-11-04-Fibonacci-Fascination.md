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
S:=\sum\_{n=0}^\infty a\_n=\frac {1}{100}\sum\_{n=0}^\infty\frac {F\_n}{10^n}=\frac {1}{89}.
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
Indeed, 
\\[
a=\frac {1+\sqrt {5}}{2\sqrt {5}},\ \ \ b=\frac {-1+\sqrt {5}}{2\sqrt {5}},
\\]
and hence
\\[
F\_n=\frac {1}{2}\left (\frac {1+\sqrt {5}}{\sqrt {5}}\right )\left (\frac {1+\sqrt {5}}{2}\right )^n+\frac {1}{2}\left (\frac {-1+\sqrt {5}}{\sqrt {5}}\right )\left (\frac {1-\sqrt {5}}{2}\right )^n,
\\]

Hence, dividing through by \\(10^{n+2}\\) and summing yields the expression
\\[
S=\frac {1}{200}\left (\frac {1+\sqrt {5}}{\sqrt {5}}\right )\sum\_{n=0}^\infty\left (\frac {\phi}{10}\right )^n+\frac {1}{200}\left (\frac {-1+\sqrt {5}}{\sqrt {5}}\right )\sum\_{n=0}^\infty\left (\frac {\bar {\phi}}{10}\right )^n,
\\]
where \\(\phi\\) is the golden ratio and \\(\bar {\phi}\\) is the conjugate root. Hence by convergence of a geometric series, it is achieved that
\\[
S=\frac {1}{200}\left (\frac {1+\sqrt {5}}{\sqrt {5}}\right )\left ( \frac {1}{1-\phi}\right )+\frac {1}{200}\left (\frac {-1+\sqrt {5}}{\sqrt {5}}\right )\left ( \frac {1}{1-\bar {\phi}}\right )
\\]
A simplification of the above yields the result:
\\[
S=\frac {1}{89}.
\\]

Not too difficult to show (if you don't mind the algebra!) but nonetheless interesting. Off course if you write it out explicitly, you can see the Fibonacci sequence emerge within the decimal expansion for 1/89:
\\[
\begin {aligned}
\frac {1}{89}= & 0.01123595505618\dots\\
= & 0.01\\\
+ & 0.001\\\
+ & 0.0002\\\
+ & 0.00003\\\
+ & 0.000005\\\
+ & 0.0000008\\\
+ & 0.00000013\\\
+ & 0.000000021\\\
+ & \vdots
\end {aligned}
\\]

Hope you found this as interesting as I did!
