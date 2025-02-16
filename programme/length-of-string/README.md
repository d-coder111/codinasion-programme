---
title: Length of string
description: Write a program to print the length of a string
image: hero.png
tags:
  - c
  - cpp
  - cs
  - python
  - java
  - go
  - js
contributors:
  - jojo4441
  - Badboy-16
  - manny-uncharted
  - superpthegreat
  - srabhishekh
  - MadhuS-1605
  - rossilor95
---

## Write a program to print the length of a string

```txt
Input  : abcd
Output : 4
```

---

<CodeBlock>

```c
#include <stdio.h>

#define LIMIT 32

int main()
{
  int length;
  char inputstr[LIMIT];

  printf("Input  : ");
  scanf("%s", inputstr);
  for (length = 0; inputstr[length] != '\0'; length++)
    ;
  printf("Output : %d\n", length);
  return 0;
}
```

```cpp
#include <iostream>
#include <string.h>
using namespace std;

int main()
{
  // string variable
  string str;

  // input
  cout << "Please enter a string : ";
  getline(cin, str);

  // output
  cout << "Length of string is : " << str.size() << endl;

  return 0;
}
```

```cs
using System;

public class LengthOfString
{
    static void Main(string[] args)
    {
        // Input string
        Console.Write("Input  : ");
        string input = Console.ReadLine();

        // Output length of string
        Console.WriteLine("Output : " + input.Length);
    }
}
```

```python
n = input("Input Enter a text : ")

print(f"\nLength of the string is {len(n)}")
```

```java
import java.util.Scanner;

public class StringLength {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter string : ");
        String input = scanner.next();
        System.out.println("\nLength of string : " + input.length());
        scanner.close();
    }
}
```

```go
package main

import "fmt"

func lengthOfString(s string) int {
	return len(s)
}

func main() {
	var s string
	fmt.Print("Enter a string : ")
	fmt.Scan(&s)
	fmt.Println("\nLength of string is", lengthOfString(s))
}
```

```javascript
const readline = require("readline");

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout,
});

rl.question("Input  : ", (inputString) => {
  console.log("Output :", inputString.length);
  rl.close();
});
```

</CodeBlock>
