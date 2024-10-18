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

Cantor proved that there are no bijective functions from the natural numbers to the real numbers, and thus they have different cardinalities. His diagonal proof shows there's an injective function from \\(\mathbb{N} \to \mathbb{R}\\) but no bijective function and thus \\(\lvert \mathbb{R} \rvert > \lvert \mathbb{N} \rvert \\). Injection but no bijection implying a strict ineqaulity is a definition of cardinality. \\(\mathbb{R}\\) is thus a "larger" infinity.

There's a bijection, and thus equal cardinality, between \\(\mathbb{N}\\) and \\(\mathbb{R}\\) if and only if (\\(\iff\\)) there is at least one bijective function from \\(\mathbb{N} \to \mathbb{R}\\). 
Remember a bijective function \\(f\\), in this case from \\(\mathbb{N} \to \mathbb{R}\\), implies an inverse function, i.e. another bijective function, in this case \\(f^{-1}\\) from \\(\mathbb{R} \to \mathbb{N}\\).
This means we only need to attack one function of a function-inverse function (bijective) pair to disprove a bijection and thus disprove a shared cardinality between the naturals and reals.

The broad idea is to "list" all of the naturals, where listing means give a finite description or explanation clearly showing how one *would enumerate them* ***in order*** if one had infinite time, show each one maps to a different real (showing an injection), and then showing a new real can be produced that's not on the list already, meaning  no natural maps to it (since they're all already "listed") and thus there can't be an inverse function over the whole set of reals to naturals, and likewise no bijection.

I'm going to make the codomain the entire set of reals. This is slightly unconvential but makes the proof easier to see in my opinion. The barebones are still the same.

Let: \\(f: \mathbb{N} \to \mathbb{R} \\), then:

| \\(\mathbb{N}\\) | \\(\mathbb{R}\\) |
| --- | --- |
| 0 | \\(\frac{1}{2}\\) |
| 1 | \\(\frac{1}{4}\\) |
| 2 | \\(\frac{1}{8}\\) |
| 3 | \\(\frac{1}{16}\\) |
| 4 | \\(\frac{1}{32}\\) |
| ⋮ | ⋮ |

Clearly each value in the second column is a different real. But it's not listing all of the realss as there are only reals from \\([0,1]\\) thus far. The naturals are listed however.

And when I do this:

| ? | 3.14159.... |
| --- | --- |


This method by Cantor disproves the bijection from \\(\mathbb{N} \to \mathbb{R}\\) and shows the bijection fails because there are too many reals compared to the naturals. Hence the reals are a greater infinity. 



