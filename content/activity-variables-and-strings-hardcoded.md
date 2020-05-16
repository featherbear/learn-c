---
title: "Activity: Variables and Strings"
layout: "bundle"
outputs: ["Reveal"]
date: 2020-05-15T01:20:42+10:00
---

> Write a program to store the numbers 3 and 15. Find the product and display it.

Hint: Multiply numbers like this - `a*b`

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
    int number1 = 3;
    int number2 = 15;

    int product = 3 * 15;

    printf("%d * %d = %d\n", number1, number2, product);

    return 0;
}
```

{{% /section %}}

---

Write a program to display the word "Butterfly", and programmatically print the second letter of the word.

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
    char word[] = "Butterfly";

    printf("The word is %s\n", word);
    printf("The second letter is %c", word[1]);

    return 0;
}
```

{{% /section %}}

---

Write a program to print out the number 1 and the first letter of the alphabet. Then print out the number 2, and the second letter of the alphabet.

{{% fragment %}}<br/>Now also print out the number 3, and the third letter{{% /fragment %}}

{{% fragment %}}<br/><br/>Now print out the remaining 23 numbers and letters...{{% /fragment %}}

---

{{< slide class="center" >}}

## Next Steps

> [Loops](../loops)

