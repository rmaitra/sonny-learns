## Part 3 Assignments

### 1. Python: Transforming a Matrix (an array of arrays) to a Dictionary
You will take the following matrix:
```python
# start with this matrix, and manipulate it into a dicionary
matrix = [['person', 'age', 'height, 'coolness_level'],
     ['Sonny',27, "5 ft 8 inches", 82],
     ['Tim',29, "5 ft 6 inches", 74],
     ['Gary', 14, "2 ft 1 inch", 23]]
```
and you can do whatever you'd like to transform it into a dictionary that looks like:
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

