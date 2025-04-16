# Grading Rubic
The students were asked to write a paragraph with the some requirements.

In the paragraph, students should inlcudes:

1. five different valid integers -- 4 points each. No more than 20 points
2. five different valid  decimals -- 4 points each. No more than 20 points
3. five different valid emails address -- 4 points each. No more than 20 points
4. five different valid price -- 4 points each. No more than 20 points
5. five different valide phone number -- 4 points each. No more than 20 points

For example: a studnet has 6 integers, 0 real numbers, 1 email addresses, 2 prices, 10 phone numbers.
His grade should be 20 + 0 + 4 + 4*2 + 20 = 52

## Hints:
You can use python regular expression to specify the patterns and find the matches. You have to figure out the correct patterns for each category.

## Integers 
Integers are whole numbers. They can be positive or negative.

The following are valid integers:
```
1234
9
-78
```
The following are not valid integers:
```
1a2b3c
nine
3.4
hello
2.5.7
```
## Decimals
The decimals have a whole number and a fractional part separated by a decimal point.

The following are valid decimals:
```
5.6
- 7.00
1.678943578976543
```

The following are not valid decimals:
```
3
-9
4.9.8
```
## Address
The addresses are a valid address begins with a positive integer and is followed by 
one or more words or abbreviations. The words or abbreviations must consist of only 
letters from the English alphabet, may only contain a capital letter as the first letter, 
and may or may not end in a period

The following are valid addresses:
```
1189 Beall Avenue
123 S. Main St.
456 Elm Ter.
88 Morning Sun
```
The following are not valid addresses:
```
Eight fifty two North Washington
10 10 Springfield Lane
14.5 S Main
12 S.Main
123 main street
```
## Price
Here a valid price is a numeric value using the US dollar sign. 
The number of cents is optional, but there must be two digits if 
the cents are shown. For prices above $999.99, there may optionally 
be a comma separating thousands, millions, etc.

The following are valid prices:
```
$1
$20
$1.99
$10.00
$1500.50
$2,000.99
$1,234,567.89
```
The following are not valid prices:
```
$1.9
$10,23.4
```
## Phone Number
Here a phone number is a valid US phone number with the area code (you don't have to check whether the area code is real or not). 
The final 7 digits must be separated by a hyphen, while the area code 
may be in parentheses or separated from the rest of the number by a hyphen. 
There may or may not be a single space between the closing parentheses and the fourth number.

The following are valid phone numbers:
```
(330) 263-2000
(330)263-2000
123-456-7890
```
The following are not valid phone numbers:
```
(123)4567890
456-7890
330 263-2000
```
## Email address
Capturing all the rules for what makes a valid email address is complex,
so we will use a simplified definition of a valid email address. 
This definition generally works just fine for extracting email addresses from documents.

The first part of the email address is the username portion, 
and it must not contain whitespace or the @ symbol. 
The username portion is followed by the @ symbol. 
After the @ symbol is the domain, which does not contain any whitespace or the @ symbol. 
The domain contains two or more non-empty components which are separated by periods. 
The final component must consist of only letters from the English alphabet.
The following are valid email addresses:
```
nsommer@wooster.edu
n.sommer@cs.wooster.edu
yippee_skippy@yee-haw.wheeeee
fun-times@Taylor.hall.wooster.edu
```
The following are not valid email addresses:
```
n@sommer@wooster.edu
n sommer@wooster.edu
nsommer@wooster..edu
nsommer@wooster.edu-org
```
