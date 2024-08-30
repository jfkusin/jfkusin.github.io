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

### A simple but detailed that the natural numbers are countably infinite but the real numbers are uncountably infinite:

First recognize that there is a **set** of all natural numbers. The concept of a set is *critical* to this proof. This a good thing because sets are a very easy to understand concept and provide much of the 
reasoning in the proof. It's what allows us to talk about *all* the natural numbers. Does that mean we can actually write all of them down? No. But we can describe the set of all of them. The set of natural numbers, called \\(\mathbb{N}\\), simply means we can completely collect all of the natural numbers. Does that mean I write down every natural number from 1...5004...999000... and fill up 
endless pages? No. It means I simply recognize there is a way to conceptually talk about this complete collection and write about it using mathematical symbols in a consistent way. We call this set \(\mathbb{N}\\), the set of all natural numbers.

We intuitively order \\(\mathbb{N}\\) in the usual way (1, 2, 3...) as rows in the table below (we'll ignore 0 here, it changes nothing). Next to each natural number, we're going to write a unique real number from the set of all real numbers \\(\mathbb{R}\\) between 0 and 1, written as \\((0,1)\\). We don't need all the real numbers, just this subset of them, to show all the naturals run out before "naming" all the reals. How can we intuitively 
write down a unique real number  next to each natural number? Real numbers have a property that strictly between any two different reals, there is another real number. This property gives us a repeatable mechanism to write down a different real next to each of the enumerated naturals. Natural numbers clearly don't have this property. Between 1 and 2 there are is no natural number. Let's recap to seal the reasoning. We've given a way to write down every natural number in the first colum, by doing it in their natural order. We've given a way to pick any two different reals and then repeatedly generate new reals. With this property of the reals and the set of naturals listed, we can now easily populate column 2 with a different real for each natural. 

Remember, we are leveraging the definition of set to completely collect all of the naturals, and then listing them because of their well-ordering property. Actually, we can in principle order any set this way (a well ordering, a list, a column) by assuming the Axiom of Choice. We don't need the Axiom of Choice to list the naturals since their ordering is more basic (from the Axiom of Induction or just intuition really). Our method is to list the naturals first, assigned a unique real from \\((0,1)\\) to each, and then find an extra real not on the list. Rather than use the iterated method of generating reals, we choose less arbitrary ones for simplicity's sake. This doesn't change the proof.  We do this graphically with a table:

|\\(\mathbb{N}\\) |\\((0,1)\\)   | 
--- | --- |
|1|0.3141592...|
|2|0.4669201...|
|3|0.7071067...|
|4|0.2718281...|
|⋮| ⋮           |

We exhaust every natural number in doing so. However large the set of all natural numbers is, each one has it's own row in the table.
We've used all of \\(\mathbb{N}\\) in the first column. 

We will be able to show an infinite number of real numbers will be not on this completed list. By doing so we will show the real numbers
are uncountably infinite.

To show there is at least one extra real number, first highlight digits in the main diagonal, one for every row of \\(\mathbb{N}\\), as shown:

|\\(\mathbb{N}\\) |\\((0,1)\\)   | 
--- | --- |
|1|0.**3**141592...|
|2|0.4**6**69201...|
|3|0.70**7**1067...|
|4|0.271**8**281...|
|⋮| ⋮           |

If we then change each digit in this diagonal, such as by adding 1, the real number formed is not already in the table (not anywhere in the second column). That new real number in this example is 0.4789... Why is it not in the table? Because it differs from 
the real number in row 1 by its first decimal digit, row 2 by its second, row 3 by its third, etc. We can also think of it like so: does this real number equal the real number in row 1? No. Does it equal the real number in row 2? No. And so on. 
It differs from each real number already in the table and it is a real number. There are no more natural numbers left to assign it to since we've said the table uses all of the natural numbers in the first column. Therefore we've 
run out of natural numbers, but we have more real numbers (by one extra) than natural numbers. In fact we can keep generating new real numbers, infinitely many, that aren't already in this table in similar ways by changing different sets of digits as long
as we can change one in each column of decimal digits and one in each row of real numbers. A diagonal is simply an easy way to satisfy this condition. There are infinite diagonals and highlighting methods since reals, and many ways to add changes. We can actually change multiple decimal digits in each row, but only at most one in each column. 

Since \\(\mathbb{N}\\) is infinite, and \\(\mathbb{R}\\) is "larger" (has a larger cardinality), we can now confidentally and consistently call \\(\mathbb{N}\\) countably infinite and \\(\mathbb{R}\\) uncountably infinite.
That's it. Due to the concept of sets, which are carefully defined to not lead to contradictions, we can leverage their simple nature to show the set of natural numbers, while infinite, is a smaller infinity than the real numbers. 



