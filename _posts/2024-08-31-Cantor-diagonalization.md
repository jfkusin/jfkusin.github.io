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
WIP

Cantor proved that there are no bijective functions from the natural numbers to the real numbers, and thus they have different cardinalities. His diagonal proof shows there's an injective function but no bijective function and thus \\(\lvert \mathbb{R}| > \rvert \mathbb{N}\\). Injection but no bijection implying a strict ineqaulity is a definition of cardinality. \\(\mathbb{R}\\) is thus a "larger" infinity.

We'll break down the proof method and explain the main concepts along the way.

There's a bijection, and thus equal cardinality, between \\(\mathbb{N}\\) and \\(\mathbb{R}\\) if and only if (\\(\iff\\)) there is at least one bijective function from \\(\mathbb{N} \to \mathbb{R}\\). 
Remember a bijective function \\(f\\), in this case from \\(\mathbb{N} \to \mathbb{R}\\), implies an inverse function, i.e. another bijective function, in this case \\(f^-1\\) from \\(\mathbb{R} \to \mathbb{N}\\).
This means we only need to attack one function of a function-inverse function (bijective) pair to disprove a bijection and thus disprove a shared cardinality between the naturals and reals.

This method by Cantor disproves the bijection from \\(\mathbb{N} \to \mathbb{R}\\) and shows the bijection fails because there are too many reals compared to the naturals. Hence the reals are a greater infinity. 



