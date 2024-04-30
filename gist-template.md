# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary
The following code will be used and explained throught this tutorial. Regex or Regular Expressions is specified set of charaacters that are used to identify a desired string. Often, they are used to check if an inputted string fits the context in which it has been submitted throughout the code. To have a valid regex hexadecimal or "hexcode" will have to satisfy the following conditions.
It should start from the "#" symbol.
It should be followed by the letters from a-f, A-F and /or digits from 0-9.
the length of the hexadecimal color code should be either 6 or 3, excluding the "#" symbol.
Here we will break down and explain the following code.

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

The code above is used to match hex values aka color code!

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components

### Anchors
^ $

The following expressions above are known as anchors or assertions in an expression. They mark the beginning and/or ending of a regular expression which is written within two forward slashes 
(/expression/). 

^#
this part of the expression will match a string that begins with the "#". 
the "#" symbol represents the hexadecimal color code must start with the "#" symbol which represents the start of a group.

### Quantifiers

{6} {3}

The part of the expression above is known as the Quantifiers. The word Quantify comes from the latin quantus, whic means "how much". When the -ers are added we know that we are working with a group of nouns. Whic means the quantifier will tell us how much is needed.

As listed in the summary above the following numbers are the only two numbers that can be listed. 
Why you might ask?

Its because the length of each code is 6 characters without the "#" symbol. Plain hexcodes already quantify how much of a color we want. in normal hexcodes the first two characters represent the amount of red, the next two represent the amount of green, and the final two represnt the amoint of blue for example (#RRGGBB). Since hexcode is 6 characters long the {6} is specified to match a string that matches a character class that is exactly 6 characters long. Since we are working with computer intelligence it will be precise.

Within the rgb values , the numerical portion of the code represents the span between 0-255. Since we are only working with 16 base. We can make use of letters to signify the value as well.


### OR Operator
|

The following syntax in the expression is known as the OR operator which is much like the pipe operator in javascript. The OR operator adds an option in the regex. Since we are searching for a 6 character code that includes lowercase letters a-f and numbers 0-9 in our beginning line of code. The OR operator states that we are looking for anything within both groups meaning. We want a 6 character code that has lowercse letters a-f and numbers 1-9 "OR" a 3 character code with lowercase letters a-f with numbers 1-9. 


### Character Classes
[a-f0-9] 

the following part of expression is called the Character class which is the characters listed inside of the square brackets. This tells the regex which characters should be matched.

This specific set of characters signifies that we want to match a lowercase a-f along with the numbers 0-9 nothing more nor less. These are case sensitive, so be positive to include the correct case intended in order to be searched correctly. This particular regex will search for lowercase letters.

Keep in mind that hexcodes can also be written with capital letters as well. 

### Flags

Even though regex is considered a literal, flags are a component that can add onto the functionality or limits for the regex. normally, there are 6 optional flags that can be utilized, either together in any order or all seperately. The most common flags to come across are listed below.

g- Global search: the regex should be tested against all possible matches in a string.

i- Case sensitve search: letter casing should be ignored while trying to find a match in a string.

### Grouping and Capturing
()

The fllowing parenthesis "()" are used for the grouping method within the expression. This helps group multiple tokens together and creates a caupture group for extracting a substring or using a back refrence. This allows us to seperate meta characters from the literal characters. Grouping can also be used to isolate part of a string or data in a program.

### Bracket Expressions
[]

The follwoing syntax of the expression are known as bracket expressions. These are used to show what characters are matched with the regex. 
For example.
[a-f] This means the string can contain any lowercse letters between a-f.
[0-9] This means that the string can contain any number between 0-9.
{6} this means that the characters can be 6 characters long.
|{3} this means that we will also accepts a code that is 3 characters long.

### Greedy and Lazy Match
?

the following syntax is a symbol of lazy or greedy matching. Greedy matching means to match the longest possible string, while lazy matching means to match the opposite or the shortest possible string.
for example

w.+l matches well in well but the lazy w.+?l matches wel.
 
 the ? indicates to match the shortest possible string so in our code this would be a lazy matching expression.


## Author

Hello my name is Sean Brown and I am currently in the process of becoming a junior developer. I am taking a leap and making a career change from the oilfield. i enkoy what i am learning currently i mainly like the front end part of development and in need of more practice on the backend. I am excited for a change and enjoy building and designing sites/ applications. You may reach my repositories from my profile. 
https://github.com/Crlyhdfrd
