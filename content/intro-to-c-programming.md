---
title: "Introduction to Programming"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-13T13:09:50+10:00

reveal_hugo:
    center: true
---


## Introduction to Programming

---

## What is Programming?

{{% section %}}
The design and development of software programs

---

A **programming language** is a formal language which follows a set of rules (syntax) to describe the behaviour of the program.  

{{% fragment %}}_Common languages you may have heard of are:</br>Python, JavaScript, C, C#, C++, .NET_</br></br>We will be learning C in this course!{{% /fragment %}}

{{% /section %}}

---

## What is C

C is a general-purpose programming language used to write software.  

{{% fragment %}}
It is used very commonly!</br>
In fact all the major operating systems (Windows, Mac, and Linux) are written in C!
{{% /fragment %}}

---

## What can C offer?

```c
#include <stdio.h>

int main(void) {
    int number = 5;                 // C offers variables!
    number = 5 * 2;                 // C offers maths!

    if (number == 10) {             // C offers conditions!
        printf("5 x 2 is 10");      // C offers output!
    } else {
        printf("5 x 2 is not 10!");
    }

    return 0;
}
```

And lots more!

---

## C Code Files

Source code files for programs written in C usually have a `.c` file extension.  
Ultimately, all source code files are just text documents that can be edited with any text editor.

## Next Steps

> [Hello World](../hello-world)
