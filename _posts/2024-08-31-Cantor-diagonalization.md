---
layout: post
title: Simple but detailed proof of Cantor's Diagonalization
subtitle: Showing the reals are a greater infinity than the naturals
cover-img: /assets/img/diagonalback.png
thumbnail-img: /assets/img/diagon.png 
share-img: /assets/img/diagon.png
mathjax: true
tags: [math, sets, proof]
author: Julian Kusin

---
Cantor proved that there are no bijective functions from the natural numbers to the real numbers, and thus they have different cardinalities. His diagonal proof shows there's an injective function from \\(\mathbb{N} \to \mathbb{R}\\) but no bijective function can exist, and thus \\(|\mathbb{N}| < |\mathbb{R}|\\). Injection but no bijection implying a strict inequality is a definition of cardinality. \\(\mathbb{R}\\) is thus a "larger" infinity.

<!---
There's a bijection, and thus equal cardinality, between \\(\mathbb{N}\\) and \\(\mathbb{R}\\) if and only if (\\(\iff\\)) there is at least one bijective function from \\(\mathbb{N} \to \mathbb{R}\\). 
Remember a bijective function \\(f\\), in this case from \\(\mathbb{N} \to \mathbb{R}\\), implies an inverse function, i.e. another bijective function, in this case \\(f^{-1}\\) from \\(\mathbb{R} \to \mathbb{N}\\).
This means we only need to attack one function of a function-inverse function (bijective) pair to disprove a bijection and thus disprove a shared cardinality between the naturals and reals.
-->

The broad idea is to "list" all of the naturals (where listing means a finite description clearly showing how one *would* enumerate them *in an order* if one had infinite time), show each one maps to a different real (showing an injection), and then showing a new real can be produced that's not on the list already. Since no natural maps to it (since they're all already "listed"), there can't be a surjection and likewise no bijection.

Let: \\(f: \mathbb{N} \to [0,1] \\) be any injective function. Letting \\(f\\) be *any* injective function will show no surjection (and thus no bijection) exists. Since it's *any* injective function, pick arbitrary reals, and put them into infinite decimal expansion form:

$$
\begin{array}{c}
\begin{array}{c  ccccccccccc}
n & & & &  & & f(n) &  &  & &  &  &  &   &  & 
\end{array}
\\
\begin{array}{c | ccccccccccc}
\hline
1 & 0 & . & 3 & 1 & 4 & 1 & 5 & 9 & 2 & 6 & ... \\
2 & 0 & . & 4 & 6 & 6 & 9 & 2 & 0 & 1 & 6 & ...  \\
3 & 0 & . & 2 & 5 & 0 & 2 & 9 & 0 & 7 & 8 & ... \\
4 & 0 & . & 2 & 7 & 1 & 8 & 2 & 8 & 1 & 8 & ... \\
5 & 0 & . & 5 & 9 & 9 & 0 & 4 & 1 & 6 & 7 & ... \\ 
⋮ & ⋮
\end{array}
\end{array}
$$

While the first column is all of the naturals, the second column is not all of the reals. Why? Because any attempt to list them shows a real will be missed (that is not true for listing the naturals; we know every one will be listed, clearly). To create a real not on "the list", simply add \\(1\\) to 
the first digit past the decimal for row one, the second digit for row two, and so on (letting \\(9+1)\\) wrap around to \\(0\\):

$$
\begin{array}{c}
\begin{array}{c  ccccccccccc}
n & & & &  & & f(n) &  &  & &  &  &  &   &  & 
\end{array}
\\
\begin{array}{c | ccccccccccc}
\hline
1 & 0 & . & \textbf{3} & 1 & 4 & 1 & 5 & 9 & 2 & 6 & ... \\
2 & 0 & . & 4 & \textbf{6} & 6 & 9 & 2 & 0 & 1 & 6 & ...  \\
3 & 0 & . & 2 & 5 & \textbf{0} & 2 & 9 & 0 & 7 & 8 & ... \\
4 & 0 & . & 2 & 7 & 1 & \textbf{8} & 2 & 8 & 1 & 8 & ... \\
5 & 0 & . & 5 & 9 & 9 & 0 & \textbf{4} & 1 & 6 & 7 & ... \\ 
⋮ & ⋮
\end{array}
\end{array}
$$

Doing so, for *any* codomain for this injective function, with any attempt to list it, will always produce a new real not previously on the list. That's because it will differ from each number already "on the list" by one digit. Therefore, while a injection exists, no surjection will ever exist. Keep in mind, no surjection exists when *letting \\(f\\) be an injective function from the naturals*. Letting \\(f\\) be such a function is precisely the assumption we want to make. We have to have an injection to even attempt a bijection. And that we have one or many, and then no surjections, proves by definition 
\\(|\mathbb{N}| < |\mathbb{R}|\\). Hence the reals are a greater infinity. 



