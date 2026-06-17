  # Arrays



### What is an Array?



An array is basically a container that stores **multiple values under one variable name**.



Instead of doing:



```java

String fruit1 = "Apple";

String fruit2 = "Banana";

String fruit3 = "Orange";

```



You can do:



```java

String[] fruits = {"Apple", "Banana", "Orange"};

```



**Think of it like:** One box with multiple slots inside.



---



### Array Declaration



```java

variableType[] name;

```



Example:



```java

String[] fruits;

int[] scores;

```



**What it does:** Creates the array variable, but doesn't create the actual slots yet.



---



### Creating the Array



```java

name = new variableType[#];

```



Example:



```java

fruits = new String[3];

```



| Part     | Meaning         |

| -------- | --------------- |

| `fruits` | Array name      |

| `String` | Data type       |

| `3`      | Number of slots |



**How I remember it:**



* `String[] fruits;` = Creates the paper.

* `new String[3];` = Draws 3 empty spaces on the paper.



Without a size, Java won't know how many slots to make.



---



### Data Types Still Matter



Arrays follow the same variable rules.



| Data          | Type      |

| ------------- | --------- |

| Words/Text    | `String`  |

| Whole Numbers | `int`     |

| Decimals      | `double`  |

| True/False    | `boolean` |



Example:



```java

String[] fruits = {"Apple", "Banana"};

int[] scores = {90, 85, 100};

double[] prices = {5.25, 10.99};

```



**Reminder:** I often forget that arrays still need the correct data type.



---



### Indexes



Arrays use **indexes** to access values.



**Important:** Indexes always start at **0**.



```java

String[] fruits = {"Apple", "Banana", "Orange"};

```



| Index | Value  |

| ----- | ------ |

| 0     | Apple  |

| 1     | Banana |

| 2     | Orange |



Example:



```java

System.out.println(fruits[0]);

```



Output:



```java

Apple

```



---



### Multidimensional Arrays



A multidimensional array has rows and columns.



Example:



```java

int[][] numbers = {

    {1, 2, 3},

    {4, 5, 6}

};

```



Think of it like a table:



| Row/Column | 0 | 1 | 2 |

| ---------- | - | - | - |

| 0          | 1 | 2 | 3 |

| 1          | 4 | 5 | 6 |



---



### Accessing Values



For multidimensional arrays:



```java

array[row][column]

```



Example:



```java

numbers[1][2]

```



| Part | Meaning |

| ---- | ------- |

| `1`  | Row     |

| `2`  | Column  |



Result:



```java

6

```



**What confused me before:** You must specify BOTH the row and the column. Also, counting still starts at `0`.



---



### Important Notes



* `int` = whole numbers only.

* Decimal values like `5.25` need `double` or `float`.



Example:



```java

double price = 5.25;

```



* In multidimensional arrays, each row gets its own `{ }`.

* Rows are separated with commas.



Example:



```java

int[][] numbers = {

    {1, 2, 3},

    {4, 5, 6}

};

```



* Numbers do **not** use quotation marks.

* Strings **must** use quotation marks.

| Correct   | Wrong                |
| --------- | -------------------- |
| `"Apple"` | `Apple`              |
| `5`       | `"5"` (if using int) |


---

### One-Line Summary
| Concept                | What It Does                           |
| ---------------------- | -------------------------------------- |
| Array                  | Stores multiple values in one variable |
| Index                  | Position of a value                    |
| First Index            | Always starts at 0                     |
| Multidimensional Array | Uses rows and columns                  |
| `int`                  | Whole numbers                          |
| `double`               | Decimal numbers                        |



      
