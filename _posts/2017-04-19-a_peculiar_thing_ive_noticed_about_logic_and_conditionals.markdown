---
layout: post
title:  "A peculiar thing I've noticed about Logic and Conditionals"
date:   2017-04-19 10:48:00 +0000
---


While doing If Statement labs, I've noticed one important thing - the order in which you put your conditions matters. Ruby reads the first expression and runs it if it evaluates to true. Taking that into consideration, I had to be careful working on two labs - Fizzbuzz and Speak to Grandma.

In Fizzbuzz, the first condition was to return Fizz if an integer is evenly divisible by 3. The first thought would be making it the first condition in my If Statement. Instead, the first statement was supposed to be the third condition - return Fizzbuzz if the number is evenly divisible by both 3 and 5. If I made Fizzbuzz a part of the elsif condition, Ruby would never run it because it would return either Fizz or Buzz whenever a number is evenly divisible by either 3 or 5. 

In Speak to Grandma the trick was to pass "I LOVE YOU GRANDMA" before "elsif phrase == phrase.upcase" because the former phrase IS written in capital letters and it would always return "NO, NOT SINCE 1938!". 

So, the most specific condition comes before the more general one. That is what confused me at first.
