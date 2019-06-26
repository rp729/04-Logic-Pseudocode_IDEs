<a href="https://github.com/CyberTrainingUSAF/04-IDE-s-and-Algorithms-Pt.-1/blob/master/00-Table-of-Contents.md" rel="Return to TOC"> Return to TOC </a>

# Pseudocode, Logic, and Design

**For this lesson, we are going to cover several concepts derived from: "Programming Logic & Design, comprehensive", 9th edition.**
**By Joyce Farrell** 

ISBN-10: 1-337-10207-5, ISBN-13: 978-1-337-10207-0

**Objectives**

**In this chapter, you will learn about:**
* Computer systems
* Simple program logic
* The steps involved in the program development cycle
* Pseudocode statements and flowchart symbols
* Using a sentinel value to end a program
* Programming and user environments
* The evolution of programming models

---

### Understanding Computer Systems

**Computer system**
* Combination of all the components required to process and store data using a computer

**Hardware**
* Equipment associated with a computer
  
**Software**
* Computer instructions that tells the hardware what to do
* Programs
  * Instructions written by programmers
* Programming
  * Writing software instructions
* Application software such as word processing, spreadsheets, payroll and inventory, even games, app
* System software such as operating systems like Windows, Linux, or UNIX, Google Android and Apple IOS

---
**Computer hardware and software accomplish three major operations**
* Input
  * Data items such as text, numbers, images, and sound
* Processing
  * Calculations and comparisons performed by the central processing unit (CPU)
* Output 
  * Resulting information that is sent to a printer, a monitor, or storage devices after processing
  * A cloud based device is accessed through the Internet

**Programming language**
* Used to write computer instructions called program code
* Writing instructions is called coding the program
* Examples
  * Visual Basic, C#, C++, or Java
  
**Syntax**
* Rules governing word usage and punctuation
* Mistakes in a language’s usage are syntax errors

**Computer memory**
* Computer’s temporary, internal storage – random access memory (RAM)
* Volatile memory – lost when the power is off

---

**Permanent storage devices**
* Nonvolatile memory

**Compiler or interpreter**
* Translates source code into machine language (binary language) statements called object code
* Checks for syntax errors

**Program executes or runs**
* Input will be accepted, some processing will occur, and results will be output

**Programs with syntax errors cannot execute**

---

**Logical errors**
* Errors in program logic produce incorrect output

**Logic of the computer program**
* Sequence of specific instructions in specific order

**Variable** 
* Named memory location whose value can vary

---

### Understanding the Program Development Cycle

**Program development cycle**
* Understand the problem
* Plan the logic
* Code the program
* Use software (a compiler or interpreter) to translate the program into machine language
* Test the program
* Put the program into production
* Maintain the program

---

   ## Program Development Cycle

![](/01_pseudocode/assets/Dev_Cycle.jpg)

---
## Using Software to Translate the Prgram into Machine Language

![](/01_pseudocode/assets/Machine_lang2.jpg)

---

### Statements and Flowchart Symbols

**Pseudocode**
* English-like representation of the logical steps it takes to solve a problem

**Flowchart**
* Pictorial representation of the logical steps it takes to solve a problem

## Writing Pseudocode

**Pseudocode representation of a number-doubling problem**

```
start
   input myNumber
   set myAnswer = myNumber * 2
   output myAnswer
stop

```

## Pseudocode Standards

* Programs begin with the word start and end with the word stop; these two words are always aligned
* Whenever a module name is used, it is followed by a set of parentheses
* Modules begin with the module name and end with return.  The module name and return are always aligned
* Each program statement performs one action

**Example** input, processing, or output
* Program statements are indented a few spaces more than the word start or the module name
* Each program statement appears on a single line if possible. When this is not possible, continuation lines are indented
* Program statements begin with lowercase letters
* No punctuation is used to end statements
---

## Drawing Flowcharts

**Create a Flowchart**
* Draw geometric shapes that contain the individual statements
* Connect shapes with arrows

**Input Symbol**
* Indicates input operation
* Parallelogram

![](/01_pseudocode/assets/input1.jpg)

**Processing symbol**
* Contains processing statements such as arithmetic
* Rectangle

![](/01_pseudocode/assets/mynumb2.jpg)

**Output symbol**
* Represents output statements
* Parallogram

![](/01_pseudocode/assets/MyAnsw3.jpg)

**Flowlines**
* Arrows that connect steps

**Terminal symbols**
* Start/stop symbols
* Shaped like a racetrack
* Called lozenges

![](/01_pseudocode/assets/StartStop4a.png)

![](/01_pseudocode/assets/Flowchart5.jpg)


---

## End a Program

**Making a Decision**
* Testing a value
* Decision symbol
  * Diamond shape
  
**Dummy value**
* Data-entry value that the user will never need
* Sentinel value

**End of File (eof)**
* Marker at the end of a file that automatically acts as a sentinel

![](/01_pseudocode/assets/EndProg6.png)

---

## Summary

* Hardware and software accomplish input, processing, and output

* Logic must be developed correctly

* Logical errors are much more difficult to locate than syntax errors

* Use flowcharts and pseudocode to plan the logic

* Avoid infinite loops by testing for a sentinel value

* Use a text editor or an IDE to enter your program statements
---

<a href="https://github.com/CyberTrainingUSAF/04-IDE-s-and-Algorithms-Pt.-1/blob/master/00-Table-of-Contents.md" > Continue to Next Topic </a>