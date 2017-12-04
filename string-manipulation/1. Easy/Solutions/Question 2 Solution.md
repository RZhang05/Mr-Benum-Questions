# Name Arranger
## Idea

It is possible to do this by storing the second name with the comma as one variable, then storing the first name in a separate variable.

When outputting, just out the first name and then the substring of the second name, from the *0th* index to the length of the string subtracted by 1.

## Pseudocode

```
input(secondName)
input(firstName)

output(firstName + " " + secondName.substring(0, secondName.length - 1))
```
