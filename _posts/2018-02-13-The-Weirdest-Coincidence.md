---
layout: post
title:  "The Weirdest Coincidence"
date:   2018-02-13
author: "Kunal Borse"
excerpt: "While thinking about the ‘Kaprekar constant’, I came across another constant. The following constant is defined for a four digited number. The process to be followed is described below."
is_pinned: false
---

While thinking about the ‘Kaprekar constant’, I came across another constant. The following constant is defined for a four digited number. The process to be followed is described below.

We take a random four digited number, say ‘abcd’ (in decimal form). Then we arrange its digits in an ascending and descending order, and divide both these into two 2 digited numbers, and perform the following.Let a>b>c>d without loss of generality,

abcd -ab and cd

dcba- dc and ba

We calculate (ab)^2 +(cd)^2 – (dc)^2 – (ba)^2

We do the process again after getting the result, until we keep getting the same result.

On getting a three digited number, we consider it to be four digited by adding a zero to the left.

What I observed was that we always get the number 1782 or 0 after performing this operation.

It is quite easy to see that 1782 again gives 1782 on subjected to this process.

I checked this using a C program and I got the following output.

Precisely, 1840 numbers give zero on performing this operation, while 7160 numbers give 1782.

I call this number the 'DOUBLE SQUARE CONSTANT'.

Let us take a few examples.

1) 1350

After arranging in descending and ascending order we get 5310 and 0135.

(53)^2+(10)^2-(01)^2-(35)^2=1683

Doing the same operation on 1683, we get 3564.

Doing the same operation on 3564, we get 1782!

It may be noted that we will again get 1782 if we do this process again on 1782.

2) 1356

After arranging in descending and ascending order we get 6531 and 1356.

(65)^2+(31)^2-(13)^2-(56)^2=1881

It is quite easy to see that on doing the operation on 1881, we get the answer as 0.

Another interesting property of the number 1782 is that 1782 times 4 is 7128!!

The coincidence here is the fact that this idea came to me on 7.2.18 !!

