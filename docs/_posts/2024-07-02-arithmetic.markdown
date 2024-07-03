---
layout: post
title:  "Fundamental Theorem of Arithmetic"
date:   2024-07-02 00:00:00 +0000
categories: lecture notes
katex: True
---

## Natural Numbers

Let us begin with some basic notions of arithmetic (number theory):

* Natural numbers: $$\mathbb{N} = \{0, 1, 2, \ldots \} $$
(Here, $$\mathbb{N}$$ represents the _set_ of natural numbers.)  

Notice that the only reasonable operation to perform on the natural numbers is addition, and consequently multiplication, which is simply repeated addition in our case.  

Also, it appears that we just need $$0$$ and $$1$$ in order to express any natural number in terms of addition. As an example, $$4 = ((((0 + 1) + 1) + 1) + 1)$$, meaning perhaps, the symbol $$4$$ is simply a representation of four instances of $$1$$ in additional series. For a deep explanation on this, look into [Peano Axioms](https://en.wikipedia.org/wiki/Peano_axioms).

## Integers

When dealing with the natural numbers, notice that subtraction and division are not always meaningful. As an example, notice that $$1 - 2 = -1$$, which is not a natural number, and $$1 \div 2 = \frac{1}{2}$$, which is also not a natural number. So, we need to be slightly more cautious when dealing with subtraction and division.

So, what are the requirement in order to facilitate subtraction? Let us recall that _subtraction_, in an algebraic sense, is addition by the negative, technically referred to as the additive inverse. So, now we introduce the notion of **integers**:

* Integers: $$\mathbb{Z} = \{\ldots, -2, -1, 0, 1, 2, \ldots\}$$  
(Here, $$\mathbb{Z}$$ represents the set of integers. Z stands for Zahlen, German for numbers).  

Now, the number $$0$$ has a bit more significance than it did with just the natural numbers. Of course, any number added to $$0$$ is simply that number. This was true with the natural numbers as well. However, with the introduction of the negative whole numbers, we also see that whenever a number is paired with its negative in addition, the sum will always be $$0$$. In this sense, we refer to $$0$$ as the _additive identity_, and analogously, we say that $$1$$ is the _multiplicative identity_ as any number multiplied by $$1$$ is simply itself. So, what is up with all the fancy terms here? You will see why when we start discussing division.

## Divisibility

In a similar sense, it appears that the existence of _fractions_ is the requirement to facilitate the operation that we referred to as division. Analogously, in an algebraic sense, division is multiplication by the _multiplicative inverse_, and we refer to the inverse here as the **reciprocal**. 

The notion of fraction and division are closely related - at the end of the day, the quantity in question is part over whole, and computationally, we find such value by performing long-division, e.g. repeated subtraction. 

As far as addition and subtraction are concerned, it appears that for all integers, there exists a negative inverse, namely the _opposites_. For examples, $$1 + (-1) = 0$$, $$(-50) + -(-50) = 0$$, and similarly, $$0 + (-0) = 0$$. So, a natural question to ask is, **does any integer have a reciprocal?**

For the most part, yes, with one critical exception - namely zero. To see why $$0$$ does not have a reciprocal, i.e. the multiplicative inverse, let us consider what we mean by being able to divide in the first place. As a motivating example, we see that $$3$$ divides into $$27$$ because $$3$$ times $$9$$ is $$27$$. We see that $$5$$ divides into $$40$$ because $$5$$ times $$8$$ is $$40$$.  

Similarly, we see that $$2$$ does not divide into $$5$$ because $$2 \times 2 = 4$$ and $$2 \times 3 = 6$$. There are no integers strictly between $$2$$ and $$3$$, and it appears that such figure is precisely the requirement for $$5$$ to be divisible by $$2$$. Let us formalize this intuition.  

We say a number is divisible by the divisor if there exists some integer such that the integer times the divisor is the number. In other words, an integer $$d$$ divides into another integer $$n$$ if there exists an integer $$k$$ such that $$n = dk$$, meaning $$d$$ times $$k$$.

So, if $$0$$ has a reciprocal, then that means $$0$$ divides into some integer. As a concrete example, let's see if $$0$$ divides $$100$$. In order for $$100$$ to be divisible by $$0$$, it looks like $$0$$ times some integer should be $$100$$. However, $$0$$ times any number is simply $$0$$. Does $$100$$ equal to $$0$$? Only if you get robbed, meaning this was probably a nonsense to begin with, and we claim that $$0$$ does not divide $$100$$.  

As a matter of fact, $$100$$ can be replaced with any nonzero integer, and the same conclusion holds. This implies that $$0$$ does not divide any number and hence **there does NOT exist a reciprocal (the multiplicative inverse) for zero**.

With this notion of divisibility, let us see what kind of integers are divisible and what kind of integers are indivisible. This concept reduces to the existence of the prime numbers and the composite integers.

## Primality

We witnessed how any natural number can be represented by adding $$1$$ __a bunch of times__. In a similar sense, can we represent any negative integer with a repeated addition of $$-1$$. As an example, see that $$-3 = (-1) + (-1) + (-1)$$. So, as the bare minimum, it appears that $$\{-1, 0, 1\}$$ are the _building blocks_ (technically known as the __generators__) for the set of integers in the context of addition. What kind of analogy can we make here in regards to multiplication?  

In other words, can we represent __any integer__ by multiplying a bunch of numbers? If so, what are those numbers called? This brings us to the notion of [the Fundamental Theorem of Arithmetic](https://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic), which states that:  

**Any natural number greater than 1 is either a prime, or a product of primes, where such product is uniquely determined by the primes and their exponents.** (Uniqueness here simply means there is only one way and one way only to write such _prime factorization_. As an intuitive example, $$8 = 2 \times 2 \times 2 = 2^3$$, and this is the only way to express $$8$$ as a product of primes. The small $$3$$ in the upper right corner indicates an exponent, which is the number of repeated multiplication with the same number, also known as the __base__: $$2$$ in our case here.)  

This proposition binds nicely with the definition of prime and composite numbers. Hence, let us recall that:  

* Prime: any natural number greater than $$1$$ that is divisible only by $$1$$ and the number itself.  
* Composite: any natural number greater than $$3$$ that is not a prime. 

This implies that $$2$$ is the least natural number that is prime and $$4$$ is the least natural number that is composite. Well, what about $$1$$? Well, first of all, $$1$$ is not greater than 3, so it certainly is not composite. Is it prime then? Unfortunately, [no](https://en.wikipedia.org/wiki/Prime_number#Primality_of_one). Therefore, we say that, by convention, $$1$$ **is neither a prime nor a composite**, and the same argument can be said about $$0$$ as well. 

Furthermore, this argument works for any integer, as any nonnegative integer is simply a natural number and a negative integer is a natural number multiplied by $$-1$$, where the natural numbers have unique prime factorization to begin with.  

## Computational Examples of Prime Factorization

* For any prime number $$p$$, $$p$$ is already in its factorization as there are no prime factors in a prime. For instance, $$31$$ is the only way to write the factorization as $$31$$ is already a prime to begin with.

* Let $$n=256$$. Notice that $$256 = 2 \times 2 \times 2 \times 2 \times 2 \times 2 \times 2 \times 2$$. Hence, we can say that $$256 = 2^{8}$$ is the prime factorization of $$256$$.

* Let $$n$$ be a composite number. Then, by the fundamental theorem of arithmetic, there exist unique prime factors for $$n$$. For instance, let us perform the prime factorization on $$n = 102$$. First of all, $$102$$ is an even number, hence it is divisible by the smallest prime number, namely $$2$$. Thus, we see that $$102 = 2 \times 51$$. Now, $$51$$ looks like a prime number, but it is actually divisible by $$3$$, which is also a prime. With $$51 = 3 \times 17$$, it follows that $$102 = 2 \times 3 \times 17$$ is the prime factorization, where the numbers in $$\{2,3,17\}$$ are all prime numbers.

For a visualization of this process, refer to the **prime factorization tree** below:

$$
\begin{array}{c}
    102 \\
    / \quad \ \backslash \\
    2 \quad \ 51 \\
    \quad \quad / \quad \backslash \\
    \quad \quad 3 \quad \ 17 \\
\end{array}
$$

## Factors and Multiples

Let us begin with the notion of __multiples__. Let $$n \in \mathbb{Z}$$. We say that the multiples of $$n$$ are of the set $$\{..., -3n, -2n, -n, 0, n, 2n, 3n, ...\} = \{nk : k \in \mathbb{Z}\}$$. For example, in the __times table__ that you are often forced to memorize, you are actually listing the nine positive multiples of the integers from $$2$$ to $$9$$. Let $$a, b \in /mathbb{Z}$$, i.e. $$a$$ and $$b$$ are integers. Formally, we say that $$a$$ is a multiple of $$b$$ if there exists an integer $$k$$ such that $$a = bk$$. See the following examples for better intuition:

* $$10$$ is a multiple of $$10$$ because $$10 = 10 \times 1$$. Clearly, for all integers $$n$$, $$n$$ is a multiple of $$n$$.
* The set of multiples of $$12$$ looks something like $$\{..., -36, -24, -12, 0, 12, 24, 36, 48, 60, ...\}$$. 
* $$51$$ is a multiple of $$3$$ because $$51 = 3 \times 17$$. 
* $$0$$ is a multiple of any integer, because for all integers $$n \in \mathbb{Z}$$, it follows that $$n \times 0 = 0$$.

As you may have noticed, it appears that the notion of divisibility and multiples are closely related. One difference is that $$0$$ does not divide any integer and $$0$$ is a multiple of all integers. Same-same but different.

Notice in the last prime factorization example that we __extracted__ a prime in each level of the prime factorization tree, which resulted in a regular __factor__ that is not necessarily a prime. This brings us to the notion of **factors**, which binds nicely with the notion of divisibility (see above). Let $$a,b \in \mathbb{Z}$, e.g. $$a$$ and $$b$$ are integers. We say that $$a$$ is a factor of $$b$$ if $$a$$ divides $$b$$, meaning that there exists an integer $$k$$ such that $$b = ak$$. Do you see how $$a$$ and $$b$$ swapped their places in the definitions for a multiple and a factor? Take a look at the following examples for better intuition:

* $$\{1,2,4,8,16,32\}$$ is the set of (positive) factors for $$32$$.

* Since $$31$$ is a prime number, it follows that only $$1$$ and $$32$$ are its factors. 

* Because $$1$$ divides any integer, it follows that $$1$$ is a factor for any integer $$n$$, including itself. 

* Things get quite tricky when $$0$$ is concerned. Since $$0$$ times any integer is $$0$$, we could say that any integer is a factor of $$0$$, meaning $$0$$ has infinitely many factors. Thus, in general, the notion of factors is not very applicable for $$0$$ as we often times ask about finitely many factors. 