---
title: '#1 Kotlin: How to measure code execution time for benchmarking'
date: 2022-09-20 08:00:00 +0530
categories: [Kotlin]
tags: [kotlin, benchmark, time]
math: true
mermaid: true
---
<!-- https://www.baeldung.com/kotlin/measure-elapsed-time -->
## Overview
Kotlin is a great language for creating high-performance applications. There might be a time when you want to measure how long it takes for a particular operation to execute. Kotlin has a built-in way to measure elapsed time. In this article, we'll show you how to measure elapsed time in Kotlin, so you can benchmark your code and optimize your application's performance.

## What is benchmarking?

Benchmarking is the process of measuring the performance of a software program or system. As your business needs change, there will be times when you need your code to execute more quickly. The main goal of benchmarking is to identify the bottlenecks, determine how quickly your code runs and optimize the code. In Kotlin, benchmarking can be used to measure the elapsed time for a particular task.

## How to measure elapsed time in Kotlin

To measure elapsed time in Kotlin, we'll use the measureTimeMillis function from the kotlin.time package. This function takes a lambda expression as an argument, and returns the time in milliseconds that it took to execute the lambda expression. For example, let's say we have a simple function that squares a number:

fun square(x: Int): Int {
return x * x
}
 We can measure how long it takes to execute this function by wrapping it in a call to measureTimeMillis :

val squareTime = measureTimeMillis {
square(10)
}
 The squareTime variable will now contain the number of milliseconds it took to execute the square function. We can use this information to benchmark our code and optimize its performance.
 
So there you have it - measuring elapsed time in Kotlin is easy with the measureTimeMillis function. Use it to benchmark your code and make your Kotlin applications run even faster!

## When to use benchmarking

As a Kotlin developer, you may find yourself in a situation where you need to benchmark your code in order to determine its performance, identify the bottlenecks, determine how quickly your code runs, optimize and execute it more quickly. In such situations you can use benchmarking to measure code execution time & fix it according to your need. You can use benchmarking in multiple places in your code. Kotlin provides a range of built in functions for this purpose and you can use appropriate functin as per your need.

## Conclusion

Kotlin provides a range of functions for measuring elapsed time, which can be useful for benchmarking purposes. In this article, we've looked at how to use the measureNanoTime and measureTimeMillis functions from Kotlin standard library to measure elapsed time in Kotlin. We've also seen how to use the TimeUnit class to format the results of our measurements. I hope this article helps you to understand some of the options available in Kotlin to measure the code execution time. So what are you going to use from these available options to benchmark your code and measure execution time, Let me know in the comments section.

Thank you for reading this article ❤️ Hope you like this short and on-point article. I would love to hear your feedback, so leave a comment below. Please share the article with others If this article helps you. If I got something wrong, leave a response and let me know in the comments section. I would love to improve. Keep learning, Keep growing 🙂 See you in another article. Bye!