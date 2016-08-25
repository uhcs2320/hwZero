# hw0, Minutes of Action. Due: soon.

You will create a C++ program that will count the total of minutes, hours, and days mentioned inside of a plain-text file.

## Input 

The input is a plain-text file, where each line is terminated with an end-of-line character.
Each line will have words or numbers.
To simplify we will assume that there will not be words containing numbers such as the word: car4sale. (Or numbers containg letters such as 22E01). A word is a string of letters (upper and lower case).
Lines in the input file that start with the symbol `#` should be considered comments and therefore skipped.

Example 1:

    #person of interest travels 20 minutes each day.
    Meredith travels 1 hour by train to visit Derek. However, Derek can visit her in one minute.
    Cristina does 4 minutes of yoga on her lunch break; she's done that in the last 3 weeks.

Each line that is not a comment will be process to find references of minutes, hours, or days.
Such items will be first a number and then one of these words: minute, minutes, hour, hours, day, days.
There may be empty lines in the input file.
The words and numbers may be separated by spaces, commas, period, new-line character, and parenthesis. Words and numbers will be separated by at least one non-letter or non-digit symbol.
You can assume that a word will be at most 30 characters long, and numbers will have maximum of 10 digits.

## Program specification

The main program should be called `uhday` and the syntax in which it will be tested is as follows:

`uhday "input=FILENAME"`

The parameter `input` specifies the name of the input file.

Example of program calls:

`uuday "input=gray.txt"`

## Output

Your program will output to the console (such as via cout, or printf) with the results of counting, independently, the minutes, hours, and days metioned in the file.
The first column is the time, the second is the name of the person, the third is the duration, and the fourth is the status.
Your program must follow the output format exactly to facilitate automated grading (and to avoid failing test cases due to things such as output of an empty line at the end).

Output for the input example.  (output is partial, just for illustration purposes).

    Minutes:24
    Hours:1
    Days:0

## Assumptions

* The input file can fit in main maimory (not larger than 10kb).

## Requirements

* This assignment is pass/fail. If your program scores more than 60 points, then you will pass. 
* Place your codes in a folder named: `hw0` (Failure to do so will cause your program to have a zero grade due to inability for doing automated grading).
* Your program should not produce any unexpected output when it is doing intermediate calculations because doing so will interfere with automated grading and some test cases will fail.
* You can not assume a maximum number of lines in the input file.
