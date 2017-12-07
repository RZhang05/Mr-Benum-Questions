# Credit Card Validator
Use the [LUHN algorithm](https://en.wikipedia.org/wiki/Luhn_algorithm) to **verify credit card numbers**.

## Algorithm Explanation

Steps taken from [here](http://www.datageneratortools.com/card/calculator)
* `Calculate the Check Digit`
  * From the rightmost digit, which is the check digit, moving left, double the value of every second digit
  * If the product of this doubling operation is greater than 9, then sum the digits of the products or alternatively subtract 9 from the product.
  * Take the sum of all the digits.
  * Multiply by 9.
  * The last digit is the check digit.
  
* `Validate the Check Digit`
  * From the rightmost digit, which is the check digit, moving left, double the value of every second digit
  * if the product of this doubling operation is greater than 9,then sum the digits of the products or alternatively subtract 9 from the product.
  * Take the sum of all the digits.
  * If the total modulo 10 is equal to 0 then the number is valid according to the Luhn formula or else it is not valid.

## Sample Run

### User Console
```
Prompt: Please enter a credit card number
User: 371449635398431
```

### Output (expanded)
The blue values are the changed values.
```md
Step One doubling the values: *3* 14 *1* 8 *4* 18 *6* 6 *5* 6 *9* 16 *4* 6 *1* <- Check Digit

Step Two sum the digits:      *3* 5 *1* 8 *4* 9 *6* 6 *5* 6 *9* 7 *4* 6 *1* <- No digits above 10

Adding them up:               *3* + *5* + *1* + *8* + *4* + *9* + *6* + *6* + *5* + *6* + *9*
                              + *7* + *4* + *6* + *1* = 80
                              
Step Three modulo by 10:      *80* % *10* = 0

Result:                       The Pan Number is Valid

Computer Output: *371449635398431* is a valid number.
```
