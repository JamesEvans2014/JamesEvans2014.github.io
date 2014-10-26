---
layout    : post
title     :  "The Curl Operator"
date      :   2014-10-26 14:25:31
categories: Curl Operator Kernel Multiply Connected Domains
---

\\(\textbf {Kernel of the curl Operator}\\)

Let \\(\Omega \subset \mathbb {R}^3\\) be a fairly general domain. As is probably well known, if one considers the 
equation
\\[
\begin {equation}
\textbf {curl} \ \boldsymbol {v}(\boldsymbol {x})=\boldsymbol {0},\ \ \ \boldsymbol {x}\in \Omega,\ 
\boldsymbol {v}\in L^2(\Omega),
\end {equation}
\\]
where \\(\Omega\\) is both bounded and simply connected, then 
\\[
\begin {equation}
\text {ker}\ \textbf {curl} := \text {ker}\{ \textbf {curl},\ L^2(\Omega)\}=\nabla H^1(\Omega)
:=\{ \boldsymbol {v}(\boldsymbol {x})=\nabla w(\boldsymbol {x})\ |\ w\in H^1(\Omega)\}.
\end {equation}
\\]
Strictly speaking one should impose suitable boundary conditions on \\(\partial\Omega\\) but so long as the boundary 
is sufficiently regular, this is not an issue. Looking at this, it is not too difficult to extend this result to 
unbounded, simply connected domains by imposing a sufficient decay at infinity such that the functions in the kernel
are \\(L^2(\Omega)\\), i.e., if \\(\boldsymbol {v}\in \text {ker}\ \textbf {curl}\\) where \\(\Omega\\)
is simply connected and unbounded, then as \\(|\boldsymbol {x}|\tends \infty\\), \\(\boldsymbol {v}(\boldsymbol {x}) 
=O( \frac {1}{|\boldsymbol {x}|^2})\\).

The case when \\(\Omega\\) is bounded and multiply-connected has been considered before 
and will be formulated here for completeness. Let \\(\Omega\\) be a bounded connected domain which lies wholly 
on one side of it's boundary \\(\dpar\Omega\\) of dimension 2 and of the class \\(C^k\\) where \\(k\geq 2\\). 
Let \\(\partial \Omega\\) have a finite number of connected components denoted \\(\Gamma\_0,\dots ,\Gamma\_n\\) where 
\\(\Gamma\_0\\) denotes the boundary of the infinite connected component of 
\\(\Omega'=\mathbb {R}^3\backslash\bar {\Omega}\\). For domains which are multiply connected, it is common to come 
across the notion of a ``cut''. There is some dispute in the literature as to the purpose of these cuts but the 
purpose is that a multiply connected domain \\(\Omega\\) with these cuts (defined below) removed should be such that 
every curl free field is the gradient of some scalar field in \\(\Omega\\) minus these cuts. Formally, one defines cuts
on a multiply connected domain as follows.

\\(\textbf {Definition}\\)

Let \\(\Sigma_1,\dots,\Sigma_m\\) be a collection of smooth surfaces such that 

\begin {enumerate}
\item \\(\Sigma\_1,\dots,\Sigma\_m\\) are open subsets of smooth manifolds 
\\(\mathcal {M}\_1,\dots ,\mathcal {M}\_m\\) respectively,
\item the boundary of each \\(\Sigma\_i\\) is contained in \\(\dpar\Omega\\),
\item the intersection of any two cuts is empty, i.e., \\(\Sigma\_i\cap\Sigma\_j=\emptyset\\), \\(i\neq j\\),
\item the open set \\(\Omega'=\Omega\backslash\bigcup\_{i=1}^m\Sigma\_i\\) is simply connected and 
pseudo-Lipschitz (For the definition of pseudo-Lipschitz, 
see [Lipschitz Domain](http://en.wikipedia.org/wiki/Lipschitz_domain)).
\end {enumerate}

Then we call \\(\Sigma\_1,\dots ,\Sigma\_m\\) a collection of cuts for the domain \\(\Omega\\).


Hence, without going through the construction, one can prove the following result:

\\(\textbf {Proposition}\\)

Let \\(\Omega\\) be an open set which is bounded and multiply connected in \\(\mathbb {R}^3\\)
satisfying the hypothesis described above. The kernel of the curl in \\((L^2(\Omega))^3\\) is the sum of two orthogonal
spaces; \\(\del H^1(\Omega)\\)and \\(\mathbb {H}\_1\\) which is a vector space of dimension \\(m\\)
(the number of cuts required to make \\(\Omega\\) simply connected) defined by
\\[
\begin {multline}
\mathbb {H}\_1=\Big \{ \boldsymbol {v}\in (L^2(\Omega))^3\ \Big |\ \boldsymbol {v}=\nabla w,\ \text {in}\ \Omega \\ 
\text {with} \ w\in H^1(\Omega')\ \text {a solution of the problem below}\Big \},
\end {multline}
\\]
where the problem in question is as follows
\\[
\begin {equation}
\begin {cases}
\Delta w=0,\ \ \ \text {in}\ \Omega',\\\
\frac {\partial w}{\partial n}\big {|}\_\Gamma =0,\\\
[w]_{\Sigma\_i}=\text {constant},\ \ \ i=1,\dots, m,\\\
\Big [ \frac {\partial w}{\partial n}\Big ]\_{\Sigma\_i}=0,\ \ \ i=1,\dots,m.
\end {cases}
\end {equation}
\\]
where \\([w]\_{\Sigma\_i} = w|_{\Sigma\_i^+}-w|_{\Sigma\_i^-}\\)

The question now becomes can this result be extended to domains which are both multiply connected and unbounded? 
One would think that it would be a combination of this result and the requirement that there is sufficient decay 
at infinity of the solutions to the various equations involved. However, it has been the case that no such solution 
has been found thus far. This may suggest that one needs to weaken the solution space to allow a greater variety 
of functions or failing that, a more detailed analysis of the kernel of the curl operator in unbounded multiply 
connected domains be carried out.
