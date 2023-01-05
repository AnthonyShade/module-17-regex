# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary
 This tutorial will dive into the Regex Email expression of `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,5})$/`.  This expression is able to match email needed for verification, examples of this format would be middle.LastName123@email.com, anythingword@domain.com, and so on.  The following sections of this piece will examine the various compents of a Regular Expression and how they are used. 
 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors
^ matches the beginning of the string
$ matches the end of the string$

### Quantifiers
{2,6}

### Grouping Constructs
creates a capture group for extracting a substring or using a backreference
### Bracket Expressions
[] Any characters specified between the opening and closing brackets will be searched | ````[C]a[tr]```` means any matching strings that have ````C```` followed by an ````a```` then a ````t```` or a ````r```` like : ````Car```` or ````Cat````|````[a-z0-9_\.-]```` means any matching with ````a-z0-9_\.-````
[-] Specifies any matching within the range of characters (character on the left side of the hypen ````-```` is the start of the range and the character on the right side of the hypen specifies the end of the range) | ````[a-z]```` means any matching character between letter ````a```` in small caps and ````z```` in small caps (including ````a```` and ````z````) / ````[0-9]```` means any matching integer between ````0```` and ````9```` (including ````0```` and ````9````) | ````[a-z0-9_\.-]```` an any matching characters between ````a```` and ````z````, ````0```` and ````9````. The remaining characters will be explained in the following sections. 

### Character Classes
^  Beginning.  Matches the beginning of the string, or the beginning of a line if the multiline flag (m) is enabled. This matches a position, not a character.
(  Capturing Group 1.  Groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.
[  Character set. Match any character in the set.
a-z  Range.  Matches a character having a character code between the two specified characters inclusive. Case Sensitive.
0-9  Range.  Matches a character in the range "0" to "9". Case sensitive.
_  Character.  Matches a "_" character (char code 95).
\.  Escaped character. Matches a "." character (char code 46).
-  Character.  Matches a "-" character (char code 45).
]
+  Quantifier.  Match 1 or more of the preceding tokens.
)
@  Character.  Matches a "@" character (char code 64).
(  Capturing Group #2.  Groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.
[  Character set. Match any character in the set.
\d  Digit. Matches and digit character (0-9).
a-z  Range. Matches a character in the range "a" to "z" (char code 97 to 122). Case sensitive.
\.  Escaped character.  Matches a "." character (char code 46).
-  Character. Matches a "-" character (char code 45).
]
+  Quantifier.  Match 1 or more of the preceding token.
)
\.  Escaped character.  Matches a "." character (char code 46).
(  Capturing group #3.  Groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.
[  Character set. Match any character in the set.
a-z  Range. Matches a character in the range "a" to "z" (char code 97 to 122). Case sensitive.
\.  Escaped character.  Matches a "." character (char code 46).
]
{2,6} Quantifier.  Match between 2 and 6 of the preceding token.
)
$  End.  Matches the end of the string , or the end of a line if the multiline flag (m) is enabled.

### The OR Operator

### Flags
changes how the expression is interpreted 
### Character Escapes

## Author
github.com/AnthonySHade
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)