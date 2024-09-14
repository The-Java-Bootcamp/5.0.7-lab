# Lab 5.0.7

**Learning Objectives**

- Understand the concept and importance of the `==` operator and the `equals()` method in Java development.
- Learn how to use `==` for primitive type comparisons and `equals()` for String comparisons.
- Explore practical applications of equality comparison in simple Java programs.
- Identify common pitfalls and best practices when working with equality in Java.
- Gain hands-on experience with a complete Java example that demonstrates proper use of `==` and `equals()`.

**Prerequisites**

- Basic understanding of Java programming.
- Familiarity with primitive data types and String objects in Java.
- Knowledge of basic Java control structures (loops, conditionals).

**What You'll Achieve**

- Develop a solid understanding of equality comparisons in Java.
- Implement practical examples that demonstrate the difference between `==` and `equals()`.
- Enhance your skills in working with primitive types and String objects.

**Assignment Details**

In the main method, perform the following comparisons and print the results:

1. Compare two int variables (both with value 5) using `==`.
2. Compare two double variables (2.0 and 2.00) using `==`.
3. Compare two String objects with the value "hello", one created using `new` and one as a string literal, using
   both `==` and `equals()`.
4. Compare two String variables initialized with the string literal "world" using `==`.
5. Use `equalsIgnoreCase()` to compare "Java" with "java".

**Example Output**

```
int comparison (5 == 5): true
double comparison (2.0 == 2.00): true
String comparison (new vs literal):
"hello" == "hello": false
"hello".equals("hello"): true
String comparison (literal vs literal):
"world" == "world": true
Case insensitive comparison ("Java".equalsIgnoreCase("java")): true
```

**Starter Code**

```java
package academy.javapro.lab;

public class EqualityLab {
    public static void main(String[] args) {
        int num1 = 5;
        int num2 = 5;

        double d1 = 2.0;
        double d2 = 2.00;

        String s1 = new String("hello");
        String s2 = "hello";

        String s3 = "world";
        String s4 = "world";

        String str1 = "Java";
        String str2 = "java";
    }
}

```

**Hints**

- The `==` operator compares the actual values for primitive types like int and double.
- For String objects, `==` compares the references, not the content.
- The `equals()` method for String compares the actual content of the strings.
- String literals with the same value refer to the same object in memory, which is why `==` works for them.
- `equalsIgnoreCase(`) is useful when you want to compare strings regardless of their capitalization.

**Submission Instructions**

1. Fork the repository
2. Clone your fork
3. Navigate into the repository
4. Implement the required loops in the main method
5. Test your implementation with various inputs
6. Git add, commit, and push to your fork
7. Submit a pull request
    - Set the title of the pull request to your first name and last name
    - In the comment, briefly explain your implementation approach and any challenges you faced

Remember, the goal is to learn and have fun! Don't hesitate to ask for help if you get stuck.