---
title: "Variables"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-13T13:49:15+10:00
---

{{< slide class="center" >}}

## Variables

---

## Variables

Variables are containers that hold data.  
_This data could be a number, name, etc..._

<br/>

In some languages variables can hold any type of data, then be replaced with a different type.  

However the C language is 'statically typed', meaning that each variable accept only a <u>specific</u> type of data.

---

## Basic Data Types

|Type|Description|Example|
|:--:|:----------|:------|
|`int`|Integer|the number `16`|
|`float`|Float|the decimal number `14.25`|
|`char`|Character|the single letter 'A'|
|`bool`|Boolean|`true` / `false`|

{{% fragment %}}
<u>What about strings?</u>  

There is no data type for a string.  
Rather, it is an array of `char`s
{{% /fragment %}}

---

## Declaring a Variable

To declare a variable, we follow the syntax

> `<type> <variable_name>;`

<br/>

How would you declare a variable called `mynumber` with the `int`eger type?

{{% section %}}

---

`int mynumber;`
{{% /section %}}

---

## Assigning a Variable

To set a variable to a particular value, we use the assignment operator '`=`'

> `<variable_name> = <value>;`

<br/>
How would you declare a variable `mynumber` with the `int` type, and then assign it the number `30`?
{{% section %}}

---

`int mynumber;`  
`mynumber = 30;`
{{% /section %}}

---

## Shortcut

Declaring variables and immediately assigning a value to them is a very common practice.  

The C language allows us to declare and assign a variable in one line!

> `int mynumber = 30;`

---

## Variable Naming

You can name your variable anything you want,  
as long as it follows the rules

* Only has the characters `A`-`Z`, `A-Z`, `0-9` and `_`
* Does not _start_ with a number
* Is not a keyword (Reserved names)

{{% section %}}

&nbsp;  

|my_var|2my_var|_3my_var|myv4r|my var5|
|:---:|:----:|:----:|:----:|:----:|
|<span style="color: lightgreen;font-size: 1.5em;">&#x2714;&#xFE0F;</span>|&#x274C;|<span style="color: lightgreen;font-size: 1.5em;">&#x2714;&#xFE0F;</span>|<span style="color: lightgreen;font-size: 1.5em;">&#x2714;&#xFE0F;</span>|&#x274C;|

---

Note: Variables are case-sensitive.

`my_var` is different to `My_var`

{{% /section %}}

---

> `int | float | char | bool`

{{% section %}}
How would you define a variable for the age of someone who is `15`?  

{{% fragment %}}<br/>`int age = 15;`{{% /fragment %}}

---

How would you define a variable to contain the temperature `19.35`°C?  

{{% fragment %}}<br/>`float temperature = 19.35;`{{% /fragment %}}

---

How would you define a variable to be `false`?  

{{% fragment %}}<br/>`bool result = false;`{{% /fragment %}}

---

How would you define a variable for the letter `H`?  

{{% fragment %}}<br/>`char letter = 'H';`<br/><br/>Note: You need to wrap the letter with apostrophes{{% /fragment %}}

---

How would you define a variable for the word `Hello`?  

{{% fragment %}}<br/><s>`char word = 'Hello';`</s><br/><s>`char word = "Hello";`</s><br/><s>`string word = "Hello";`</s><br/><br/>`char word[] = "Hello";`</s>{{% /fragment %}}

{{% /section  %}}

---

{{< slide class="center" >}}

## Next Steps

> [Strings](../strings)