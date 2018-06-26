## Part 3 Assignments

### 1. Python: Transforming a Matrix (an array of arrays) to a Dictionary
You will take the following matrix:
```python
def transform_matrix_to_dictionary(matrix):
    # YOUR LOGIC GOES HERE

# start with this matrix, and manipulate it into a dicionary
matrix = [['person', 'age', 'height, 'coolness_level'],
     ['Sonny',27, "5 ft 8 inches", 82],
     ['Tim',29, "5 ft 6 inches", 74],
     ['Gary', 14, "2 ft 1 inch", 23]]
     
dictionary = transform_matrix_to_dictionary(matrix)
print dictionary
```
and you can do whatever you'd like to transform it into a dictionary in the function ```transform_matrix_to_dictionary``` but the output should create a dictionary that looks like:
```python
{ # the top level dictionary
  "Sonny": {  #start of a new dictionary/object called "Sonny"
      "age": 27,
      "height": "5 ft 8 inches",
      "coolness_level": 82
  },
  "Tim":{  #start of a new dictionary/object called "Tim"
      "age": 29,
      "height": "5 ft 6 inches",
      "coolness_level": 74
  },
  "Gary":{  #start of a new dictionary/object called "Gary"
      "age": 14,
      "height": "2 ft 1 inch",
      "coolness_level": 23
  }
}
```

## 2. Python: Unscramble the String 
There was a problem with Shakespeare's text processer and the beautiful poem he wrote was scrambled! Fortunately the bug on his text processor was found online and the IT group made a post saying that the bug tends to scramble text this exact way:

1. all white space was turned to "." (periods)
2. the capitalized word beginning every sentence is lowercased
3. every "t" was changed to "4"
4. every "a" was changed to "$"
5. the whole string was reversed!

Knowing the logic of how the bug on Shakespeare's text processer messed up his poem, create a python function that converts the messed up string BACK to how it should look!

```python
def unscramble(string):
    # YOUR LOGIC GOES HERE

# this is the messed up string
string = ".4elup$c.$.eb.regnol.on.ll'i.dn$.,evol.ym.nrows.4ub.eb.,4on.4liw.uoh4.fi.,ro.;em$n.yh4.esufer.dn$.reh4$f.yh4.yned.?oemor.uoh4.4r$.eroferehw.!oemor.,oemor.o"

poem = unscramble(string)
print poem
```

## 3. Python: For-Loopin'
Write a program which will find all numbers divisible by 7 but **NOT** divisibly by 5, between 2000 and 5200 (both included). The numbers obtained should be printed in a comma-separated sequence on a single line.

To figure out if a number is divisible by 7, you will use the **modulus** ```%``` operator. An example:
```python
# modulus prints the REMAINDER of a division operation
print 14 % 7  # 14 is divisible by 7 so this will print 0
print 13 % 7  # this will print a remainder of 1!
print 16 % 7  # this will print a remainder of 2!

# to determine if a number is divisible by 7 you would check:
num = 39
if num % 7 == 0:
   print "The number is divisible by 7!"
else:
   print "The number is NOT divisible by 7!"
   
# to determine if a number is NOT divisible by 5
num = 11
if num % 5 != 0: # notice the exclamation mark ("==" means equals or is the same, "!=" means NOT the same)
  print "The number is NOT divisible by 5"
```
You will write a script that:
1. **loops** through all numbers between 2000 and 5200 
2. checks to see if the number is divisible by 7 and NOT divisible by 5
3. if it is divisible by 7 and not divisible by 5, add the number to an array

