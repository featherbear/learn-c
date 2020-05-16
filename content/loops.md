---
title: "Loops"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-15T01:21:42+10:00
---

{{< slide class="center" >}}

## Loops

---

## Loops

Loops allow us to repeat parts of code several times.  

They are very powerful when used with variables, as they can do different things depending on the variable.

---

## The While Loop

> `while (COND) { ... }`

The `while` loop will repeat its code block for as long as given condition is true.

{{% section %}}

{{% fragment %}}```c
int number = 3;
while (number > 0) {
    printf("%d\n", number);
    number = number - 1;
}
printf("Blast Off!");
```

```
3
2
1
Blast Off!
```

{{% /fragment %}}

---

Every time the loop begins, the `COND` is evaluated.  

If it is true - the loop will run.  
Otherwise the program will go to the next code block.

---

```
int limit = 5;
int number = 6;

printf("Starting at %d\n", number);

while (number < limit) {                // this
    printf("Counted to %d\n", number);  // code
    number = number + 1;                // won't
}                                       // run

printf("Finished at %d\n", number);
```

{{% /section %}}

---

## The For Loop

> `for (INIT;COND;STEP) {...}`

{{% section %}}
When using the `while` loop, we had to separately define a variable, a condition and step instruction.

```c
int number = 3;             // INIT variable
while (number > 0) {        // COND check
    printf("%d\n", number);
    number = number - 1;    // STEP instruction
}
printf("Blast Off!");
```

---

With a `for` loop, we can combine everything together!

```c
for (int number = 3; number > 0; number = number - 1) {
//   ^ INIT          ^ COND      ^ STEP
    printf("%d\n", number);
}
printf("Blast Off!");
```

```
3
2
1
Blast Off!
```
{{% /section %}}

---

Write a program to print out the numbers 1-26, and their corresponding letters in the alphabet.

{{% section %}}

```c
#include <stdio.h>

int main(void) {
    
    // WRITE YOUR CODE HERE

    return 0;
}
```

---

```c
#include <stdio.h>

int main(void) {
    int i = 1;
    char c = 'A';

    while (i <= 26) {              // i = 1..26
        printf("%d - %c\n", i, c); // e.g "1 - A"
        i++;                       // Shorthand for i = i + 1
        c++;                       // Shorthand for c = c + 1
    }

    return 0;
}
```

{{% /section %}}

---

When using `for` loops, we can also initialise multiple values, and perform several step instructions.

Note: All the variables must be the same data type!

```c
#include <stdio.h>

int main(void) {
    for (int a = 1, b = 2; a < 5; a++, b += 2) {
        //                             ^ short for b = b + 2
        printf("%d", b);
    }

    return 0;
}
```

{{% fragment %}}How many times does this loop run?{{% /fragment %}}{{% fragment %}}A: Four times{{% /fragment %}}

{{% fragment %}}What does the program output?{{% /fragment %}}{{% fragment %}}2 4 6 8{{% /fragment %}}
