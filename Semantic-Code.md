Here are 20 pairs of code and semantic queries across 10 different programming paradigms:

1. Python
Code:
```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return(fibonacci(n-1) + fibonacci(n-2))

print(fibonacci(10))
```
Semantic Query: Calculate the nth Fibonacci number using a recursive function.

2. Java
Code:
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
Semantic Query: Print "Hello, World!" to the console.

3. JavaScript
Code:
```javascript
const numbers = [1, 2, 3, 4, 5];
const doubledNumbers = numbers.map(num => num * 2);
console.log(doubledNumbers);
```
Semantic Query: Double each number in an array using the map function.

4. React Component
Code:
```jsx
import React from 'react';

const Button = ({ label, onClick }) => {
  return (
    <button onClick={onClick}>
      {label}
    </button>
  );
}

export default Button;
```
Semantic Query: Create a reusable Button component in React.

5. SQL
Code:
```sql
SELECT firstName, lastName
FROM employees
WHERE department = 'Sales'
ORDER BY lastName;
```
Semantic Query: Retrieve the first and last names of employees from the Sales department, ordered by last name.

6. C++
Code:
```cpp
#include <iostream>
using namespace std;

int main() {
    int num1, num2, sum;
    
    cout << "Enter two numbers: ";
    cin >> num1 >> num2;
    
    sum = num1 + num2;
    
    cout << "The sum is: " << sum;
    
    return 0;
}
```
Semantic Query: Write a program in C++ to take two numbers as input and print their sum.

7. Ruby
Code:
```ruby
class Person
  attr_reader :name, :age

  def initialize(name, age)
    @name = name
    @age = age
  end

  def greet
    puts "Hello, my name is #{name} and I'm #{age} years old."
  end
end

person = Person.new("Alice", 25)
person.greet
```
Semantic Query: Create a Person class with a name and age attribute, and a method to greet with the person's name and age.

8. Swift
Code:
```swift
var numbers = [1, 2, 3, 4, 5]
var evenNumbers = numbers.filter { $0 % 2 == 0 }
print(evenNumbers)
```
Semantic Query: Filter an array of numbers to get only the even numbers using the filter function in Swift.

9. C#
Code:
```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Enter your name:");
            string name = Console.ReadLine();
            Console.WriteLine($"Hello, {name}!");
        }
    }
}
```
Semantic Query: Write a C# program to ask the user for their name and print a greeting with their name.

10. Rust
Code:
```rust
fn is_palindrome(s: &str) -> bool {
    let reversed = s.chars().rev().collect::<String>();
    s == reversed
}

fn main() {
    let word = "racecar";
    if is_palindrome(word) {
        println!("{} is a palindrome", word);
    } else {
        println!("{} is not a palindrome", word);
    }
}
```
Semantic Query: Create a Rust function to check if a given string is a palindrome.

11. Go
Code:
```go
package main

import "fmt"

func findMax(nums []int) int {
    max := nums[0]
    for _, num := range nums {
        if num > max {
            max = num
        }
    }
    return max
}

func main() {
    numbers := []int{5, 2, 9, 1, 7}
    maxNum := findMax(numbers)
    fmt.Printf("The maximum number is: %d", maxNum)
}
```
Semantic Query: Write a Go program to find the maximum number in a slice of integers.

12. Kotlin
Code:
```kotlin
fun calculateArea(radius: Double): Double {
    return Math.PI * radius * radius
}

fun main() {
    val radius = 5.0
    val area = calculateArea(radius)
    println("The area of a circle with radius $radius is $area")
}
```
Semantic Query: Create a Kotlin function to calculate the area of a circle given its radius.

13. PHP
Code:
```php
<?php
function reverseString($str) {
    return strrev($str);
}

$originalString = "Hello, World!";
$reversedString = reverseString($originalString);

echo "Original string: " . $originalString . "\n";
echo "Reversed string: " . $reversedString;
?>
```
Semantic Query: Write a PHP function to reverse a given string.

14. R
Code:
```r
# Calculate the mean of a vector
my_vector <- c(1, 2, 3, 4, 5)
mean_value <- mean(my_vector)
print(mean_value)

# Plot a simple line chart
x <- 1:10
y <- x^2
plot(x, y, type = "l", main = "Square Function", xlab = "X", ylab = "Y")
```
Semantic Query: Calculate the mean of a vector and plot a simple line chart in R.

15. Scala
Code:
```scala
object FibonacciSequence extends App {
  def fibonacci(n: Int): Int = {
    if (n <= 1) n
    else fibonacci(n - 1) + fibonacci(n - 2)
  }

  println(fibonacci(10))
}
```
Semantic Query: Write a Scala program to calculate the nth Fibonacci number using recursion.

16. Bash
Code:
```bash
#!/bin/bash

read -p "Enter a number: " num

if [ $num -eq 0 ]; then
    echo "Zero is neither even nor odd."
elif [ $((num % 2)) -eq 0 ]; then
    echo "$num is even."
else
    echo "$num is odd."
fi
```
Semantic Query: Write a Bash script to check if a given number is even or odd.

17. SQL (with PostgreSQL syntax)
Code:
```sql
CREATE TABLE employees (
    id SERIAL PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    email VARCHAR(100) UNIQUE NOT NULL,
    hire_date DATE NOT NULL
);

INSERT INTO employees (first_name, last_name, email, hire_date)
VALUES ('John', 'Doe', 'john.doe@example.com', '2022-01-01'),
       ('Jane', 'Smith', 'jane.smith@example.com', '2021-03-15'),
       ('Michael', 'Johnson', 'michael.johnson@example.com', '2020-07-22');
```
Semantic Query: Create an employees table with columns for id, first name, last name, email, and hire date. Insert three rows of data into the table.

18. HTML/CSS
Code:
```html
<!DOCTYPE html>
<html>
<head>
    <title>My Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
        }
        h1 {
            color: #333;
            text-align: center;
        }
    </style>
</head>
<body>
    <h1>Welcome to My Page</h1>
    <p>This is a simple HTML page with some CSS styling.</p>
</body>
</html>
```
Semantic Query: Create a simple HTML page with a heading and a paragraph, styled with CSS to set the font family, background color, and heading color.

19. React Component (with JSX)
Code:
```jsx
import React, { useState } from 'react';

const Counter = () => {
  const [count, setCount] = useState(0);

  const incrementCount = () => {
    setCount(count + 1);
  };

  const decrementCount = () => {
    setCount(count - 1);
  };

  return (
    <div>
      <h1>Counter</h1>
      <p>Count: {count}</p>
      <button onClick={incrementCount}>Increment</button>
      <button onClick={decrementCount}>Decrement</button>
    </div>
  );
};

export default Counter;
```
Semantic Query: Create a React component that displays a counter value and has buttons to increment and decrement the counter.

20. TypeScript
Code:
```typescript
interface Person {
  name: string;
  age: number;
  greet: () => void;
}

class Employee implements Person {
  name: string;
  age: number;

  constructor(name: string, age: number) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, my name is ${this.name} and I'm ${this.age} years old.`);
  }
}

const employee = new Employee('John', 30);
employee.greet();
```
Semantic Query: Create a TypeScript class that implements a Person interface with properties for name, age, and a greet method.
