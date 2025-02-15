# Excel Functions and Shortcuts

## Introduction:

Here is a brief overview of the excel functionalitites or shortcuts that were helpful in the process of navigating excel, Hope this helps you :)

***Credits:***\
<img width="155" alt="image" src="https://github.com/user-attachments/assets/a1ee359c-d5a2-4110-b299-dce2b3f460f0" />
> [Excel Formulas and Functions, BY: Kevin Stratvert](https://www.youtube.com/watch?v=Y8xhrUa3KH4&ab_channel=KevinStratvert)

## Basic Functionalities
### Keyboard Functions:
- CTRL+C: COPY
- CTRL+V: PASTE
- CTRL+X: CUT
- CTRL+Z: UNDO
- **CTRL+Y: REDO**
- **CTRL+(UP ARROW): Go to top row**
- CTRL+(DOWN ARROW): Go to bottom row
- CTRL+(LEFT ARROW): Go to extreme left column
- CTRL+(RIGHT ARROW): Go to extreme right column
- CTRL+SHIFT+V: Paste just the value and not the formatting
- **F2: Edit Active Cell**
- **CTRL+D: Fill down from cell above**
- **CTRL+SHIFT+"+": Insert new row**
- CTRL+SPACE then CTRL+SHIFT+"+": Insert new column
- SHIFT+SPACE then CTRL+"-": Delete row
- CTRL+"mouse click": Select multiple cells
- **ALT+(DOWN ARROW): Create dropdown list**
- **CTRL+D: Autofill Down**
- **CTRL+R: Autofill right**
- CTRL+B: Bold character
- CTRL+I: Italic Character
- CTRL+U: Underline character
- **ALT+N+V: Create Pivot Table**
- **ALT+SHIFT+(RIGHT ARROW): Group Selected Data**
- **ALT+SHIFT+(LEFT ARROW): Ungroup Selected Data**
- **ALT+A+R+A: Refresh All Pivot Tables**
- **ALT+"=": Autosum**
- **CTRL+F: FIND**
- **CTRL+H: REPLACE**
- **CTRL+SHIFT+L: Apply/Remove Filters**
- **ALT+(DOWN ARROW) on column header: Open Filter Menu**


*Always use '=' for entering formulas/functions*

*Here use the formula bar whenever necessary, it is in the top section and find out different functions that assist you in your work*
<img width="800" height="100" alt="image" src="https://github.com/user-attachments/assets/10f87637-9a45-457b-9edf-e8ffaf5061c9" />

**Absolute References**
<img width="1149" alt="image" src="https://github.com/user-attachments/assets/834f2b2d-2660-4438-9e29-c76c5283dd62" />
- Using F4 key as a shortcut for absolute reference
- $ represents the absolute reference it can be used as a prefix for either column or row i.e as below cases
  - $A$2: This would mean an absolute reference of A column and 2nd row
  - $A2: Here the absolute reference is only for the A column not on the row eg: A3, A4...
  - A$2: Here the absolute reference is only for the 2nd row but not for the column  eg: B2, C2...
 
To get absolute reference from another tab, follow below steps:
- Get the tab name in **'** single quotes
- Leave an exclaimation mark next to it
- add the absolute reference column next to the exclamation mark( it needs $ sign to be absolute) 
<img width="1106" alt="image" src="https://github.com/user-attachments/assets/d4a8d099-f698-4ce7-a6ec-a1f6007689c7" />



### Arithmetic Operations
- SUM(A1:A9): Gives out the summation values
- AVERAGE(A1:A9): Gives out the average values
- PRODUCT(A1:A9): Gives product of a set of numbers in a range of cells
- MAX(A1:A9): Gives out the maximum values from the given set
- MIN(A1:A9): Gives out minimim values from the given set
- **Other Minor Arithmetic Functions/Formulas**
  - A1*A2: Use of wildcard is for the multiplication
  - A1/A2: Forward slash is used for the division
  - QUOTIENT(18,3): Gives you the quotient
  - MOD(10,3): Gives you the remainder value
  - ABS(A1): Gives the absolute value(+,- as +)
  - **ROUND(A1,2): Rounding to 2 decimal points**
  - CEILING(6.7) -> 7 : Getting nearest higher integer 
  - FLOOR(6.7) -> 6 : Getting nearest lower integer 
- **Different Counts:**
  - COUNT(A1:A9): Gives out the total number of **numerical values** present in that list
  - **COUNT(A1:A9): Gives out the total number of **character/string values** present in that list**
  - COUNT(A1:A9): Gives out the total number of **blank** values present in that list
- **LARGE(A1:A9,2): Here 2 is the position i.e we get the 2nd highest from A1:A9**
- **SMALL(A1:A9,2): Here 2 is the position i.e we get the 2nd lowest from A1:A9**
- **Logical and Arithmetic Operators**
  - ">=" : Greater than equal to
  - "<" : Less than
  - ">" : Greater than
  - "=" : Equal to
  - "<=" : Less than equal to
  - "<>" : Not equal to

### String Functions  

---

####  1. Basic String Functions  

| Function  | Description                        | Example                | Result    |
|-----------|------------------------------------|------------------------|-----------|
| **LEFT()** | Extracts **N** characters from the left | `=LEFT("Excel",2)`     | `"Ex"`    |
| **RIGHT()** | Extracts **N** characters from the right | `=RIGHT("Excel",2)`    | `"el"`    |
| **MID()** | Extracts a substring from a given position | `=MID("Excel",2,3)` | `"xce"`   |
| **LEN()** | Returns the **length** of a string | `=LEN("Excel")`       | `5`       |
| **TRIM()** | Removes extra spaces | `=TRIM("  Hello  World  ")` | `"Hello World"` |
| **UPPER()** | Converts text to **uppercase** | `=UPPER("excel")`     | `"EXCEL"` |
| **LOWER()** | Converts text to **lowercase** | `=LOWER("Excel")`     | `"excel"` |
| **PROPER()** | Capitalizes **first letter** of each word | `=PROPER("hello world")` | `"Hello World"` |

---

####  2. Combining & Splitting Strings  

| Function  | Description                        | Example                 | Result             |
|-----------|------------------------------------|-------------------------|--------------------|
| **CONCAT()** | Joins multiple text values | `=CONCAT("Hello", " ", "World")` | `"Hello World"` |
| **TEXTJOIN()** | Joins text with a delimiter | `=TEXTJOIN(", ", TRUE, "Apple", "Banana", "Cherry")` | `"Apple, Banana, Cherry"` |
| **& (Ampersand)** | Concatenates strings manually | `="Hello" & " " & "World"` | `"Hello World"` |

---

####  3. Searching & Replacing  

| Function  | Description                        | Example                 | Result |
|-----------|------------------------------------|-------------------------|--------|
| **FIND()** | Finds position of a substring (case-sensitive) | `=FIND("e", "Excel")` | `2` |
| **SEARCH()** | Finds position of a substring (not case-sensitive) | `=SEARCH("e", "EXCEL")` | `2` |
| **SUBSTITUTE()** | Replaces **all occurrences** of a text | `=SUBSTITUTE("2024-07-01", "-", "/")` | `"2024/07/01"` |
| **REPLACE()** | Replaces text at a specific position | `=REPLACE("Excel", 2, 2, "XX")` | `"EXXel"` |

---

#### 4. Formatting & Extracting Text  

| Function  | Description                        | Example                 | Result    |
|-----------|------------------------------------|-------------------------|-----------|
| **TEXT()** | Formats numbers as text | `=TEXT(1000, "$#,##0.00")` | `"$1,000.00"` |
| **VALUE()** | Converts text to number | `=VALUE("100")` | `100` |
| **NUMBERVALUE()** | Converts localized numbers to numeric values | `=NUMBERVALUE("1.234,56", ",", ".")` | `1234.56` |

---

####  5. Handling Errors & Special Cases  

| Function  | Description                        | Example                 | Result |
|-----------|------------------------------------|-------------------------|--------|
| **EXACT()** | Checks if two strings are exactly the same (case-sensitive) | `=EXACT("Excel", "EXCEL")` | `FALSE` |
| **ISTEXT()** | Checks if a value is text | `=ISTEXT("Excel")` | `TRUE` |
| **ISNUMBER()** | Checks if a value is a number | `=ISNUMBER("Excel")` | `FALSE` |

---

  
 
