# Strings Lab 1

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

Write code that prints out all the numbers from 1 to 10 as a single string.
(Hint: the `String()` function can convert an Int to a String)

***
```
var num = 10
var i = 0

while i < num  {
i += 1
print("This a string now", String(i))
}
```
## Question 2

Write code that prints out all the even numbers from 5 to 51 as a single string.

***
```
var num = 52
var i = 4
//var line = String()
var line = "All the numbers are even "

while i < num  {
i += 1
if i % 2 == 0 {

line.append("\(i)" + " ")

}

}
print("\(line)")
```
## Question 3

Write code that prints out every number ending in 4 between 1 and 60 as a single string.

***
```
var num = 61
var i = 0
//var line = String()
var line = "All the numbers are even "

while i < num  {
i += 1
if i % 10 == 4 {

line.append("\(i)" + " ")

}

}
print("\(line)")
```
## Question 4

Print each character in the string `"Hello world!"`

***
```
for c in "Hellow World!"{
print(c)
}
```
## Question 5

Print out the last character in the string below.  You cannot use the Character literal "!" (i.e you must access `myStringSeven`'s characters).

`var myStringSeven = "Hello world!"`

***
```
var myStringSeven = "Hello world!
print(myStringSeven.removeLast())
```
## Question 6

Write code that switches on a string, given the following conditions:
- If the string's length is even, print out every character.
- If the string's length is odd, print out every other character.

***

```
var strings = "Test run"
var stringL = strings.count
var empty = 0


if stringL % 2 == 0{
print(strings)
}
else {
for i in strings{
if empty % 2 == 0 {
print(i)
}
empty += 1
}
}
```
## Question 7

Initialize a String with a character. Show that it is a Character, and not another String, that you're using to initialize it.

```
var newString: String = "A"
var string = Character(newString)
print(string)
```

***

## Question 8

Build five pairs of **canonically equivalent** strings, the first of each being a pre-composed character and the second being one that uses combinable unicode scalars. Show that they are equivalent.

```
var test1 = "Test!"
var test2 = "T\u{0065}st!"
var test3 = "Te\u{0073}t!"
var test4 = "Tes\u{0074}!"
var test5 = "Test\u{0021}"

if test1 == test2 && test1 == test3 && test1 == test4 && test1 == test5{
print("True")
}

```
***
## Question 9

**Using only Unicode**, print out `"HELLO WORLD!"`
```
print("\u{0022}\u{0048}\u{0045}\u{004c}\u{004c}\u{004f}\u{0020}\u{0057}\u{004f}\u{0052}\u{004c}\u{0044}\u{0021}\u{0022}\u{0020}")
```
***
## Question 10

**Using only Unicode**, print out your name.

```
print("\u{0045}\u{0072}\u{0069}\u{0063}\u{0020}\u{004d}\u{0065}\u{0069}")
```
***
## Question 11

**Using only Unicode**, print out `"HELLO WORLD!"` in another language.
```
print("\u{004f60}\u{00597d}\u{00ff0c}\u{004e16}\u{00754c}")
```

***
## Question 12

Print the below flower box using the following information.

- The unicode number for ⚘ is U-2698
- The top and bottom of the box are represented by dashes and the rows are |
- Use the terminator argument in your print statements to print on the same line.
- Hint: It may be useful to try printing out a box of just one character to start then work your way from there.

```swift
Flower Box:
- - - - - - - - - - -
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
- - - - - - - - - - -
```

***
## Question 13

Write a program that sets up a chess board using Unicode.

```swift
Chess Board:
♖ ♘ ♗ ♕ ♔ ♗ ♘ ♖
♙ ♙ ♙ ♙ ♙ ♙ ♙ ♙




♟ ♟ ♟ ♟ ♟ ♟ ♟ ♟
♜ ♞ ♝ ♛ ♚ ♝ ♞ ♜
```

***
## Question 14

You are given a string stored in the variable `aString`. Create new string named `replacedString` that contains the characters of the original string with all the occurrences of the character `"e"` replaced by `"\*"`.

```swift
var aString = "Replace the letter e with \*"
// Your code here
 ```
```
let string = "replacedString"
let newString = string.replacingOccurrences(of: "e", with: "*")
print(newString)
```

Example:

Input:
`var aString = "Replace the letter e with *"`

Expected values:
`replacedString = "R*plac* th* l*tt*r * with *"`

***
## Question 15

You are given a string stored in variable `aString`. Create a new string called `reverse` that contains the original string in reverse order. Print the reversed string.

```swift
var aString = "this string has 29 characters"
var reverse = ""

// Your code here
```
```
var myString = "NEED FOOD"
print(String(myString.reversed()))
```

Example:
Input:
`var aString = "Hello"`

Output:
`"olleH"`

***
## Question 16

You are given a string stored in variable `aString`. Print `true` if `aString` is a palindrome, and `false` otherwise. A **palindrome** is a string which reads the same backward or forward.

```swift
let aString = "anutforajaroftuna"

// Your code here
```
```
var aString = "RATS STAR"
var test = (String(aString.reversed()))

if test == aString{
print("true")
}
```

Example 1:
Input:
`var aString = "anutforajaroftuna"`

Output:
`true`

Example 2:
Input:
`var aString = "Hello"`

Output:
`false`

***
## Question 17

You are given a string stored in variable `problem`. Write code so that you print each word of the string on a new line.

```swift
var problem = "split this string into words and print them on separate lines"

// Your code
```
```
var problem = "split this string into words and print them on separate lines"
var seperate = problem.components(separatedBy: (" "))
print(seperate)
```

Example:
Input:
`var problem ="split this string into words and print them on separate lines"`

Output:
```swift
split
this
string
into
words
and
print
them
on
separate
lines
```

***
## Question 18

You are given a string stored in variable `problem`. Write code that prints the longest word in the string.

```swift
var problem = "find the longest word in the problem description"

// Your code here
```

Example:
Input:
`var problem = "find the longest word in the problem description"`

Output:
`description`

Hint: Keep track of the longest word you encounter and also keep track of its length.

***
## Question 19

Given a string in English, create a tuple containing the number of vowels and consonants.

```swift
let vowels = "aeiou"
let consonants = "bcdfghjklmnpqrstvwxyz"
let input = "Count how many vowels I have!"
```

***
## Question 20

Given a string of words separated by a `" "`. Write code that prints out the length of the last word.

If there is no last word print out `"No last word"`.

Example:
Input: `"How are you doing this Monday?"`

Output: `7`

***
