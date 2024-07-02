---
layout: post
title:  "Arithmetic"
date:   2024-07-02 00:00:00 +0700
categories: lecture notes
katex: True
---

## Natural Numbers

Let us begin with some basic notions of arithmetic (number theory):  

* Natural numbers: $$\mathbb{N} = \{0, 1, 2, \ldots \} $$  
(Here, $$\mathbb{N}$$ represents the _set_ of natural numbers.)  

Notice that the only reasonable operation to perform on the natural numbers is addition, and conseqeuently multiplication, which is simply repeated addition in our case.  

Also, it appears that we just need 0 and 1 in order to express any natural number in terms of addition. As an example, $$4 = ((((0 + 1) + 1) + 1) + 1)$$, meaning perhaps, the symbol 4 is simply a representation of four instance of 1's in series. For a deep explanation on this, look into [Peano Axioms](https://en.wikipedia.org/wiki/Peano_axioms).

## Integers

When dealing with the natural numbers, notice that subtraction and division are not always meaningful. As an example, notice that $$1 - 2 = -1$$, which is not a natural number, and $$1 \div 2 = \frac{1}{2}$$, which is also not a natural number. So, we need to be slightly more cautious when dealing with subtraction and division.

So, what are the requirement in order to facilitate subtraction? Let us recall that _subtraction_, in an algebraic sense, is addition by the negative, technically referred to as the additive inverse. So, now we introduce the notion of **integers**:

* Integers: $$\mathbb{Z} = \{\ldots, -2, -1, 0, 1, 2, \ldots\}$$  
(Here, $$\mathbb{Z}$$ represents the set of integers. Z stands for Zahlen, German for numbers).  

Now, the number 0 has a bit more significance than it did with just the natural numbers. Of course, any number added to 0 is simply that number. This was true with the natural numbers as well. However, with the introduction of the negative whole numbers, we also see that whenever a number is paired with its negative in addition, the sum will always be 0. In this sense, we refer to 0 as the _additive identity_, and analogously, we say that 1 is the _multiplicative identity_ as any number multiplied by 1 is simply itself. So, what is up with all the fancy terms here? You will see why when we start discussing division.

## Divisibility

In a similar sense, it appears that the existence of _fractions_ is the requirement to facilitate the operation that we referred to as division. Analogously, in an algebraic sense, division is multiplication by the _multiplicative inverse_, and we refer to the inverse here as the **reciprocal**. 

The notion of fraction and division are closely related - at the end of the day, the quantity in question is part over whole, and computationally, we find such value by performing long-division. 

As far as addition and subtraction were concerned, it appears that for all integers, there exists a negative inverse, namely the _opposites_. For examples, $$1 + (-1) = 0$$, $$(-50) + -(-50) = 0$$, and similarly, $$0 + (-0) = 0$$. So, a natural question to ask is, **does any integer have a reciprocal?**

For the most part, yes, with one critical exception - namely zero. To see why 0 does not have a reciprocal, i.e. the multiplicative inverse, let us consider what we mean by being able to divide in the first place. As a motivating example, we see that 3 divides into 27 because 3 times 9 is 27. We see that 5 divides into 40 because 5 times 8 is 40.  

Similarly, we see that 2 does not divide into 5 because 2 times 2 is 4 and 2 times 3 is 6. There are no integers strictly between 2 and 3, and it appears that such figure is precisely the requirement for 5 to be divisible by 2. Let us formalize this intuition.  

We say a number is divisible by the divisor if there exists some integer such that the integer times the divisor is the number. In other words, an integer $$d$$ divides into another integer $$n$$ if there exists an integer $$k$$ such that $$n = dk$$, meaning $$d$$ times $$k$$ (More on variables in Unit 2).  

So, if 0 has a reciprocal, then that means 0 divides into some integer. As a concrete example, let's see if 0 divides 100. Suppose that 0 divides 100. Then, it looks like 0 times some integer is 100. However, 0 times any number is simply 0. Does 100 equal to 0? Only if you get robbed, meaning this was probably a nonsense to begin with, and we claim that 0 does not divide 100.  

As a matter of fact, 100 can be replaced with any nonzero integer, and the same conclusion holds. This implies that 0 does not divide any number and hence there does NOT exist a reciprocal (the multiplicative inverse) for 0.

With this notion of divisibility, let us see what kind of integers are divisible and what kind of integers are indivisible. This concept reduces to the existence of the prime numbers and the composite integers.

## Primality

We witnessed how any natural number can be represented by adding a _bunch_ of 1's. In a similar sense, can we represent any negative integer with a repeated addition of -1. As an example, see that -3 = (-1) + (-1) + (-1). So, as the bare minimum, it appears that -1, 0, and 1 are the _building blocks_ for the set of integers in the context of addition. What kind of analogy can we make here in regards to multiplication?  

In other words, can we represent any integer by multiplying a bunch of numbers? If so, what are those _numbers_ called? This brings us to the notion of [the Fundamental Theorem of Arithmetic](https://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic), which states that:  

**Any natural number greater than 1 is either a prime, or a product of primes, where such product is uniquely determined by the primes and their exponents.** (Uniqueness here simply means there is only one way and one way only to write such _prime factorization_. As an intuitive example, $$4 = 2^2$$, and this is the only way to express 4 as a product of primes.)  

This proposition binds nicely with the definition of prime and composite numbers. Hence, let us recall that:  

> * Prime: any natural number greater than 1 that is divisible by only 1 and the number itself.  
> * Composite: any natural number greater than 3 that is not prime. 

What about 1? Well, first of all, 1 is not greater than 3, so it certainly is not composite. Is it prime then? Unfortunately, [no](https://en.wikipedia.org/wiki/Prime_number#Primality_of_one). Therefore, we say that, by convention, **1 is neither a prime nor a composite**.  

And lastly, this argument works for any integer, as any nonnegative integer is simply a natural number and a negative integer is simply a natural number multiplied by -1, where the natural numbers here have unique prime factorization to begin with.  

## Rational Numbers

Now, we have enough background to really _define_ what we mean by fractions. Mathematicians refer to fractions as the _rational numbers_, hence both the terms will be used interchangeably.

> * Rational number: a number of the form $$\frac{n}{d}$$, where  
>    1. $$n$$ and $$d$$ are integers  
>    2. $$d$$ is not zero (For the reasons detailed in the above section)
>    3. all common primes of $$n$$ and $$d$$ in their prime factorizations have been cancelled out. In other words, the fraction is in its _simplest form_.  

As you may have guessed, $$n$$ stands for the numerator, the top number, and $$d$$ stands for denominator, 

If these conditions are not satisfied, then we are looking at a number that appears to be a fraction but it really is not a fraction, mathematically speaking. We refer to the set of rational numbers with the symbol $$\mathbb{Q}$$. Why Q? Please let me know if you figure this out. 

Lastly, we can easily see that all integers are rational numbers: simply set the denominator to be 1. 

In the following section, the notion of variables will be slightly more formalized along with the review of the arithmetic operations on the rational numbers.