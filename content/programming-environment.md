---
title: "Programming Environment"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-13T13:27:03+10:00
---

{{< slide class="center" >}}

## Programming Environment

---

## The Terminal

{{% section %}}

---

### What is a terminal?

A terminal is an interface that lets us access the system with just a keyboard. This is how we will _compile_ and _execute_ most of our programs.

|Window Command Prompt|Bash Terminal|
|:-------------------:|:-----------:|
|![](https://featherbear.cc/UNSW-COMP1511/notes/Introduction%20to%20the%20Terminal/Introduction%20to%20the%20Terminal_files/image001.png)|![](Screenshot from 2020-05-13 17-52-26.png)|


{{% /section %}}

---

### Writing C Code

In every programing language, code is just plain text!  
We can use any text editor we want!  

</br>
Integrated Development Environments (IDEs) are text editors designed for programming!  
For example, [Visual Studio Code](https://code.visualstudio.com/) <!-- Sponsor me Microsoft :') -->

---

### Compiling Code

{{% section %}}

To run C code, we first need to **compile** it.  

A compiler is another program that turns our code into something the computer can run.  

![](compiler-flow.png)

For C code, we can use a program called `gcc`

---

### `GCC`

> `gcc <SOURCE> -o <OUTPUT>`  

</br>
For example, if we want to compile our source code called `program.c`...

> `gcc program.c -o myprogram`

{{% /section %}}

---

### Running Code

We can then run our program

> `./myprogram`

---

### Takeaway

* Pick a text editor for editing code
  * I recommend an IDE like [Visual Studio Code](https://code.visualstudio.com/)
* Install the `gcc` compiler
  * Already included in Linux and Mac
* Practise compiling and executing programs

> [Hello World](../hello-world)