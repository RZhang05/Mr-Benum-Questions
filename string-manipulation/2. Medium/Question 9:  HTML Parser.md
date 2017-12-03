# HTML Parser

Remove text between HTML tags. In general, your program should ensure that the tags match.

## Sample Input 1
```
<p>This is a paragraph.</p>
```
## Sample Output 1
```
This is a paragraph.
```
## Sample Input 2
```
<h1>The biggest heading</h1>
```
## Sample Output 2
```
The biggest heading
```
## Sample Input 3
```
<title>Welcome Page</html>
```
## Sample Output 3
```
Error
```
## Explanation for Sample 3
> We can see that the starting tag `<title>` and the ending tag `</html>` are completely different, thus, returning an error.

## Sample Input 4
```
<h1>This has a bad ending tag<h1>
```
## Sample Output 4
```
Error
```
## Explanation for Sample 4
> We can see that the ending tag does not have a black slash, therefore, not closing the tags properly, returning an error.
