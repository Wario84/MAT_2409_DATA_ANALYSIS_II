---

layout: post
title: "Tutorial 1: R, syntaxys, atomic elements and console."
author: "Mario H. Gonzalez-Sauri"
date: "2022-02-22"

---

# Introduction

The purpose of this tutorials to to teach you Data Science using the
**R-language** in the simplest way to encourage new users. Learning Data
Science goes hand in hand with gaining skills with a computer
programming language. As, it was cover in the first lecture, **R** is a
free open source language

I have identified, through my experience of teaching R, six main
building blocks of the language. We will cover this blocks in the
following way:

-   Week 1: Learn **R** and its integration with **R-studio**, the
    operators, the atomic element and basic operations in the console.
-   Week 2: Learn basic `object` creation and manipulation: `vectors`,
    `matrices`, `dataframes`, `arrays`, `lists`.
-   Week 3: How to read/save data from **R**, and how to perform
    descriptive statistics and linear regression.
-   Week 4: Basic Data Visualization Using **R**.  
-   Week 5: Basic Algorithms 1: Use of `functions`, `loops`, `while`,
    `if`, `else` statements.
-   Week 6 onward, we will deploy our skill running Machine
    Learning (ML) algorithms and String Analysis.

***

# Instroctutions for the the tutorials.

 The exercises are simple, design to develop intuition, confidence to step the learning curve!

<figure>
<img src="https://www.valamis.com/documents/10197/520324/steep-lc.png" height="300" alt="Learning Curve" /><figcaption aria-hidden="true">Learning Curve</figcaption>
</figure>

*Source: [Valamis, 2020](https://www.valamis.com/)*

1. Each weak, you will take look in [this](https://wario84.github.io/idsc_mgs/) repository and read the corresponding tutorial exercise for each week.
2. Here in this website, I am posting the instructions and the solutions to all the exercises.
3. Your task is to perform all the excercises of each tutorial in an `Rscrip`.
4. 

***
# 1. The operators

The operators are **special characters** that perform an **action** with
a specific result. The most common arithmetic operators to get some
familiarity. This operators are not only common for `R` but you may know
them from spread sheets, calculators or other languages.

CRAN has an exhaustive list of operators that you can retrieve
[here](https://cran.r-project.org/doc/manuals/r-release/R-lang.html#Operators)

<center>
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;border-style:solid;border-width:1px;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:0px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:0px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
<tr>
<th class="tg-c3ow">
</th>
<th class="tg-7btt">
List of Operators
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">-</span>
</td>
<td class="tg-c3ow">
Minus.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">+</span>
</td>
<td class="tg-c3ow">
Plus.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">:</span>
</td>
<td class="tg-c3ow">
Sequence.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">\</span>
</td>
<td class="tg-c3ow">
Multiplication.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">/</span>
</td>
<td class="tg-c3ow">
Division.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">^</span>
</td>
<td class="tg-c3ow">
Exponentiation.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">%%</span>
</td>
<td class="tg-c3ow">
Modulus.
</td>
</tr>
</tbody>
</table>
</center>

# 2. Atomic elements.

The atomic elements are the most fundamental building blocks of the
**R** language. They are the most essential input of the language, here
are the main types:

<center>
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;border-style:solid;border-width:1px;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:0px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:0px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg">
<thead>
<tr>
<th class="tg-c3ow">
</th>
<th class="tg-7btt">
Atomic Element
</th>
</tr>
</thead>
<tbody>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">1L, 2L, â¦, 10</span>
</td>
<td class="tg-c3ow">
Integer.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">1.1, 4.5, 3.2</span><br>
</td>
<td class="tg-c3ow">
Numeric.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">âaâ, âBDâ,
âfâ</span>
</td>
<td class="tg-c3ow">
Character.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">TRUE, FALSE</span><br>
</td>
<td class="tg-c3ow">
Logical.
</td>
</tr>
<tr>
<td class="tg-c3ow">
<span style="color:#905;background-color:#DDD">NA</span><br>
</td>
<td class="tg-c3ow">
Not Available / Missing Values.
</td>
</tr>
</tbody>
</table>
</center>
<!--  More generally, they help us to manipulate variables, evaluate statements, construct functions and perform any sort of operation. -->

# 3. Lines and chunks of code.

Now we can use **operators + atomic elements** to write lines of code.
**R** runs this lines of code following these two rules:

1.  Similar to math, lines are read and evaluated from *left* to
    *right*.
2.  Similar to a book, lines are read and evaluated from *top* to
    *button*.

Lines of code are the use to perform analysis, evaluate statements and
any sort of operation that you can imagine. Different from independent
lines of code, a group of two or more lines used for a particular
operation is called a **chunk** of code. But, before we get into them,
practice your knowledge of operators and atomic elements to perform
basic arithmetic operations.

## Exercise 1: Use R as a calculator.

Instruction: Solve this exercises by writing the correct atomic elements
and operators to perform each arithmetic operation. These exercise can
only evaluate a unique answer for each line.

### Writting tips

1.  Use the **most simple** combination of atomic elements and
    operators. For instance, if asked to perform `2 plus 3`, avoid using
    more atomic elements and operators typing `2 + 1 + 1 + 1`. The best
    answer is not only correct but also the simplest. Example: `2 + 3`.
2.  Leave a **space** or white space in between each operator and atomic
    element. For instance, write `2 + 3` but not `2+3`. An exception to
    this rule is to write powers, which `3^3` is preferred but not

<!-- -->

1.  Addition: 2 plus 3.

``` r
 2 + 3
```

    [1] 5

2.  Subtraction: 5 minus 4.

<!-- -->

    [1] 1

3.  Multiplication: 3 times 5.

<!-- -->

    [1] 15

3.  Division: 10 divided by 2.

<!-- -->

    [1] 5

4.  Exponentiation: 4 to the power of 3.

<!-- -->

    [1] 64

5.  Module: 5 module 2

<!-- -->

    [1] 1

# Other resources

If you want to increase your knowledge of **R** and accelerate your
learning check out:

-   The excellent [Introduction to R from
    Datacamp](https://www.datacamp.com/courses/free-introduction-to-r).
-   The Comprehensive R Archive Network (CRAN) also has a more
    comprehensive
    [manual](https://cran.r-project.org/doc/manuals/r-release/R-intro.pdf).
-   Watch for free the videos of the [Advance Your Skills as an R
    Expert, from
    Linkedin](https://www.linkedin.com/learning/paths/advance-your-skills-as-an-r-expert)
