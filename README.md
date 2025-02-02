# jflnjnsn  
Expressing Numbers With Words:
A C♯ program for transforming numbers¹ in decimal² numeral³’⁴ form 
into English number words⁵ 

Jeffrey L. Johnson

Introduction 
In this program decimal numerals² in the form of digit strings with possible minus sign and
period are accepted as input.  These represent rational⁶ real⁷ numbers, and when affixed
with a minus sign, have a negative polarity.  Input expressions denoting integers contain
digits.  Decimal expression inputs will additionally contain a period.  The program then
computes a numeral⁴ in the form of an English compound⁸ noun⁹ such as "forty-five",
"minus three", or "zero point four five".  Latinate names--the building blocks for large
numbers--like billion, quadrillion, etc. are computed rather than being drawn from an
array, and so are unlimited in number and size, except for the constraints of the .NET
software framework and the hardware that it is running on.  Either short¹⁰ scale or long
scale¹⁰ values may be computed.  The short scale is used in the Anglosphere and elsewhere,
while the long scale is used in much of Europe.

The real numbers may be divided into three types: 1. integers,¹¹ a subtype of the rationals⁶.
2. non-integer rationals,⁶ and 3. irrationals.¹²  A rational number is one which can be defined
as the ratio of two integers.  Irrational numbers are those which cannot be so defined.
Non-integer rational⁴ numbers in turn are of two subtypes: a. decimal fractions,¹³ which can
be represented by a decimal expression with a finite number of digits,¹⁴ for example
1/4 = 0.25; and b. numbers which cannot be so represented, for example 1/3.  Specifically
the program takes inputs representing type 1 and type 2 numbers.  Expressions of the latter
type are inputted in the form of decimal expressions with a minus sign, an integer part, a
period, and a decimal part.  Examples: "minus (or negative) three" (aural only), and
"twenty-three million five hundred (and) forty thousand" (aural or written) respectively.
"and" may optionally be inserted.  The decimal fraction 25.974 is expressed as
"twenty-five point nine seven four" (aural only).                    

The mathematical concept of cardinality¹⁵ or size of a set underlies the cardinal numerals.¹⁶
Examples in English are: zero, nine, eighty-three, one thousand.  The mathematical concept 
of index of a sequence¹⁷ underlies the ordinal numerals.¹⁸  Examples in English are:
zeroth, ninth, eighty-third, one thousandth.  These may also be denoted as 0th, 9th, 83rd,
1,000th.  The program also outputs these forms.

Optional features are implemented for the expression of integers:
1. "and" may be inserted in various positions in the English expression.
E.g. 354,010,741 ⇒ "three hundred and fifty four million ten thousand
seven hundred and forty one.
2. 1 may conditionally be expressed as "a", e.g. 1,000 ⇒ "a thousand".
3. "hundred" may stand for "thousand"  For example,  "3656 ⇒
"thirty-six hundred (and) fifty-six", as opposed to "three thousand (and)
six hundred fifty-six".

Glossary
1. number
"A number is a mathematical object used to count, measure, and label. The most basic
examples are the natural numbers 1, 2, 3, 4, and so forth."
https://en.wikipedia.org/wiki/Number
2. decimal numeral system
"The decimal numeral system is the standard system for denoting integer and non-integer
numbers." "A decimal numeral (also often just decimal or, less correctly, decimal number),
refers generally to the notation of a number in the decimal numeral system."
https://en.wikipedia.org/wiki/Decimal

3. numeral system
"A numeral system is a writing system for expressing numbers; that is, a mathematical
notation for representing numbers of a given set, using digits or other symbols in a consistent
manner."
https://en.wikipedia.org/wiki/Numeral_system

4. numeral
"In linguistics, a numeral in the broadest sense is a word or phrase that describes a
numerical quantity."
https://en.wikipedia.org/wiki/Numeral_(linguistics)

5. English number word
"English number words include numerals and various words derived from them, as well as
a large number of words borrowed from other languages."
https://en.wikipedia.org/wiki/English_numerals

6. rational number
"a rational number is a number that can be expressed as the quotient or fraction p/q of
two integers, a numerator p and a nonzero denominator q."
https://en.wikipedia.org/wiki/Rational_number                  

