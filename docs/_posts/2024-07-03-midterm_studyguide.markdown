---
layout: post
title:  "Midterm Exam Study Guide"
date:   2024-07-02 00:00:00 +0000
categories: announcement
katex: True
---

Answer the following as a review for your upcoming midterm exam. Make sure to show as much work as possible in order to maximize your points on the exam - any unsupported answers will warrant partial credit.

1. Let $$n \in \mathbb{N}$$ (i.e. $$n$$ is an element of the set of natural numbers, hence $$n$$ is any positive whole number starting with $$0$$). What does it mean for $$n$$ to be a prime? What does it mean for $$n$$ to be a composite? What if $$n = 0$$? What if $$n = 1$$? Hint: do you remember the **definition** of prime numbers and composite numbers? Sometimes, a number is neither prime nor composite.

    * Solution: We say that $$n \in \mathbb{N}$$ is a prime number if it is greater than $$1$$ and the only divisors are $$1$$ and $$n$$. If $$n$$ is greater than $$1$$ ($$3$$ is also fine, since the smallest composite natural number begins with $$4$$) that is not a prime is called a composite number. Both $$0$$ and $$1$$ are **neither** prime nor composite. For a detailed explanation, please refer to the article about this topic.

1. What is the prime factorization of $$76$$? Show your work by constructing a prime factorization tree. Then, list the first 4 positive multiples and all positive factors of $$76$$. 

    * Solution: The prime factorization of $$76$$ is $$2 \times 2 \times 19 = 2^2 \times 19$$ (as long as all the primes are present, the answer is considered correct regardless of order and the usage of the exponential notation). One possible tree might look something like:

$$
\begin{array}{c}
    76 \\
    / \quad \ \backslash \\
    2 \quad \ 38 \\
    \quad \quad / \quad \backslash \\
    \quad \quad 2 \quad \ 19 \\
\end{array}
$$

1. What is the condition for fraction addition/subtraction? Compute $$\frac{2}{3} + \frac{5}{7}$$. Hint: you need a common ...

    * Solution: Addition on a pair of rational numbers is well-defined if and only if the rational numbers have a **common denominator**. There is a _formula_ that you may use to facilitate the addition/subtraction as indicated in the article: $$\frac{2}{3} + \frac{5}{7} = \frac{2 \times 7 + 3 \times 5}{3 \times 7} = \frac{14 + 15}{21} = \frac{29}{21}$$. Improper fractions are acceptable as answers as long as the question does not specify that your answer must be in a mixed-number representation.

1. How do you divide by a fraction? Compute $$\frac{2}{3} \div \frac{5}{7}$$. Hint: division is multiplication by ...

    * Solution: **REMEMBER that the operation of division is defined as multiplication by the reciprocal**. Reciprocal of $$\frac{5}{7}$$ is $$\frac{7}{5}$$ (Reciprocal of a nonzero whole number $$n$$ simply $$\frac{1}{n}$$, and the reciprocal of a nonzero rational number $$\frac{a}{b}$$ is $$\frac{b}{a}$$). It then follows that $$\frac{2}{3} \div \frac{5}{7} = \frac{2}{3} \times \frac{7}{5} = \frac{14}{15}$$.

1. How do you interpret $$1 \frac{2}{3}$$? Is it the same as $$1 + \frac{2}{3}$$ or $$1 \times \frac{2}{3}$$? Explain.

    * Solution: Mixed-number representation is often times confusing and I _prefer_ not to use them in computation of rational numbers. This is because, generally in mathematics, numbers written next to each other will indicate that the performed operation is multiplication, as you will start to see in Algebra. However, in mixed-number representation, the whole number and the fractional parts are actually **being added**. Thus, $$1 \frac{2}{3}$$ should be interpreted as $$1 + \frac{2}{3}$$, and the equivalent representation using improper fraction is $$1 + \frac{2}{3} = \frac{3}{3} + \frac{2}{3} = \frac{5}{3}$$.

1. What are the least common multiple (LCM) and greatest common divisors (GCD) of $$12$$ and $$20$$?

    * Solution: Let us list the (positive) common multiples and the common divisors of $$12$$ and $$20$$.

    * Multiples of 12: $$\{12, 24, 36, 48, 60, 72, ...\}$$
    * Multiples of 20: $$\{20, 40, 60, 80, 100, 120, ...\}$$
  
    Hence, it appears that $$60$$ is the least common multiple.

    * Divisors of 12: $$\{1,2,3,4,6,12\}$$
    * Divisors of 20: $$\{1,2,4,5,10,20\}$$
  
    Hence, it appears that $$4$$ is the greatest common divisor.