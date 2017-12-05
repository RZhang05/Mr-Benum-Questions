# Spell Checker
Get a word as input and check it against a **text file dictionary** `(downloaded from the Internet)`. Consider doing a **binary search** for greater efficiency.

## Suggested Source
This source excludes quite a lot of words, however it does cover a large amount of English language with over `80,000` words included.

[View source here](http://www.gwicks.net/dictionaries.htm)

The one used for this program was the first one at `84,000` words for time efficiency.
You can use any other sizes, however your search will take longer even with **binary search**.

## General Idea :bulb:
Reading through a text file of words is quite simple, as per the previous questions. However, the concept of a **binary search** may be harder to understand.

Here is the basic concept:
* A Binary Search compares the element to the middle element in the given list
* If it is lower, compare it to the middle of the lowest point in the list, and the middle of the list
* If it is higher, compare it to the middle of the middle of the list and the highest point in the list

**Example**
Remember that the lowest range is the index, but we change the highest range according to the results.

`Searching for: 80` `List: 1 to 100` `Initial Values: Lowest range = 0 | Highest range = 100`

⬆️ = `Went up` ⬇️ = `Went down` 🎰 = `Success`
* `First run:` 80 compares to 50 | Result: 80 is higher ⬆️ | Lowest range = 50 ⬆️ | Highest range = 100
* `Second run:` 80 compares to 75 | Result: 80 is higher ⬆️ | Lowest range = 75 ⬆️ | Highest range = 100
* `Third run:` 80 compares to 87 | Result: 80 is lower ⬇️ | Lowest range = 75 | Highest range = 87 ⬇️
* `Fourth run:` 80 compares to 81 | Result: 80 is lower ⬇️ | Lowest range = 75 | Highest range = 81 ⬇️
* `Fifth run:` 80 compares to 79 | Result: 80 is higher ⬆️ |  Lowest range = 79 ⬆️ | Highest range = 81
* `Sixth run:` 80 compares to 80 | Result: WE FOUND IT! 🎰 | Lowest range = 80 ⬆️ | Highest range = 81

## Example Run
### User Console
```
(prompt) Enter a word:
(user)   appliance
```

### Console Output
Note: There is no need to output the currently checking, this is for **readability** purposes.
```
Currently checking: laurence
Currently checking: diner
Currently checking: canonizing
Currently checking: backstops
Currently checking: analysers
Currently checking: armors
Currently checking: aoudad
Currently checking: appropriations
Currently checking: apparently
Currently checking: appliqu�d
Currently checking: appends
Currently checking: applauding
Currently checking: applicability
Currently checking: appledore
Currently checking: appletreewick
Currently checking: appliance
Direct match: appliance
```



