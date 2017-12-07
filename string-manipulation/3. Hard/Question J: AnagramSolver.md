# Anagram Solver
Create a program that will take *an anagram* and create all **possible permutations** of the letters to make possible english words. Then get each checked against a **dictionary array** (or just use the `SpellCheck program`).

## Getting all possible permutations
The explanation below involves a concept called **recursion**. As it will not be explained in depth, it is advised that you catch yourself up before continuing.

### What is Recursion?
Recursion is essentially calling a function on itself. For example:

```java
//main method
warpedMath(0);

//function that will call itself, until a is equal to 3
function warpedMath (int a) {
   if(a != 3) {
      a++;
      warpedMath(a); //calls itself again
   } else {
      return; //breaks out of the function
   }
}
```

The given example is a function that given an integer other than 3, it will constantly add a value to it until it is equal to 3. (**Note that if you put a value above 3 it will never stop**)

### Recursive Pseudocode
Things to know beforehand:
* Concept of Recursion
* Substring
* For loops
* ArrayList (or array)

```java
function permutations(String prefix, String object) { //the prefix is just the character that is the front of the word
  //Obtain the String's length
  
  if(String.length > 0) {
    //prefix is going to be the found word
    if(prefix is a word) {
      //print out prefix
    }
  } else {
    for(i starts at 0; i is less than String.length; i increments by 1) {
      //call permutations on itself, with the prefix set to the given string's .charAt(i) and the String object being the rest of the String
      permutations(the character of the string with index i, rest of string);
    }
  }
  
}
```

Implementing the above pseudocode will generate all possible values, outputted as the variable `prefix`. However, the runtime for each additional character increases exponentially and this code is quite slow.



