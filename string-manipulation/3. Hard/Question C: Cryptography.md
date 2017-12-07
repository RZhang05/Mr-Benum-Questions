# Cryptography
Research a simple `encryption or decryption` algorithm (For example, a Base64 Java encoder/decoder) , or make one up your own. Create a program that will prompt the user for a **string** and then **ask** the user if they want to encrypt or decrypt. Output the resulting string.

## :bulb: Idea
Below is an explanation for the implementation of a Base64 Encoder in Java. Note that it is written in Pseudocode and you will still have to figure it out yourself. It's just a possibility!

### Base 64 Encoder
Important note: You will have to declare a main method that throws the `UnsupportedEncodingException`. The steps for the encoder follow below:
```java
imports required: javax.xml.bind.DatatypeConverter, java.io.UnsupportedEncodingException

Take in a string (no spaces) from the user
Ask whether the user would like to encrypt or decrypt

if encrypt {

    Use the printBase64Binary method of DatatypeConverter to encode the inputted string 
    from the user (note: the string should be changed to a byte array first)
    Output the value to the console
    
} else if decrypt {

    Use the parseBase64Binary method of DatatypeConverter to decode the inputted string from the user, 
    the result will have to be changed to a string
    Output the value to the console
    
}
```
### Console
Provided you have completed the above steps correctly you should see one of the two possible outcomes below:

ENCRYPTION
```
(comp) Enter a word:
(user) java
(comp) Would you like to Decrypt or Encrypt?
(user) Encrypt
(comp) Encryped value is    amF2YQ==
```

DECRYPTION
```
(comp) Enter a word:
(user) amF2YQ==
(comp) Would you like to Decrypt or Encrypt?
(user) Decrypt
(comp) decoded value is 	java
```
