### Week 6 Regular Expressions Homework

### This is a template for the report of 21 problems on [this site](http://regextutorials.com/excercise.html).

### Fork this repository, change this file and send us the link for grading.

### We recommend you (re)watch our presentation, and use a [cheatsheet](./cheatsheet.md) while working on the following problems.

### If you are having problems with figuring out the correct solution, skip it for later, and if you are completely lost, use the hints and try to understand them.

---

### Problem 1: Floating point numbers
```
\d\.\d+
```
### Problem 2: Years before 1990
```
.+19[0-8][0-9].
```
### Problem 3: Hexadecimal colors
```
#[0-9A-F]{6}
```
### Problem 4: Grayscale colors
```
#([0-9a-fA-F]{1,2})\1\1
```
### Problem 5: Too long lines
```
.{30,}
```
### Problem 6: Remove repeating words
```
(\s.+)\1
$1
```
### Problem 7: Match HTML tags
```
<.?\w+\s?\w*>
```
### Problem 8: Cut numbers two digits after floating point
```
(\d\.\d{2})\d+
$1
```
### Problem 9: Digit commas formatting
```
(\d)(?=(\d{3})+\b)
$1,
```
### Problem 10: Match lowercase function declarations
```
function\s[a-z]+\w*\(.?\)
```
### Problem 11: Change date formats
```
(\d{4})-(\d{2})-(\d{2})
$3.$2.$1
```
### Problem 12: Validate 24h time format
```
([0-1]\d|2[0-3]):[0-5]\d
```
### Problem 13: Validate AM/PM time format
```
\b(0?\d|1[0-2]):[0-5]\d\s[A,P]M
```
### Problem 14: Pascal style to C-style parameters
```
;(\s\w)
,$1
```
### Problem 15: Change variable initialization
```
var\s*(\w*)\s=\s*new\s*((\w|<|>)+)
$2 $1
```
### Problem 16: IPv6 adresses
```
([0-9a-f]{0,4}:){1,7}[0-9a-f]{1,4}
```
### Problem 17: Validate 32 or 24 bit hexadecimal colors
```
(#[0-9a-f]{6}\b)|(#[0-9a-f]{8}\b)
```
### Problem 18: Replace operators with function calls
```
(\w[0-9a-z()*.]+)\s\+\s([0-9a-z()*.]+)
Add($1, $2)
```
### Problem 19: Extract query string from URL
```
(\w+=.+)|(\?)
```
### Problem 20: Extract host from URL
```
http://.+com
```
### Problem 21: Strings not containing word
```
Cake(.(?!chocolate))+$
```
