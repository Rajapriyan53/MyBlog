---
title: "Day1"
lastmod: 2020-06-23
date: 2020-06-20
draft: false
---
## Python

#### Data types

1. **Text type:**                  str  
2. **Numeric Types:**         int, float, complex
3. **Sequence Types:**  list, tuple, range
4. **Mapping Type:** 	dict
5. **Set Types:** 	set, frozenset
6. **Boolean Type:** 	bool
7. **Binary Types:** 	bytes, bytearray, memoryview



#### Storage Types
 

1.  **List** is a collection which is ordered and changeable. Allows duplicate members. **Example**: thislist = \["apple", "banana", "cherry"\] <br>

2.  **Tuple** is a collection which is ordered and unchangeable. Allows duplicate members. **Example**:  thistuple = ("apple", "banana", "cherry") <br>

3.  **Set** is a collection which is unordered and unindexed. No duplicate members.**Example**:  thisset = {"apple", "banana", "cherry"}<br>

4.  **Dictionary** is a collection which is unordered, changeable and indexed. No duplicate members. **Example**:   thisdict =  {  
  "brand": "Ford",  
  "model": "Mustang",  
  "year": 1964  
}


#### Lambda function

A lambda function is a small anonymous function.

A lambda function can take any number of arguments, but can only have one expression.

**Example :**  x = lambda a : a + 10  

#### Class Example

class Person:  
  def \_\_init\_\_(self, name, age):  
    self.name = name  
    self.age = age  
  
p1 = Person("John", 36)  
  
print(p1.name)  
print(p1.age)

#### RegEx Functions

1. **findall** - 	Returns a list containing all matches
2. **search**- 	Returns a Match object if there is a match anywhere in the string
3. **split**- 	Returns a list where the string has been split at each match
4. **sub** - 	Replaces one or many matches with a string

      **Any Character Except New Line**
\d      - Digit (0-9)
\D      - Not a Digit (0-9)
\w      - Word Character (a-z, A-Z, 0-9, _)
\W      - Not a Word Character
\s      - Whitespace (space, tab, newline)
\S      - Not Whitespace (space, tab, newline)

\b      - Word Boundary
\B      - Not a Word Boundary
^       - Beginning of a String
$       - End of a String

[]      - Matches Characters in brackets
[^ ]    - Matches Characters NOT in brackets
|       - Either Or
( )     - Group

**Quantifiers:**

\*     0 or More

\+       1 or More
      
?       - 0 or One

{3}     - Exact Number

{3,4}   - Range of Numbers (Minimum, Maximum)

**Examples:**

+ pattern = re.compile(r'abc')

+ matches = pattern.finditer(text_to_search)

+ for mat in matches:
    print(mat)
    
**Output:**
&lt;re.Match object; span=(1, 4), match='abc'&gt;
&lt;re.Match object; span=(69, 72), match='abc'&gt;



