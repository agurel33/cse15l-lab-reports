# Week 4 Lab Report

## Introduction

* text

## Table of Contents

1. Code Change #1: Allowing for text after the links
2. Code Change #2: Not including images
3. Code Change #3: Allowing for no links in file

## Code Change #1: Allowing for text after the links

![Image](images/week4_github1.PNG)

[Failure-Inducing Input](https://raw.githubusercontent.com/agurel33/markdown-parse/main/test-file2.md)

```
$ javac MarkdownParse.java
$ java MarkdownParse text-file2.md
Value of currentIndex at the beginning of the loop: 0
Value of currentIndex at end of loop: 28
Value of currentIndex at the beginning of the loop: 28
Value of currentIndex at end of loop: 28
Value of currentIndex at the beginning of the loop: 28
Value of currentIndex at end of loop: 28
Value of currentIndex at the beginning of the loop: 28
Value of currentIndex at end of loop: 28
Value of currentIndex at the beginning of the loop: 28
Value of currentIndex at end of loop: 28
Value of currentIndex at the beginning of the loop: 28
Value of currentIndex at end of loop: 28
Value of currentIndex at the beginning of the loop: 28
Value of currentIndex at end of loop: 28
... (infinite loop)
```

* Before this change, whenever a file didn't end with a link or had text after the last link, the code would run into an infinite loop. The bug would be that the getLinks() method would not accept strings that did not have links at the end of them. The failure-inducing input would be any input of a file that had some text or empty spaces after any given links in the file. The symptom of this failure-inducing input and bug is an infinite loop and no output given.

## Code Change #2: Not including images

* text

## Code Change #3: Allowing for no links in file

* text