---
title: Inches to Feet
description: Write a programme to convert inches to feet
image: hero.png
tags:
  - c
  - python
  - cpp
  - java
  - js
  - go
  - cs
contributors:
  - ClasherKasten
  - rossilor95
---

## Write a programme to convert inches to feet

```txt
Input  : 12
Output : 1
```

---

<CodeBlock>

```c
#include <stdio.h>

int main(void)
{
    int inch;
    printf("Input  : ");
    scanf("%d", &inch);
    printf("Output : %f\n", inch / 12.0);
    return 0;
}
```

```python
print("Output :", int(input("Input  : ")) / 12)
```

```cpp
#include <iostream>

int main(void)
{
    int inch;
    std::cout << "Input  : ";
    std::cin >> inch;
    std::cout << "Output : " << inch / 12.0 << std::endl;
    return 0;
}
```

```java
import java.util.Scanner;

class InchesToFeet {

  public static void main(String[] args) {
    try (Scanner sc = new Scanner(System.in)) {
      System.out.print("Input  : ");
      int inches = sc.nextInt();
      System.out.print("Output : ");
      System.out.println(inches / 12.0);
    } catch (Exception e) {
      System.err.println("An Error occured");
    }
  }
}
```

```javascript
"use strict";

const readline = require("readline");

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

rl.question("Input  : ", (inches) => {
  const result = parseInt(inches) / 12;
  if (!isNaN(result)) {
    console.log(`Output : ${result}`);
  } else {
    console.log("An Error occured");
  }
  rl.close();
});
```

```go
package main

import "fmt"

func inchesToFeet(inches float32) float32 {
	return inches / 12.0
}

func main() {
	fmt.Print("Input  : ")

	var inches float32
	fmt.Scan(&inches)

	fmt.Println("Output :", inchesToFeet(inches))
}
```

```cs
using System;

namespace UnitConversion
{
    public class InchesToFeet
    {
        public static double ConvertInchesToFeet(double inches) =>
            inches / 12.0;

        public static void Main()
        {
            Console.Write("Input  : ");

            double inches;
            if (double.TryParse(Console.ReadLine(), out inches))
            {
                double feet = ConvertInchesToFeet(inches);
                Console.WriteLine("Output : " + Math.Round(feet, 2));
            }
            else
            {
                Console.WriteLine("Invalid Input");
            }
        }
    }
}
```

</CodeBlock>
