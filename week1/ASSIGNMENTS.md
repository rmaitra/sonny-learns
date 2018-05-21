## 1. Dice Rolling Simulator

The Goal: Like the title suggests, this project involves writing a program that simulates rolling dice. When the program runs, it will randomly choose a number between 1 and 6. (Or whatever other integer you prefer — the number of sides on the die is up to you.) The program will print what that number is. It should then ask you if you’d like to roll again. For this project, you’ll need to set the min and max number that your dice can produce. For the average die, that means a minimum of 1 and a maximum of 6. You’ll also want a function that randomly grabs a number within that range and prints it.
Concepts to keep in mind:

- Random
- Integer
- Print
- While Loops

you will want to use this library:
```python
import random
```

### Requirements
1. a function that randomly gets a number between a specified range
2. ask the user for "yes" or "no" input on whether to roll again

## 2. Magic 8 Ball Program

The Goal: Yes, you'll program that randomly gives these responses for any user inputed question:

1. "It is certain"
2. "Outlook good"
3. "You may rely on it"
4. "Ask again later"
5. "Concentrate and ask again"
6. "Reply hazy, try again"
7. "My reply is no"
8. "My sources say no"

Notice there are 8 responses. You will need to randomly generate a number between 1-8 and based on the number, you will pick a response, no matter the question, then print the response.

you will want to use this library:
```python
import random
```

### Requirements
1. ask the user for a question
2. print a response randomly between the 8 responses given
3. be able to quit the program if the user says "quit" or continue to prompt the user

## 3. Plot Random Array of Numbers

The Goal: learn how to generate an array of random numbers (of any range e.g. 0-100, -1000-3000, etc) and plot them as a line curve with ```matplotlib```. 

These are the python libraries you will use:
```python
import random
import matplotlib
```

### Requirements
1. the program should generate 1000 random numbers and add them to an array.
2. the array should be plotted
3. the average of the random numbers should be calculated
4. the average should be plotted as a straight line

## 4. Open/Read/Manipulate a CSV file of financial data

The Goal: 
- learn how to open a file with a program
- store the lines of a CSV into an array
- plot the data

These are the python libraries you will use:
```python
import matplotlib
```

### Requirements
1. the program should first open hw3.csv which is in this repository
2. read the csv, line by line, and append the number data into an array
3. calculate the average of the array
4. plot the data and the average 
