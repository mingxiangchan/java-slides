## Intro to Algorithms

---

### Definition

- method used to solve a problem

+++

### Problem

Find the age of the youngest person in a classroom of students

---

### Big O Notation

- measures the **worst case scenario** to solve a problem
- written as O(1), O(n), O(n<sup>2</sup>)

+++

### Worse Case Scenario

- more disk space
- more processing time
- more memory

+++

### O(1)

- constant time regardless of length of input
- examples
  - find first element in array
  - sum 2 numbers

+++

### O(n)

- time taken increases linearly with length of input
- examples
  - for loop

+++

### O(n<sup>2</sup>)

- time taken increases exponentially with length of input
- examples
  - nested for loop

+++

What is the Big O for

```java
int[][] x = {{1,2},{3,4}}

int target = 3

// find nested indexex of element matching target
for (int i = 0; i < x.length; i++) {
  y = x[i]

  for (int n = 0; n < max; n++) {
    z = y[n]

    if (z === 3) {
      return {i, n}
    }
  }
}


```

+++

Some Interesting Big Os

[Click Here](https://cooervo.github.io/Algorithms-DataStructures-BigONotation/index.html)

---

### Binary Search

+++

![](https://www.mathwarehouse.com/programming/images/binary-vs-linear-search/binary-and-linear-search-animations.gif)

+++

### Steps

1. sort the array
2. find element at `midpoint_index`
3. if `==` target, congrats! return `midpoint_indx`
4. if `>` or `<` target:
   - change `startIndex` and `endIndex`, recalulate midpoint
   - repeat from step 3
