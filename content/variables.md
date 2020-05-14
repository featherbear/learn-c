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

