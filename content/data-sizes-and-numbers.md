---
title: "Data Sizes and Numbers"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-14T20:20:40+10:00
---

## Data Sizes

Computers store data digitally in binary bits  
(1s and 0s)

As computers do not have unlimited memory,  
there is a limit on how big a data type can be.

---

## Data Sizes

|Type|Size|
|:---|:--:|
|char|1 byte|
|short|2 bytes|
|unsigned short|2 bytes|
|int|4 bytes|
|unsigned int|4 bytes|

> 1 byte = 8 bits

---

## How Big?

{{% section %}}

How many numbers can you make with 8 bits?  
{{% fragment %}}You can make $ 2^8 = 256 $ numbers with 8 bits{{% /fragment %}}

{{% fragment %}}How many numbers can you make with 16 bits?{{% /fragment %}}  
{{% fragment %}}You can make $ 2^{16} = 65536 $ numbers with 16 bits{{% /fragment %}}

{{% fragment %}}With 32 bits? $ 2^{32} = 4294967296 ${{% /fragment %}}

---

|$2^8$|$2^{16}$|$2^{32}$|
|:---:|:------:|:------:|
|$256$|$65536$|$4294967296$|

<br/>

A `char` is 1 byte long - it can hold 256 values.  

A `short` is 2 bytes long - it can hold 65536 values.  

An `int` is 4 bytes long - it can hold 4294967296 values.  

{{% /section %}}

---

## Signed Numbers

{{% section %}}

_"A `short` is 2 bytes long - it can hold 65536 values"_

<u>Signed variables</u> allow for negative values to be stored.  
As we have limited space, the maximum positive number is decreased.

a `signed short` has the range $-32768$ to $32767$  

> Signed Range: $-2^{n-1}$  to  $2^{n-1}-1$

---

> Range: $-2^{n-1}$  to  $2^{n-1}-1$

What is the range of values for a `signed char`?

Hint: A `char` is 1 byte long

{{% fragment %}}$-2^{7}$  to  $2^{7}-1$<br/>$-128$  to  $127${{% /fragment %}}

---

Question: Why is the positive maximum different to the negative maximum?
<br/>
<br/>

{{% fragment %}}Answer: We need to also store the $0$ value.<br/><br/>This zero value happens to use the positive range.{{% /fragment %}}

{{% /section %}}

---

## Unsigned Numbers

{{% section %}}

_"A `short` is 2 bytes long - it can hold 65536 values"_

<u>Unsigned variables</u> allow only positive values to be stored.  

an `unsigned short` has the range $0$ to $65535$  

> Unsigned Range: $0$  to  $2^{n}-1$

---

> Unsigned Range: $0$  to  $2^{n}-1$

What is the range of values for an `unsigned char`?

Hint: A `char` is 1 byte long

{{% fragment %}}$0$  to  $2^{8}-1$<br/>$0$  to  $255${{% /fragment %}}

{{% /section %}}
