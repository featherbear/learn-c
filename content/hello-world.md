---
title: "Hello, World!"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-13T13:27:03+10:00
---

{{< slide class="center" >}}

## Hello World!

```c
#include <stdio.h>

int main(void) {
    printf("Hello, world!\n");

    return 0;
}
```

{{% section %}}

---

{{< slide transition="fade" >}}

|Code|Explanation|
|:---:|:---:|
|`#include <stdio.h>`|Load the I/O library|

---

{{< slide transition="fade" >}}

|Code|Explanation|
|:---:|:---:|
|`int main(void) { ... }`|Code entry-point|

---

{{< slide transition="fade" >}}

|Code|Explanation|
|:---:|:---:|
|`printf("Hello, world!\n");`|Displays the line "Hello, world!"|

---

{{< slide transition="fade" >}}

|Code|Explanation|
|:---:|:---:|
|`return 0;`|Return from the function</br>(with a value of 0)|

{{% /section %}}

---

{{< slide transition="fade" >}}

## Syntax We See


```c
#include <stdio.h>

int main(void) {
    printf("Hello, world!\n");

    return 0;
}
```

|Type|Example|
|:---|:------|
|Entry-point|`int main { ... }`|
|Strings|`"Hello, world!\n"`|
|Functions|`printf(...)`|
|Semicolons|`;`|

---

# Hello, &lt;YOU&gt;

> **EXERCISE**  
Write a C program to print out "Hello", followed by your name.

{{% section %}}

---

Wait, how do I write the code?

{{% fragment %}}Read: <u>[Setting up your Programming Environment](../programming-environment)</u>{{% /fragment %}}

{{% /section %}}

---

{{< slide transition="fade" >}}

> Write a C program to print out "Hello", followed by your name.

#### Step One

Open a code editor

---

{{< slide transition="fade" >}}

> Write a C program to print out "Hello", followed by your name.

#### Step Two

Load the C library for input and output.  

{{% fragment %}}```c
#include <stdio.h>
```
{{% /fragment %}}

---

{{< slide transition="fade" >}}

> Write a C program to print out "Hello", followed by your name.

#### Step Three

Create the entry-point code

{{% fragment %}}```c
#include <stdio.h>

int main(void) {
    return 0;
};
```
{{% /fragment %}}

---

{{< slide transition="fade" >}}

> Write a C program to print out "Hello", followed by your name.

#### Step Four

Write a string that says "Hello", and your name.  

Hint: Use `printf()`  
Don't forget your semicolons!

{{% fragment %}}```c
#include <stdio.h>

int main(void) {
    printf("Hello, Andrew!");

    return 0;
}
```
{{% /fragment %}}

---

{{< slide transition="fade" >}}

> Write a C program to print out "Hello", followed by your name.

#### Step Five

Save the source code file.  

Name it whatever you like, but end it with `.c`  

_e.g. `hello.c`_

---

{{< slide transition="fade" >}}

> Write a C program to print out "Hello", followed by your name.

#### Step Six

Compile the file.  

In a _terminal_, navigate to the file and compile it.

_e.g. `gcc hello.c -o hello`_

---

{{< slide transition="fade" >}}

> Write a C program to print out "Hello", followed by your name.

#### Step Seven

Execute the file!  

```bash
$> ./hello

Hello, Andrew!
```

---

## Next Steps

You've written your first program!  
But this program can't do that much...

> [Variables](../variables)
