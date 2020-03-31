POL 345 Precept Week 8: If statement
================
Jing Qian
2020/03/31

Welcome! This document contains materials that would be helpful for week 8 of POL 345. Specifically, we will cover two important control structures in programming: *for loop* and *if statement*, as well as the *K-Means* algorithm.

In this document, we will focus on the *if statement*.

### 2. If statement[1]

#### 2.1 Basic Idea of if statement

A lot of times, we want to apply different operations to different objects, depending on the value of the object. For example, when we calculate the absolute value of a number, we keep the original value for non-negative values, but not for negative numbers. In such cases, we can use the *if statement* to automatically decide which operation to execute, depending on the *test* pre-defined by the programmer. The basic syntax of *if statement* is as the following:

``` r
if (test_expression){
  statement
}
```

In the chunk above:

-   `test_expression` is a the *test* that you want to conduct, which should return a value of either `TRUE` or `FALSE`.
-   `statement` is the block of code to be executed, **only when `test_expression` returns `TRUE`**.

Below is an example of a basic if statement:

``` r
#Determine if a number is positive
x = 5
if (x > 0){
  print("Positive number")
}
```

    ## [1] "Positive number"

As you can see, in the example above, `test_expression` compares the value in object `x` with 0, and returns `TRUE` if `x` is positive, and `FALSE` otherwise. Since `x` equals 5, which is positive, the `test_expression` returns `TRUE`, and the code `print("Positive number")` get executed.

Alternatively, if `x` is non-positive, the code `print("Positive number")` will simply be ignored since the `text_expression` returns `FALSE`, as in the example below:

``` r
x = -5 #x is now negative
if (x > 0){
  print("Positive number")
}
```

The basic structure of the if statement can be illustrated in the following figure: <img src="images/r-if-statement.jpg" width="30%" style="display: block; margin: auto;" />

[1] Some materials from <https://www.datamentor.io/r-programming/if-else-statement/>
