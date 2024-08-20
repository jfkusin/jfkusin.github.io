---
layout: post
title: A simple abstract algebra proof
subtitle: 
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
mathjax: true
tags: [math, abstract algebra, proof]
author: Julian Kusin
---

Suppose $$a$$ and $$b$$ belong to a commutative ring and $$ab$$ is a zero-divisor. Show that either \\(a)\\ or \\(b)\\ is a zero-divisor.

Given \\(a, b \in R\\) where \\(R)\\ is a commutative ring and \\(ab \neq 0)\\. By definition of zero divisor \\(\exists c \in R)\\ such that \\(c \neq 0\))
and \\((ab)c = 0\\). By associativity and commutativity \\((ab)c = 0 = a(bc) = b(ca) by associativity and commutativity)\\. 

From \\(a(bc) = 0)\\ we get \\(a = 0)\\ or \\(bc = 0)\\. If \\(bc = 0)\\ then \\(b)\\ is a zero divisor or \\(b = 0\\), but \\(b)\\ can't equal \\(0)\\ because that
would make \\(ab = 0\)), which contradicts our given that \\(ab)\\ is a non-zero element of \\(R)\\ by definition of being a zero divisor. Thefore \\(b)\\ is a zero divisor. 
We can do the same for \\(b(ca) = 0)\\ to show \\(a)\\ is also a zero divisor. This completes our proof.

