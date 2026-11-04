# Using Files in Java

### Starter Code - File Example

Here is a file example using a file called `input.txt` stored in the `src` folder. It counts the number of letter `a's` in the text file.

```java
import java.io.File;  
import java.io.IOException;  
import java.util.Scanner;  
  
public class Main {  
    public static void main(String[] args) throws IOException {  
  
        File myObj = new File("src/input.txt");  
        Scanner myReader = new Scanner(myObj);  
        StringBuilder data = new StringBuilder();  
  
        while (myReader.hasNextLine()) {  
            data.append(myReader.nextLine()).append("\n");  
        }  
        System.out.println(data);  
  
        int counter = 0;  
        for (char letter : data.toString().toCharArray()) {  
            if (letter == 'a' || letter == 'A') {  
                counter++;  
            }  
        }  
        System.out.println("Number of a's: " + counter);  
    }  
}
```

---
## Exercises

## 07-0: Count the Number of Lines

In **IntelliJ IDEA**, create a **New Project** called **CountLines**.

In the **src** folder create a **Java class** file called *CountLines.java* with the following source code.
### Objective

Practice opening a file and reading it line by line.

### File

Make a text file in your `src` folder called

`poem.txt`

with the following contents

```
Roses are red
Violets are blue
Java is fun
And programming too
```

### Task

Write a program that:

1. Opens `poem.txt`.
2. Reads every line.
3. Counts how many lines are in the file.
4. Displays the total.

### Sample Output

```
Number of lines: 4
```

### Concepts

- `File`
- `Scanner`
- `while(hasNextLine())`
- Counter variables
---

## 07-1: Calculate the Sum and Average of Numbers

In **IntelliJ IDEA**, create a **New Project** called **SumAverageNumbers**.

In the **src** folder create a **Java class** file called *SumAverageNumbers.java* with the following source code.
### Objective

Read numeric data from a file.

### File

`marks.txt`

```
78
85
92
67
88
```

### Task

Write a program that:

1. Reads all the numbers from the file.
2. Calculates the sum.
3. Calculates the average.
4. Displays both values.

### Sample Output

```
Sum: 410
Average: 82.0
```

### Extension

Find the highest and lowest mark.

### Concepts

- `hasNextInt()`
- Accumulators
- Numeric processing

---

## 07-2: Word Search

In **IntelliJ IDEA**, create a **New Project** called **WordSearch**.

In the **src** folder create a **Java class** file called *WordSearch.java* with the following source code.
### Objective

Search for specific text within a file.

### File

`story.txt`

```
The dragon flew over the mountain.
The knight chased the dragon.
The dragon found a cave.
```

### Task

Ask the user for a word (e.g., "dragon").

The program should:

1. Read each line of the file.
2. Count how many lines contain the word.
3. Display the count.

### Sample Output

```
Enter word: dragon

The word appears in 3 lines.
```

### Extension

Display the matching lines.

### Concepts

- String methods
- `contains()`
- User input combined with file input

---

## 07-3: Create a Student Directory

In **IntelliJ IDEA**, create a **New Project** called **StudentDirectory**.

In the **src** folder create a **Java class** file called *StudentDirectory.java* with the following source code.
### Objective

Extract structured information from a text file.

### File

`students.txt`

```
Emma,17
Liam,18
Sophia,17
Noah,18
```

### Task

Write a program that:

1. Reads each line.
2. Splits the line into name and age.
3. Displays the information in a formatted way.

### Sample Output

```
Student: Emma   Age: 17
Student: Liam   Age: 18
Student: Sophia Age: 17
Student: Noah   Age: 18
```

### Extension

Count how many students are 18 years old.

### Concepts

- `split(",")`
- Parsing file data
- String arrays

---

## 07-4: Analyze a Book File

In **IntelliJ IDEA**, create a **New Project** called **BookFile**.

In the **src** folder create a **Java class** file called *BookFile.java* with the following source code.
### Objective

Perform multiple calculations while reading a file.

### File

`book.txt` (Any paragraph of text.)

### Task

Determine:

1. Total number of lines.
2. Total number of words.
3. Total number of characters (excluding spaces).

### Sample Output

```
Lines: 12
Words: 145
Characters: 623
```

### Extension

Find the longest word in the file.

### Concepts

- Nested processing
- String manipulation
- Counters

---

## 07-5: Grade Report Generator

In **IntelliJ IDEA**, create a **New Project** called **GradeReportGenerator**.

In the **src** folder create a **Java class** file called *GradeReportGenerator.java* with the following source code.
### Objective

Use file input to produce a meaningful report.

### File

`grades.txt`

```
Alice 85
Bob 72
Charlie 91
Diana 67
Ethan 88
```

### Task

Write a program that:

1. Reads each student's name and grade.
2. Calculates the class average.
3. Determines the highest grade.
4. Lists all students who scored above the average.

### Sample Output

```
Class Average: 80.6

Highest Grade:
Charlie - 91

Students Above Average:
Alice - 85
Charlie - 91
Ethan - 88
```

### Extension

Assign letter grades (A, B, C, D, F).

### Concepts

- File processing
- Arrays or `ArrayList`
- Multiple passes through data (or storing data in memory)

---
