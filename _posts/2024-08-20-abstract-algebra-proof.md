---
layout: post
title: An abstract algebra proof using zero divisors
subtitle: 
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
mathjax: true
tags: [math, abstract algebra, proof]
author: Julian Kusin
---

Suppose \\(a\\) and \\(b\\) belong to a commutative ring and \\(ab\\) is a zero-divisor. Show that either \\(a\\) or \\(b\\) is a zero-divisor.

Given \\(a, b \in R\\) where \\(R\\) is a commutative ring and \\(ab \neq 0\\). By definition of zero divisor \\(\exists c \in R\\) such that \\(c \neq 0\\)
and \\((ab)c = 0\\) (meaning \\(c\\) is also a zero divisor. This is because zero divisor has a mutual property). By associativity and commutativity \\((ab)c = 0 = a(bc) = b(ca)\\). 

From \\(a(bc) = 0\\) we get \\(a = 0\\) or \\(bc = 0\\). \\(a\\) can't equal \\(0\\) because that would make \\(ab = 0\\) which contradicts our given that \\(ab\\) 
is a  non-zero element of \\(R\\) by definition of being a zero divisor. If \\(bc = 0\\) then \\(b\\) is a zero divisor or \\(b = 0\\), but \\(b\\) can't equal \\(0\\) 
because that would make \\(ab = 0\\). Thefore \\(b\\) is a zero divisor. 

We can do the same for \\(b(ca) = 0\\) to show \\(a\\) is also a zero divisor. This completes our proof.

I think there is a bit of redundancy in this proof but it makes the proof clearer in some ways. I'm using Gallian's [*Contemporary Abstract Algebra*](https://www.amazon.com/Contemporary-Abstract-Algebra-Textbooks-Mathematics/dp/0367651785/ref=pd_lpo_sccl_1/131-9942725-2254717?pd_rd_w=h1xuF&content-id=amzn1.sym.4c8c52db-06f8-4e42-8e56-912796f2ea6c&pf_rd_p=4c8c52db-06f8-4e42-8e56-912796f2ea6c&pf_rd_r=DW2YZ3DS8DSMW10QW59D&pd_rd_wg=QHLH9&pd_rd_r=9f148064-e5a9-48a0-bf53-92e94d09782a&pd_rd_i=0367651785&psc=1)
for definitions. If you want to know more about proofs in general I recommend Velleman's [*How to Prove It: A Structured Approach*](https://www.amazon.com/How-Prove-Structured-Approach-2nd/dp/0521675995). 


