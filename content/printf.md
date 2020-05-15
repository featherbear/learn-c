---
title: "printf"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-13T13:48:15+10:00
---

{{< slide class="center" >}}

## The `printf` Function

---

## The `printf` Function

It is very useful for programs to display an output!  
We can use the `printf` function to do this!

---

## The `printf` Function

> `printf(FMT,arg1,arg2,...);`

{{% section %}}

* `FMT` - Format string
  * Tells the function what to do with its arguments
* arg[n] - Displayed, depending on the format string

---

The format string (FMT) instructs the function on how to display the information.  

For example, `printf("Hello")` will display Hello.

---

To show numbers, we can use the `%d` format specifier.

`printf("A day has %d hours", 24);`  

```c
$> ./program
A day has 24 hours
```

---

To show single letters, we can use the `%c` format specifier.

`printf("Dog starts with a %c", 'd');`  

```c
$> ./program
Dog starts with a d
```

---

To print out a `'%'`, we put `%%` in the format specifier.  

`printf("The percentage sign is %%.");`  

```c
$> ./program
The percentage sign is %.
```

---

There are many other format specifiers!

| | |
|:---:|:---|
|`%f`|Floating Point Number|
|`%s`|String|
|`%x`|Hexadecimal Number|
|`%p`|Point|
||etc...|

{{% /section %}}

---

## The New Line Character `\n`

{{% section %}}

If we run the following program.

```c
#include <stdio.h>

int main(void){
    printf("Hello");
    printf("How are you?");
    return 0;
}
```

We will see this

```c
HelloHow are you?
```

&nbsp;  
This is because printf does not start on a new line!

---

{{< slide transition="fade" >}}

To show each sentence separately, we need to put a new line character - represented by `\n`.

```c
#include <stdio.h>

int main(void){
    printf("Hello\n");
    printf("How are you?\n");
    return 0;
}
```

We will now see

```c
Hello
How are you?
```

{{% /section %}}

---

## Try It

Write a program to print "My name is ...", followed by your name. Use an appropriate format specifier.

```c
#include <stdio.h>

int main(void) {

    // WRITE YOUR CODE HERE

    return 0;
}
```

---

## Try It

Write a program to print out a bird

```
  __
<(o )___
 ( ._> /
  `---'
```