7. real number
"a real number is a number that can be used to measure a continuous one-dimensional
quantity such as a distance, duration or temperature."
https://en.wikipedia.org/wiki/Real_number 
https://en.wikipedia.org/wiki/Numeral_(linguistics)

8. compound
"In linguistics, a compound is a lexeme (less precisely, a word or sign) that consists
of more than one stem."
https://en.wikipedia.org/wiki/Compound_(linguistics)

9. noun
"In grammar, a noun is a word that represents a concrete or abstract thing, such as
living creatures, places, actions, qualities, states of existence, and ideas."
https://en.wikipedia.org/wiki/Noun

10. short scale and long scale
https://en.wikipedia.org/wiki/Long_and_short_scales 

11. integer
"An integer is the number zero (0), a positive natural number (1, 2, 3, etc.) or a
negative integer (−1, −2, −3, etc.)"
https://en.wikipedia.org/wiki/Integer
"integer
1. A member of the set of positive whole numbers {1, 2, 3, … },
negative whole numbers {−1, −2, −3, … }; or 0.
2. A complete unit or entity.
3. An entire entity; particularly, in arithmetic, a whole number, in contradistinction to a fraction.
Thus, in the number 54.7, 54 is an integer, and .7 a fraction (seven tenths of a unit).
4. A complete entity; a whole number, in contradistinction to a fraction or a mixed number.
5. An expression of the form a + b√-1, where a and b are real integers.
6. Any of the natural numbers (positive or negative) or zero."
The American Heritage® Dictionary of the English Language, 5th Edition
Note: The  equation z = a + b√-1, where a, b are real numbers, is the general formula for
generating complex numbers z." 
See: https://en.wikipedia.org/wiki/Complex_number

12. irrational number
"In mathematics, the irrational numbers are all the real numbers that are not
rational numbers. That is, irrational numbers cannot be expressed as the ratio of
two integers."
https://en.wikipedia.org/wiki/Irrational_number

13. decimal fraction
"Decimal fractions (sometimes called decimal numbers, especially in contexts
involving explicit fractions) are the rational numbers that may be expressed as a
fraction whose denominator is a power of ten."
https://en.wikipedia.org/wiki/Decimal#Decimal_fractions

14. numerical digit (or digit)
"A numerical digit (often shortened to just digit) is a single symbol used alone
(such as "1") or in combinations (such as "15"), to represent numbers in a positional
numeral system."
https://en.wikipedia.org/wiki/Numerical_digit
15. cardinality
"In mathematics, the cardinality of a set is a measure of the number of elements of the set.
For example, the set A = { 2, 4, 6 } contains 3 elements, and therefore A has a cardinality of 3."
https://en.wikipedia.org/wiki/Cardinality

16. cardinal numeral
"In linguistics, and more precisely in traditional grammar, a cardinal numeral
(or cardinal number word) is a part of speech used to count. Examples in English
are the words one, two, three, and the compounds three hundred [and] forty-two and
nine hundred [and] sixty." 
https://en.wikipedia.org/wiki/Cardinal_numeral
"Cardinal numbers refer to the size of a group. In English, these words are numerals."
https://en.wikipedia.org/wiki/English_numerals#Cardinal_numbers
"In mathematics, a cardinal number, or cardinal for short, is what is commonly called
the number of elements of a set. In the case of a finite set, its cardinal number, or
cardinality is therefore a natural number."
https://en.wikipedia.org/wiki/Cardinal_number

17. sequence
"In mathematics, a sequence is an enumerated collection of objects in which
repetitions are allowed and order matters."
https://en.wikipedia.org/wiki/Sequence

18. ordinal numeral
"In linguistics, ordinal numerals or ordinal number words are words representing
position or rank in a sequential order; the order may be of size, importance, chronology,
and so on (e.g., "third", "tertiary")."
https://en.wikipedia.org/wiki/Ordinal_numeral
"Ordinal numbers refer to a position (also called index or rank) in a sequence." "zeroth,
ninth, eighty-third"
https://en.wikipedia.org/wiki/English_numerals#Ordinal_numbers
"In set theory, an ordinal number, or ordinal, is a generalization of ordinal numerals
(first, second, nth, etc.) aimed to extend enumeration to infinite sets."
https://en.wikipedia.org/wiki/Ordinal_number 
