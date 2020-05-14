---
title: "Strings"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-14T20:18:04+10:00
---

{{< slide class="center" >}}

## Strings

---

## Strings

A string is a word, formed by combining letters.

H, e, l, l, o &#x27A1;&#xFE0F; Hello

<br/>
Some languages (Python) have a datatype for strings, however not C.  

In C, we define a string as an <u>array of characters</u>.  

> `char var[] = "Hello";`

---

_In C, we define a string as an <u>array of characters</u>._

> `char var[] = "Hello";`

* The `[]` indicates that `var` is an _array_ of type `char`
* The word is wrapped in quotes - not apostrophes

|||
|:-----|:--------------------|
|Letter|`char c = 'H';`      |
|String|`char w[] = "Hello";`|

---

## The Null Character '\0'

Every byte of data is stored in a different memory address. They however are kept in the same region.

```c
int main(void) {
    char string1[] = "Foo";
    char string2[] = "Bar";
    char string3[] = "Buzz";
}
```

{{% section %}}

{{% fragment %}}Our memory should look something like this:</br>`'F'`, `'o'`, `'o'`, `'B'`, `'a'`, `'r'`, `'B'`, `'u'`, `'z'`, `'z'`{{% /fragment %}}

{{% fragment %}}However, we do not have a way of figuring out which memory is for what variable!{{% /fragment %}}

---

To solve this, we append a special symbol which indicates the end of the string.  
This symbol is the <u>NULL character</u>, represented by `\0`

---

> NULL character - `\0`

{{% fragment %}}Our memory looks like this:</br>`'F'`, `'o'`, `'o'`, `'\0'`, `'B'`, `'a'`, `'r'`, `'\0'`, ...{{% /fragment %}}

<!-- Note: It will actually look like B u z z \0 B a r \0 F o o \0 as these values are found on the stack -->

{{% /section %}}

---

{{< slide transition="fade" >}}

## The Null Character '\0'

> `char w[] = "Hi";`

When using a string enclosed in apostrophes, the NULL character is automatically added.<br/><br/>

{{% fragment %}}> `char w[] = {'H','i','\0'}`

If we decide to define our string with characters, we need to make sure to put the NULL character in!{{% /fragment %}}

---


## Review

{{% section %}}

Is the expression `"H"` valid?

---

Is the expression `"Hello"` valid?

---

Is the expression `'Hello'` valid?

---

Is the expression `''` valid?

---

Is the expression `""` valid?

---

What is the equivalent definition of the following  
`char word[] = "Computer";`?

<br/>

```c
char word[] = { ??? };
```

{{% /section %}}

---

## Inspecting Strings

We can extract a single character from a string  
by using its positional <u>index</u>. We count indices from $0$.

<br/>
`char word[] = "Computer";`

{{% fragment %}}<br/>word[0] is 'C'<br/>word[1] is 'o'<br/>...<br/>word[7] is 'r'{{% /fragment %}}  
{{% fragment %}}word[8] is '\0'{{% /fragment %}}

---

## Mutating Strings

Like changing variables, we can change characters in strings with the assignment operator `'='`

```c
#include <stdio.h>

int main(void) {
    char word[] = "Fire";
    printf("Current word is %s.\n", word);

    word[2] = 'l';
    word[3] = 'l';
    printf("New word is %s.\n", word);

    return 0;
}
```

```bash
$> ./program
Current word is Fire.
New word is Fill.
```

<!-- 
## String Functions

The C library provides basic string functions

Comparing strings -->