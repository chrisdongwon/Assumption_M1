---
layout: post
title:  "Rational Numbers"
date:   2024-07-02 00:00:00 +0000
categories: lecture notes
katex: True
---

## Preview of Algebra: Variables

Let us recall that a variable is simply a representation of any number. To be more precise, variables are arbitrary members of a specific mathematical _set_. As an example, I can say that $$x$$ is a number from the sets of fractions excluding the integers. Notice that with this restriction, $$x$$ can't really be _any_ number. Traditionally, $$x$$ is the designated letter/symbol for a variable. When other variables need to be referenced, other letters can be used as well. However, let us remember that same instance of the variables refer to the same value. As an example, the expression $$x \cdot x$$ refers to multiplication where the left $$x$$ and the right $$x$$ refer to the same value designated for $$x$$.  

In summary, a variable is an arbitrary number, but we need to be careful about the _set_ of numbers that $$x$$ is originating from. 

## Rational Numbers

Now, we have enough background to really _define_ what we mean by fractions. Mathematicians refer to fractions as the _rational numbers_, hence both the terms will be used interchangeably.

 * Rational number: a number of the form $$\frac{n}{d}$$, where  
    1. $$n$$ and $$d$$ are integers  
    2. $$d$$ is not zero (For the reasons detailed in the above section)
    3. all common primes of $$n$$ and $$d$$ in their prime factorizations have been cancelled out. In other words, the fraction is in its _simplest form_.  

As you may have guessed, $$n$$ stands for the numerator, the top number, and $$d$$ stands for denominator, 

If these conditions are not satisfied, then we are looking at a number that appears to be a fraction but it really is not a fraction, mathematically speaking. We refer to the set of rational numbers with the symbol $$\mathbb{Q}$$. Why Q? Please let me know if you figure this out. 

Lastly, we can easily see that all integers are rational numbers: simply set the denominator to be 1. 

## Rational Number Equality & Inequality

* When are two fractions equal? There are two schools of thoughts that are equivalent:
    1. When $$a = c$$ and $$b = d$$ (The numerators and the denominators are the same)
    2. When $$ad = bc$$ ("Cross-multiplication" technique).

To see why the second assertion is true, consider the following. Let's say we want to compare $$\frac{a}{b}$$ and $$\frac{c}{d}$$. In order to compare in fractions, we need to have a common denominator - intuitively speaking, it is because we are counting how many parts when each part is equally _cut_ - and the size of this _cut_ is precisely what we refer to as the denominator (or simply, the divisor). So, it appears that a common multiple of $$b$$ and $$d$$ is simply $$bd$$, and it follows that $$\frac{a}{b} = \frac{a}{b} \cdot 1 = \frac{a}{b} \cdot \frac{d}{d} = \frac{ad}{bd}$$, and similarly, $$\frac{c}{d} = 1 \cdot \frac{c}{d}= \frac{b}{b} \cdot \frac{c}{d} = \frac{bc}{bd}$$. Now can we can use the first reasoning to see how the fractions compare. 

* Provided that the fractions in comparison are both positive, how do we see which fraction is greater? There are a few techniques to facilitate this:
  1. If the denominators are the same, simply compare the numerators (E.g. How many slices of pie did I eat vs. did you eat?)  
  2. If the numerators are the same, then compare the denominators (E.g. Is a slice of a whole pizza cut in half bigger than a slice of a whole pizza sliced up in 20 equally sized slices?) Notice that greater the denominator, smaller the quantity.  
  3. Algebraically, $$\frac{a}{b} < \frac{c}{d}$$ if $$ad < bc$$, provided that the fractions in comparison are both positive to begin with.
  
## Addition and Multiplication in Rational Numbers

* Adding/subtracting Fractions: Recall that addition and subtraction in fraction only makes sense when we have a common denominator. Thus, the proposed formula gives us _any_ sum and differences of two fractions: $$\frac{a}{b} \pm \frac{c}{d} = \frac{ad \pm bc}{bd}$$. 

* Multiplying/dividing Fractions: Luckily, multiplication and division are more natural operations to perform on fractions. Similarly, we state that $$\frac{a}{b} \cdot \frac{c}{d} = \frac{ac}{bd}$$ and $$\frac{a}{b} \div \frac{c}{d} = \frac{a}{b} \cdot \frac{d}{c} = \frac{ad}{bc}$$.

## Exponentiation (a.k.a. Powers)

Lastly, let us recall the notion of _exponents_ (also known as _powers_). In order to understand what we mean by exponents, let us make a simple analogy:  

**If multiplication is repeated addition, then exponentiation is repeated multiplication.**  

What do we mean by this? For an example, $$x + x = 2x$$ and $$x \cdot x = x^2$$. Hence, we can state the following for the exponentiation of fractions: $$(\frac{a}{b})^2 = (\frac{a}{b})(\frac{a}{b}) = \frac{a \cdot a}{b \cdot b} = \frac{a^2}{b^2}$$. In a more general sense, we see that for any positive integer $$n$$, $$(\frac{a}{b})^n = \frac{a^n}{b^n}$$.

What happens when the exponent is zero? Let us make another analogy here - when we add 0 to any number, we get the number back - in thise sense, we referred to 0 as the additive identity. It appears that when we add _zero times_, the sum intuitively should be 0. In a similar sense, when we multiply 1 to any number, we get the number back - in this sense, we refer to 1 as the multiplicative identity. It appears that when we multiply _zero times_ (careful: not to zero, but zero times), the product intuitively then should be - you guessed it - the multiplicative identity, 1. Hence, when any nonzero number is exponentiated to the zero power, the computation yields 1, as in $$(\frac{a}{b})^0 = 1$$, provided $$a \not = 0$$. What about negative exponents? More on this on the following section.