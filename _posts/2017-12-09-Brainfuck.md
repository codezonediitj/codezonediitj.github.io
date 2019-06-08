---
layout: post
title:  "Brainfuck"
date:   2017-12-09
author: "Gagandeep Singh"
excerpt: "+++++++[>++++++++++<-]>+++.>+++++++[>++++++++++<-]>++++.

Confused? If yes, then I just wanted to say HI but the language here is the infamous esolang, the brainfuck. "
---

+++++++[>++++++++++<-]>+++.>+++++++[>++++++++++<-]>++++.

Confused? If yes, then I just wanted to say HI but the language here is the infamous esolang, the brainfuck. It seems weird but the purpose of the language is to look weird. Let’s dive more into this mysterious looking language that is sufficient to blog one’s mind.

This language uses just eight commands, yes just eight. They are, “><+-.,[]” and that’s it. Isn’t it amazing that we can use just those limited characters to convey what we want to say. The idea of this language was brought into reality by Urban Muller in 1993. Let me tell you how the first line prints, “HI”. Actually, brainfuck is represented by an array of 30000 cells each initialized with a value of 0. ‘+’ increments that value by 1. So, I did seven times ‘+’ and hence value of cell#1 increased by 6. Now, ‘[‘ is the beginning of the loop. ‘>’ moves the data pointer to cell#2 and 10 times ‘+’ increases that value by 10. ‘<’ moves the data pointer back to cell#1 and ‘-‘ decreases its value by 1. The loop continues until value at cell#1 becomes 0. Then I moved to cell#2 and increased its value by 3 and the final value there is 73 which corresponds to ‘H’ and the ‘.’ prints that. So much pain in just printing one letter.

Actually, there is class of such languages just like, ‘brainfuck’, which is known as esoteric programming languages, or in short esolangs. These are not meant for mainstream programming, instead these are for hobbyists. The first one of this kind was, INTERCAL, short for “Compiler Language With No Pronounceable Acronym” which was created in 1972. In addition, in 1993, one more language named as FALSE, appeared, which has a compiler of only 1024 bytes. You might be knowing Pikachu, yes that cartoon character. There is an esolang with that name too. The interesting thing about it, is that it uses only three elements, pi, pika and pikachu. It is quite funny in this sense. Now adding to your surprise, there is a language named, Shakespearean Programming Language. Yes, it’s true. The most interesting part of the language is that you can use variable names only from Shakespearean characters.

And the list goes on and on and on. There are plenty of such languages. You can even create one language of yours just for fun. How about a language which uses only currency symbols? Try it out!!!

Thank you for reading this article. If you find anything incorrect then please mention in the comments section.
