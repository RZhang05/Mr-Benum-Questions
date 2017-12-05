# Word Search Solver
Write a program that will solve a **word search** that is provided as a **text file**. The output should show the found words by making them contrast with the **random letters**. This could be achieved by making the words show in `UPPERCASE` and the random filler letters in `lowercase`. Again, consider **horizontal words only**.

## General Idea :bulb:
Taking the program you wrote for the previous question, you can adapt the general idea, to **Search for** instead of **produce** the crossword's terms.

## Sample Run
### Input from file: words.txt (the words you're looking for)
```
== Words.txt==
green
red
magenta
yellow
purple
blue
orange
white
black
turquoise
cyan
blurple
grey
```

### Input from file: wordsearch.txt (the wordsearch file)
```
muggreenpfskb
whredibghecyb
sehflmagentao
uidyellowfker
dhlmpurplepxm
pbluehqhtmniy
norangexpkjkz
whiteuqzqkbda
scbblackobjfi
amturquoiseei
klcyanxhjmlch
xbohjvblurple
greyivfajrhfe
```

### Console Output (the solved file)
```
mug-GREEN-pfskb
wh-RED-ibghecyb
sehfl-MAGENTA-o
uid-YELLOW-fker
dhlm-PURPLE-pxm
p-BLUE-hqhtmniy
n-ORANGE-xpkjkz
WHITE-uqzqkbda
scb BLACK-objfi
am-TURQUOISE-ei
kl-CYAN-xhjmlch
xbohjv-BLURPLE
GREY-ivfajrhfe
```

