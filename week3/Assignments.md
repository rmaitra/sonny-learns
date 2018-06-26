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
```
