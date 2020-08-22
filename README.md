# Arithmatic-Formatter
arrange arithmetic problems vertically to make them easier to solve. For example, "235 + 52" becomes:    235 +  52 -----
### Assignment

Students in primary school often arrange arithmetic problems vertically to make them easier to solve. For example, "235 + 52" becomes:

```
  235
+  52
-----
```

Create a function that receives arithmetic problems as a list of strings, and returns the problems arranged vertically and side by side. The function should optionally take a second argument in a boolean. When this argument is set to True, the function should also display the answer to the arithmetic problems.

### For example

Function Call:
```py
arithmetic_arranger(["32 + 698", "3801 - 2", "45 + 43", "123 + 49"])
```

Output:
```
   32      3801      45      123
+ 698    -    2    + 43    +  49
-----    ------    ----    -----
```

Function Call:
```py
arithmetic_arranger(["32 + 8", "1 - 3801", "9999 + 9999", "523 - 49"], True)
```

Output:
```
  32         1      9999      523
+  8    - 3801    + 9999    -  49
----    ------    ------    -----
  40     -3800     19998      474
```

### Rules

In the following instances, the function should return a string describing a meaningful error message.

* if there are more than five problems, return `Error: Too many problems.`
* if the problems include the multiplication * or division / characters, return `Error: Operator must be '+' or '-'.`
* if the operands include characters other than numbers, return `Error: Numbers must only contain digits.`
* if the operands have more than four digits, return `Error: Numbers cannot be more than four digits.`

When formatting the problems, the function should return a string following these rules:

* there should be a single space between the operator and the longest of the two operands
* the operator should be on the same line as the second operand
* the operands should be in the order in which they are provided. The first number will be the top one and the second will be the bottom.
* numbers should be right-aligned
* there should be four spaces between each problem
* there should be dashes at the bottom of each problem. These dashes should run along the entire length of each individual problem

Refer to previous examples to see how the output should look like.

Do not import any Python libraries.

### Development

Write your code in `arithmetic_arranger.py`. For development, you can use `main.py` to test your `arithmetic_arranger()` function. Click the "run" button and `main.py` will run.

### Testing 

The unit tests for this project are in `test_module.py`. We imported the tests from `test_module.py` to `main.py` for your convenience. The tests will run automatically whenever you hit the "run" button.
