/* ENWW-express all forms version
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
End of Introduction
---------------------------------------------------------
Guide to selected methods, with aliases, and the array s_shortScaleIlliNames
GetEnglishNumeral
This is the main method.

GetLatinateCardinalNumeralFor10ToPowerMultipleOf3
TheLatinateIlliNameFor10ToPowerMultipleOf3
ulong ⇒ string 
The central method for producing "illi" names, such as "million", "quadrillion", etc.
The input is an index, where 0 ⇒ "thousand", 1 ⇒ "million", 2 ⇒ "billion" (short scale), etc.

TheConcatenationOf
string/array ⇒ string
Strings together a sequence of characters, integers, strings or arrays.
Indirectly calls ConcatenateTwoCharacterArrays, which utilizes the System method
Buffer.BlockCopy.

GetEnglishCardinalNumeralForInteger
TheEnglishCardinalNumeralForTheInteger
strings, bool ⇒ string
This is the main method for generating integers.

 s_shortScaleIlliNames
This is an array of 1201 illion names used for checking the output of the latinate
"illion name" generator, which produces words like "billion", "quadrillion", etc.                     */

using System;
using static System.Array;
using static System.Buffer;
using System.Collections;
using System.Collections.Generic;
using static System.Console;
using static System.ConsoleColor;
using System.Diagnostics;
using static System.Environment;
using System.Linq;
using System.Linq.Expressions;
using static System.Math;
using static System.String;
// For StringBuilder.
using System.Text;
using System.Text.RegularExpressions;
using static ExpressionOfNumbersInEnglish.NumberExpression;
using static ExpressionOfNumbersInEnglish.StringAndArrayProcessing;
using System.Xml.Linq;
using static System.Runtime.InteropServices.JavaScript.JSType;
using System.Net.NetworkInformation;
using System.Diagnostics.Metrics;
//using static ExpressionOfNumbersInEnglish.ControlOfTimedInteractionWithUsers;
// Use expression body for methods (IDE0022)
// Re: https://learn.microsoft.com/en-us/dotnet/fundamentals/code-analysis/style-rules/ide0022
#pragma warning disable IDE0022
// Use conditional expression for return
#pragma warning disable IDE0046
// Use expression body for local functions
#pragma warning disable IDE0061
// Naming Styles
#pragma warning disable IDE1006
// Top-level statements: 
// This calls the main method.
GetEnglishNumeral(); // abcdefghijkl
//var L1 = ThePowerSetOf("abc"); WriteLine("L1.Count" + L1.Count()); Wait(3);
////for (var i = 0; i <  4096; i++)
//foreach(string str in L1)
//{
//    WriteLine(str); Wait(1);
//}
//
//
//39);
namespace ExpressionOfNumbersInEnglish
{
    // See: https://learn.microsoft.com/en-us/dotnet/standard/exceptions/how-to-create-user-defined-exceptions
    public class NullOrEmptyException : Exception
    {
        public NullOrEmptyException() { }
        public NullOrEmptyException(string message) : base(message) { }
        public NullOrEmptyException(string message, Exception inner)
            : base(message, inner) { }
    }
    public static class NumberExpression
    {
/*     The static keyword should be applied to all members of static classes.
        https://learn.microsoft.com/en-us/dotnet/csharp/misc/cs0708?f1url=%3FappId%3Droslyn%26k%3Dk(CS0708)
        Pascal case used for public fields per:
        https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions
        "A public field, these should be used sparingly"
        Use camel casing ("camelCasing") when naming private or internal fields.
        Static fields are prefixed with s_.
        See https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names
        When naming public members of types, such as fields, properties, events, use pascal casing. 
        https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names               
        const identifiers use Pascal case.                                                                                                           
        A field declared without the static modifier is an instance variable.
        https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/language-specification/variables             */
        public const char
        NullCharacter = '\u0000',
        Space = '\u0020',
        DoubleQuote = '\u0022',
        Hyphen = '\u002d',
        MinusSign = '\u002d',
        Period = '\u002e',
        Zero = '\u0030',
        Backslash = '\u005c',
        Enter = (char)13;  // or (char)ConsoleKey.Enter; 
        public const string
        CommaString = ",",
        HyphenString = "-",
        MinusSignString = "-",
        PeriodString = ".",
        SpaceString = " ",
        ControlCharacters = "[^\x20-\x7F]",
        NonzeroDigits = "123456789",
        Digits = "0123456789";
        public static readonly string
        s_lowerCaseLetters = "abcdefghijklmnopqrstuvwxyz",
        s_upperCaseLetters = s_lowerCaseLetters.ToUpper(),
        s_letters = s_lowerCaseLetters + s_upperCaseLetters,
        /*     Not included are the alt key (Windows); the option and command keys (Apple); 
                and page up, page down, control, shift, tab, and space bar.                                                   */
        s_keyboardSymbols =
            "~`!@#$%^&*()-_=+[{]}|;:',<.>/?" + DoubleQuote + Backslash,
        // These number 68.
        s_keyboardCharacters = TheConcatenationOf(s_keyboardSymbols, Digits, s_letters),
        s_nondigitalCharacters = TheConcatenationOf(s_letters, s_keyboardSymbols,
                                                        NullCharacter, Space, ControlCharacters);
        #region s_shortScaleIlliNames       
/*     This array is not referenced in the program, and is only for reference
        and testing.
        -illion names are here given values in the "Short scale", as used in 
        Brazil and in most English-speaking and Arabic-speaking countries. 
        See https://en.wikipedia.org/wiki/Names_of_large_numbers and
        https://en.wikipedia.org/wiki/Long_and_short_scales#Short_scale
        This array uses the scheme invented by Nicolas Chuquet and extended
        in the Conway-Wechsler system.  
        See http://www.mrob.com/pub/math/largenum.html#chuquet
        and http://www.mrob.com/pub/math/largenum.html#conway-wechsler

        These names, except for "thousand", accord with the values given at
        https://kyodaisuu.github.io/illion/#list in the column headed
        "Conway-Wechsler system".

        Also see http://lcn2.github.io/mersenne-english-name/tenpower/tenpower.html
        https://kyodaisuu.github.io/illion/conway.html (compute name for any index)
        and https://kyodaisuu.github.io/illion/10000.html
        for lists of these names.

        At https://www.justintools.com/numbers/numbers-charts-tables.php and
        https://simple.wikipedia.org/wiki/Names_of_large_numbers
        name "Millinillion" is given for 10³⁰⁰³.  At this site Greek-based large
        number groups are listed: micrillion (from μικρός: "small), nanillion
        (from  νᾶνος: "dwarf"), mecillion (from μῆκος: "length")
        Nullable array of non-nullable element types                                                            */
        private static readonly string[]? s_shortScaleIlliNames = new string[1201]
        {                                                                                                                                  /*
            The etymological information here is from Latin, except as noted.
                                                                                Short scale
                                                                   3 × (Index + 1)       (Power / 3) - 1
      Number group name                              Power of 10               Index
           Illi name                                     No. of 0's following 1                                                                                                         
                  ⬇                                                       ⬇                          ⬇
            Late Old English; from "hund" ‘hundred’, from Proto-Germanic *hundą ('hundred') +
            *radą ('count'), a neuter variant of *radō ('row, line, series').    
            "hundred"                                                  2                            -                                                                                                                    
            Old English "thūsend", from Proto-Germanic þūsundī.                                                               */
            "thousand", //                                             3                            0   
/*         Old French; probably from Italian "milione", from "mille": 'thousand'.
            + the Italian augmentative suffix "-one".                                                                                      */
            "million", //                                                6                            1
/*         Early modern French; from million, 
            derived by substituting a prefix derived from Latin "bis": 'twice''.                                              */
            "billion", //                                                 9                            2
/*         Early modern French, from million, 
            derived by substituting a prefix derived from the Latin "tres" 'three'.                                         */
            "trillion", //                                               12                            3
/*         Early modern French; from million,  derived by substituting a prefix derived from the Latin 
            "quadrus 'a square'.  Cf. Latin "quattuor" 'four' and "quartus" 'fourth'.                                                          */
            "quadrillion", //                                        15                            4
/*         Early modern French; from million, derived by substituting the prefix "quint-", 
            from the Latin "quintus" ‘the fifth’).                                                                                              */
            "quintillion", //                                         18                            5
/*         The following -illion names are beyond the range of the integer type ulong
            (0 to 18.447 quintillion). However this program treats numbers using strings or 
            arrays, not integers, and these names are deployed.         
            Early modern French; from million, by substituting the prefix the Latin "sextus", 'sixth'.      */
            "sextillion", //                                           21                            6
            // Early modern French; from million, by substituting the root of Latin "septem" 'seven'.
            "septillion", //                                           24                            7
/*         Early modern French.  Shortening in English of (Latin) "octingenti": 'eight', 
            appended (as below) to -illion".                                                                                                  */
            "octillion", //                                             27                            8
            // Early modern French.  From "novem": 'nine'.
            "nonillion", //                                           30                             9
            // Root of "decem": 'ten'
           "decillion", //                                            33                           10
           // From "undecim": 'eleven'. 
           "undecillion", //                                        36                           11
            // From "duodecim": 'twelve'.
            "duodecillion", //                                     39                          12
            // From "tredecim": 'thirteen'.
            "tredecillion", //                                       42                          13
            // From "quattuordecim": 'fourteen'.
            "quattuordecillion", //                              45                          14
            // From "quinque": 'five'.                                         
            "quindecillion", //                                    48                          15
            // From "sedecim": 'sixteen'. 
            "sedecillion", //                                        51                          16           
            // From "septendecim": 'seventeen'. 
            "septendecillion", //                                 54                          17
/*         Cf. "octingenti": 'eight', "duodeviginti": 'eighteen'  (counts backward from twenty), 
            and "octoginta": 'eighty'.                                                                                 */
            "octodecillion", //                                     57                          18
/*         Cf. "novem": 'nine'. Labial 'm' changed to palatal 'n' in English  
            to provide phonetic consonance with the consonant which follows it.
            Such consonant consonance occurs throughout in names given below.            */
            "novendecillion", //                                  60                          19
            // From "viginti": 'twenty'. 
            "vigintillion", //                                        63                          20
/*         Cf. "viginti unum": 'twenty-one'. 
            Note that consonant consonance is not imposed on "un-",
            so "umvigintillion": not used.                                                                    */
            "unvigintillion", //                                    66                          21
            // Cf. "viginti duo": 'twenty-two'.
            "duovigintillion", //                                  69                          22
            // Cf. "viginti tres": 'twenty-three'.
            "tresvigintillion", //                                  72                          23
            // Cf. "viginti quattuor": 'twenty-four'.
            "quattuorvigintillion", //                           75                          24
            // Cf. "viginti quinque": 'twenty-five'.
            "quinvigintillion", //                                 78                         25
            // Cf. "viginti sex": 'twenty-six'.
            "sesvigintillion", //                                    81                         26
/*         Cf. "viginti septem": 'twenty-seven'.    
            Note that 'm' and 'v' are both labial,
            so no consonant adjustment of 'm': made.                                                */
            "septemvigintillion", //                             84                          27
            // Cf. "viginti octo": 'twenty-eight'.
            "octovigintillion", //                                 87                          28
            // Cf. "viginti novem": 'twenty-nine'.
            "novemvigintillion", //                             90                          29
            // Cf. "triginta": 'thirty'.
            "trigintillion", //                                        93                          30
            "untrigintillion", //                                    96                          31
            "duotrigintillion", //                                  99                          32
            "trestrigintillion", //                                102                          33
            "quattuortrigintillion", //                         105                         34
            "quintrigintillion", //                               108                          35
            "sestrigintillion", //                                 111                          36
            "septentrigintillion", //                           114                          37
            "octotrigintillion", //                               117                         38
            "noventrigintillion", //                            120                         39
            // Cf. "quadraginta": 'forty'.
            "quadragintillion", //                               123                         40
            "unquadragintillion", //                           126                         41
            "duoquadragintillion", //                         129                         42
            "tresquadragintillion", //                         132                         43
            "quattuorquadragintillion", //                  135                         44
            "quinquadragintillion", //                        138                         45
            "sesquadragintillion", //                          141                         46
            "septenquadragintillion", //                     144                         47  
            "octoquadragintillion", //                        147                         48
            "novenquadragintillion", //                     150                         49
            // Cf. "quinquaginta": 'fifty'.
            "quinquagintillion", //                             153                         50
            "unquinquagintillion", //                         156                         51
            "duoquinquagintillion", //                       159                         52
            "tresquinquagintillion", //                       162                         53
            "quattuorquinquagintillion", //               165                         54
            "quinquinquagintillion", //                     168                          55
            "sesquinquagintillion", //                       171                          56
            "septenquinquagintillion", //                  174                          57
            "octoquinquagintillion", //                     177                          58
            "novenquinquagintillion", //                  180                          59
            // Cf. "sexaginta": 'sixty'.
            "sexagintillion", //                                  183                          60
            "unsexagintillion", //                              186                          61
            "duosexagintillion", //                            189                          62
            "tresexagintillion", //                              192                          63
            "quattuorsexagintillion", //                     195                          64
            "quinsexagintillion", //                           198                          65
            "sesexagintillion", //                               201                          66
            "septensexagintillion", //                        204                          67
            "octosexagintillion", //                           207                          68
            "novensexagintillion", //                        210                          69
            // Cf. "septuaginta": 'seventy'.
            "septuagintillion", //                               213                          70
            "unseptuagintillion", //                           216                          71
            "duoseptuagintillion", //                         219                          72
            "treseptuagintillion", //                           222                          73
            "quattuorseptuagintillion", //                  225                          74
            "quinseptuagintillion",  //                       228                          75
            "seseptuagintillion", //                            231                          76
            "septenseptuagintillion", //                     234                          77
            "octoseptuagintillion", //                        237                          78
            "novenseptuagintillion", //                     240                          79
            // Cf. "octoginta": 'eighty '.
            "octogintillion", //                                  243                          80
            "unoctogintillion", //                              246                          81
            "duooctogintillion", //                            249                          82
            "tresoctogintillion", //                            252                          83
            "quattuoroctogintillion", //                     255                          84
            "quinoctogintillion", //                           258                          85
            "sexoctogintillion", //                             261                          86
            "septemoctogintillion", //                       264                          87
            "octooctogintillion", //                           267                          88
            "novemoctogintillion", //                       270                          89
            // Cf. "nonaginta": 'ninety'.
            "nonagintillion", //                                 273                          90
            "unnonagintillion", //                             276                          91
            "duononagintillion", //                           279                          92
            "trenonagintillion", //                             282                          93
            "quattuornonagintillion", //                    285                          94
            "quinnonagintillion", //                          288                          95
            "senonagintillion", //                              291                          96
            "septenonagintillion", //                         294                          97
            "octononagintillion", //                          297                          98
            "novenonagintillion", //                         300                          99
            // Cf. "centum": 'one hundred'.
            "centillion", //                                         303                        100
            "uncentillion", //                                     306                        101
            "duocentillion", //                                   309                        102
            "trescentillion", //                                   312                        103
            "quattuorcentillion", //                            315                        104
            "quincentillion", //                                  318                        105
            "sexcentillion", //                                    321                        106
            "septencentillion", //                               324                        107
            "octocentillion", //                                  327                        108
            "novencentillion", //                               330                        109
            "decicentillion", //                                  333                        110
            "undecicentillion", //                              336                        111
            "duodecicentillion", //                            339                        112
            "tredecicentillion", //                              342                        113
            "quattuordecicentillion", //                     345                        114
            "quindecicentillion", //                           348                        115
            "sedecicentillion", //                               351                        116
            "septendecicentillion", //                        354                        117
            "octodecicentillion", //                           357                        118
            "novendecicentillion", //                        360                        119
            "viginticentillion", //                              363                        120
            "unviginticentillion", //                          366                        121
            "duoviginticentillion", //                        369                        122
            "tresviginticentillion", //                        372                        123
            "quattuorviginticentillion", //                 375                        124
            "quinviginticentillion", //                       378                        125
            "sesviginticentillion", //                         381                        126
            "septemviginticentillion", //                   384                        127
            "octoviginticentillion", //                       387                        128
            "novemviginticentillion", //                   390                        129
            "trigintacentillion", //                             393                        130
            "untrigintacentillion", //                         396                        131
            "duotrigintacentillion", //                       399                        132
            "trestrigintacentillion", //                       402                        133
            "quattuortrigintacentillion", //                405                        134
            "quintrigintacentillion", //                      408                        135
            "sestrigintacentillion", //                        411                        136
            "septentrigintacentillion", //                   414                        137
            "octotrigintacentillion", //                      417                        138
            "noventrigintacentillion", //                   420                        139
            "quadragintacentillion", //                      423                        140
            "unquadragintacentillion", //                  426                        141
            "duoquadragintacentillion", //                429                        142
            "tresquadragintacentillion", //                432                        143
            "quattuorquadragintacentillion", //         435                       144
            "quinquadragintacentillion", //               438                       145
            "sesquadragintacentillion", //                 441                       146
            "septenquadragintacentillion", //            444                       147
            "octoquadragintacentillion", //                447                       148
            "novenquadragintacentillion", //             450                       149
            "quinquagintacentillion", //                     453                       150
            "unquinquagintacentillion", //                 456                       151
            "duoquinquagintacentillion", //               459                       152
            "tresquinquagintacentillion", //               462                       153
            "quattuorquinquagintacentillion", //       465                        154
            "quinquinquagintacentillion", //             468                        155
            "sesquinquagintacentillion", //               471                        156
            "septenquinquagintacentillion", //          474                        157
            "octoquinquagintacentillion", //             477                        158
            "novenquinquagintacentillion", //          480                        159
            "sexagintacentillion", //                          483                       160
            "unsexagintacentillion", //                      486                       161
            "duosexagintacentillion", //                    489                       162
            "tresexagintacentillion", //                      492                       163
            "quattuorsexagintacentillion", //             495                       164
            "quinsexagintacentillion", //                    498                      165
            "sesexagintacentillion", //                        501                      166
            "septensexagintacentillion", //                 504                      167
            "octosexagintacentillion", //                    507                      168
            "novensexagintacentillion", //                 510                      169
            "septuagintacentillion", //                       513                       170
            "unseptuagintacentillion", //                   516                        171
            "duoseptuagintacentillion", //                 519                        172
            "treseptuagintacentillion", //                   522                        173
            "quattuorseptuagintacentillion", //          525                        174
            "quinseptuagintacentillion", //                528                        175
            "seseptuagintacentillion", //                    531                       176
            "septenseptuagintacentillion", //             534                       177
            "octoseptuagintacentillion", //                537                       178
            "novenseptuagintacentillion", //             540                       179
            "octogintacentillion", //                          543                       180
            "unoctogintacentillion", //                      546                       181
            "duooctogintacentillion", //                    549                       182
            "tresoctogintacentillion", //                    552                       183
            "quattuoroctogintacentillion", //             555                       184
            "quinoctogintacentillion", //                   558                       185
            "sexoctogintacentillion", //                     561                       186
            "septemoctogintacentillion", //               564                       187
            "octooctogintacentillion", //                   567                       188
            "novemoctogintacentillion", //               570                       189
            "nonagintacentillion", //                         573                       190
            "unnonagintacentillion", //                     576                       191
            "duononagintacentillion", //                   579                       192
            "trenonagintacentillion", //                     582                       193
            "quattuornonagintacentillion", //            585                       194
            "quinnonagintacentillion", //                  588                       195
            "senonagintacentillion", //                      591                       196
            "septenonagintacentillion", //                 594                       197
            "octononagintacentillion", //                  597                        198
            "novenonagintacentillion", //                 600                        199
            "ducentillion", //                                     603                        200 
            "unducentillion", //                                 606                        201
            "duoducentillion", //                               609                        202
            "treducentillion", //                                 612                        203
            "quattuorducentillion", //                        615                        204
            "quinducentillion", //                              618                        205
            "seducentillion", //                                  621                        206
            "septenducentillion", //                           624                        207
            "octoducentillion", //                              627                        208
            "novenducentillion", //                           630                        209
            "deciducentillion", //                              633                        210
            "undeciducentillion", //                          636                        211
            "duodeciducentillion", //                        639                        212
            "tredeciducentillion", //                          642                        213
            "quattuordeciducentillion", //                 645                        214
            "quindeciducentillion", //                       648                        215
            "sedeciducentillion", //                           651                        216
            "septendeciducentillion", //                    654                        217
            "octodeciducentillion", //                       657                        218
            "novendeciducentillion", //                    660                        219
            "vigintiducentillion", //                          663                        220
            "unvigintiducentillion", //                      666                        221
            "duovigintiducentillion", //                    669                        222
            "tresvigintiducentillion", //                    672                        223
            "quattuorvigintiducentillion", //             675                        224
            "quinvigintiducentillion", //                   678                        215
            "sesvigintiducentillion", //                     681                        226
            "septemvigintiducentillion", //               684                        227
            "octovigintiducentillion", //                   687                        228
            "novemvigintiducentillion", //               690                        229
            "trigintaducentillion", //                         693                        230
            "untrigintaducentillion", //                     696                        231
            "duotrigintaducentillion", //                   699                        232
            "trestrigintaducentillion", //                   702                        233
            "quattuortrigintaducentillion", //           705                        234
            "quintrigintaducentillion", //                  708                       235
            "sestrigintaducentillion", //                    711                        236
            "septentrigintaducentillion", //               714                        237
            "octotrigintaducentillion", //                   717                       238
            "noventrigintaducentillion", //                720                       239
            "quadragintaducentillion", //                  723                        240
            "unquadragintaducentillion", //              726                        241
            "duoquadragintaducentillion", //            729                        242
            "tresquadragintaducentillion", //            732                        243
            "quattuorquadragintaducentillion", //     735                        244
            "quinquadragintaducentillion", //           738                        245
            "sesquadragintaducentillion", //             741                        246
            "septenquadragintaducentillion", //        744                        247
            "octoquadragintaducentillion", //           747                        248
            "novenquadragintaducentillion", //        750                        249
            "quinquagintaducentillion", //                753                       250
            "unquinquagintaducentillion", //            756                       251
            "duoquinquagintaducentillion", //          759                       252
            "tresquinquagintaducentillion", //           762                      253
            "quattuorquinquagintaducentillion", //   765                      254
            "quinquinquagintaducentillion", //         768                       255
            "sesquinquagintaducentillion", //           771                        256
            "septenquinquagintaducentillion", //      774                        257
            "octoquinquagintaducentillion", //         777                        258
            "novenquinquagintaducentillion", //      780                        259
            "sexagintaducentillion", //                      783                        260
            "unsexagintaducentillion", //                  786                        261
            "duosexagintaducentillion", //                789                        262
            "tresexagintaducentillion", //                  792                        263
            "quattuorsexagintaducentillion", //         795                        264
            "quinsexagintaducentillion", //               798                        265
            "sesexagintaducentillion", //                   801                       266
            "septensexagintaducentillion", //            804                        267
            "octosexagintaducentillion", //               807                        268
            "novensexagintaducentillion", //            810                        269
            "septuagintaducentillion", //                  813                        270
            "unseptuagintaducentillion", //              816                        271
            "duoseptuagintaducentillion", //            819                        272
            "treseptuagintaducentillion", //              822                        273
            "quattuorseptuagintaducentillion", //     825                        274
            "quinseptuagintaducentillion", //           828                        275
            "seseptuagintaducentillion", //               831                        276
            "septenseptuagintaducentillion", //        834                        277
            "octoseptuagintaducentillion", //           837                        278
            "novenseptuagintaducentillion", //        840                        279
            "octogintaducentillion", //                     843                        280
            "unoctogintaducentillion", //                 846                        281 
            "duooctogintaducentillion", //               849                        282
            "tresoctogintaducentillion", //               852                        283
            "quattuoroctogintaducentillion", //        855                        284
            "quinoctogintaducentillion", //              858                        285
            "sexoctogintaducentillion", //                861                        286
            "septemoctogintaducentillion", //          864                        287
            "octooctogintaducentillion", //               867                        288
            "novemoctogintaducentillion", //           870                        289
            "nonagintaducentillion", //                     873                        290
            "unnonagintaducentillion", //                 876                        291
            "duononagintaducentillion", //               879                        292
            "trenonagintaducentillion", //                 882                        293
            "quattuornonagintaducentillion", //        885                       294
            "quinnonagintaducentillion", //              888                        295
            "senonagintaducentillion", //                  891                        296
            "septenonagintaducentillion", //             894                        297
            "octononagintaducentillion", //              897                        298
            "novenonagintaducentillion", //             900                        299
            "trecentillion", //                                    903                        300
            "untrecentillion", //                                906                        301
            "duotrecentillion", //                              909                        302
            "trestrecentillion", //                              912                        303
            "quattuortrecentillion", //                      915                        304
            "quintrecentillion", //                            918                        305
            "sestrecentillion", //                              921                        306
            "septentrecentillion", //                        924                        307
            "octotrecentillion", //                            927                       308
            "noventrecentillion", //                         930                       309
            "decitrecentillion", //                            933                        310
            "undecitrecentillion", //                        936                        311
            "duodecitrecentillion", //                      939                        312
            "tredecitrecentillion", //                        942                        313
            "quattuordecitrecentillion", //               945                        314
            "quindecitrecentillion", //                     948                        315
            "sedecitrecentillion", //                         951                        316
            "septendecitrecentillion", //                  954                       317
            "octodecitrecentillion", //                     957                        318
            "novendecitrecentillion", //                  960                        319
            "vigintitrecentillion", //                        963                        320
            "unvigintitrecentillion", //                    966                        321
            "duovigintitrecentillion", //                  969                        322
            "tresvigintitrecentillion", //                  972                        323
            "quattuorvigintitrecentillion", //          975                        324
            "quinvigintitrecentillion", //                978                        325
            "sesvigintitrecentillion", //                  981                        326
            "septemvigintitrecentillion", //            984                        327
            "octovigintitrecentillion", //                987                        328
            "novemvigintitrecentillion", //            990                        329
            "trigintatrecentillion", //                      993                        330
            "untrigintatrecentillion", //                  996                        331
            "duotrigintatrecentillion", //                999                        332
            "trestrigintatrecentillion", //               1002                        333
            "quattuortrigintatrecentillion", //        1005                       334
            "quintrigintatrecentillion", //              1008                        335
            "sestrigintatrecentillion", //                 1011                        336
            "septentrigintatrecentillion", //            1014                        337
            "octotrigintatrecentillion", //                1017                        338
            "noventrigintatrecentillion", //             1020                        339
            "quadragintatrecentillion", //                1023                        340
            "unquadragintatrecentillion", //            1026                        341
            "duoquadragintatrecentillion", //          1029                        342
            "tresquadragintatrecentillion", //           1032                        343
            "quattuorquadragintatrecentillion", //    1035                        344
            "quinquadragintatrecentillion", //          1038                        345
            "sesquadragintatrecentillion", //            1041                        346
            "septenquadragintatrecentillion", //       1044                        347
            "octoquadragintatrecentillion", //          1047                        348
            "novenquadragintatrecentillion", //       1050                        349
            "quinquagintatrecentillion", //               1053                        350
            "unquinquagintatrecentillion", //           1056                        351
            "duoquinquagintatrecentillion", //         1059                        352
            "tresquinquagintatrecentillion", //         1062                        353
            "quattuorquinquagintatrecentillion", //  1065                        354
            "quinquinquagintatrecentillion", //        1068                        355
            "sesquinquagintatrecentillion", //          1071                        356
            "septenquinquagintatrecentillion", //     1074                        357
            "octoquinquagintatrecentillion", //        1077                        358
            "novenquinquagintatrecentillion", //     1080                        359
            "sexagintatrecentillion", //                     1083                        360
            "unsexagintatrecentillion", //                 1086                        361
            "duosexagintatrecentillion", //               1089                        362
            "tresexagintatrecentillion", //                 1092                        363
            "quattuorsexagintatrecentillion", //        1095                        364
            "quinsexagintatrecentillion", //              1098                        365
            "sesexagintatrecentillion", //                  1101                        366
            "septensexagintatrecentillion", //            1104                        367
            "octosexagintatrecentillion", //               1107                        368
            "novensexagintatrecentillion", //            1110                        369
            "septuagintatrecentillion", //                   1113                        370
            "unseptuagintatrecentillion", //               1116                        371
            "duoseptuagintatrecentillion", //             1119                        372
            "treseptuagintatrecentillion", //               1122                        373
            "quattuorseptuagintatrecentillion", //      1125                        374
            "quinseptuagintatrecentillion", //            1128                        375
            "seseptuagintatrecentillion", //                1131                        376
            "septenseptuagintatrecentillion", //         1134                        377
            "octoseptuagintatrecentillion", //            1137                        378
            "novenseptuagintatrecentillion", //         1140                        379
            "octogintatrecentillion", //                      1143                        380
            "unoctogintatrecentillion", //                  1146                        381
            "duooctogintatrecentillion", //                1149                        382
            "tresoctogintatrecentillion", //                 1152                       383
            "quattuoroctogintatrecentillion", //         1155                       384
            "quinoctogintatrecentillion", //               1158                        385
            "sexoctogintatrecentillion", //                 1161                        386
            "septemoctogintatrecentillion", //           1164                        387
            "octooctogintatrecentillion", //               1167                        388
            "novemoctogintatrecentillion", //           1170                        389
            "nonagintatrecentillion", //                     1173                        390
            "unnonagintatrecentillion", //                 1176                        391
            "duononagintatrecentillion", //               1179                        392
            "trenonagintatrecentillion", //                 1182                        393
            "quattuornonagintatrecentillion", //        1185                        394
            "quinnonagintatrecentillion", //               1188                        395
            "senonagintatrecentillion", //                   1191                        396
            "septenonagintatrecentillion", //              1194                        397
            "octononagintatrecentillion", //               1197                        398
            "novenonagintatrecentillion", //               1200                       399
            "quadringentillion", //                              1203                        400
            "unquadringentillion", //                          1206                       401
            "duoquadringentillion", //                        1209                       402
            "tresquadringentillion", //                        1212                       403
            "quattuorquadringentillion", //                 1215                      404
            "quinquadringentillion", //                       1218                      405
            "sesquadringentillion", //                         1221                      406
            "septenquadringentillion", //                    1224                      407
            "octoquadringentillion", //                       1227                       408
            "novenquadringentillion", //                    1230                       409
            "deciquadringentillion", //                       1233                       410
            "undeciquadringentillion", //                   1236                       411
            "duodeciquadringentillion", //                 1239                       412
            "tredeciquadringentillion", //                   1242                       413
            "quattuordeciquadringentillion", //          1245                       414
            "quindeciquadringentillion", //                1248                       415
            "sedeciquadringentillion", //                    1251                       416
            "septendeciquadringentillion", //              1254                      417   
            "octodeciquadringentillion", //                  1257                      418
            "novendeciquadringentillion", //               1260                      419
            "vigintiquadringentillion", //                     1263                      420
            "unvigintiquadringentillion", //                 1266                      421
            "duovigintiquadringentillion", //               1269                      422
            "tresvigintiquadringentillion", //               1272                      423
            "quattuorvigintiquadringentillion", //        1275                      424
            "quinvigintiquadringentillion", //              1278                      425
            "sesvigintiquadringentillion", //                1281                      426
            "septemvigintiquadringentillion", //          1284                      427
            "octovigintiquadringentillion", //               1287                      428
            "novemvigintiquadringentillion", //           1290                      429
            "trigintaquadringentillion", //                     1293                      430
            "untrigintaquadringentillion", //                 1296                      431
            "duotrigintaquadringentillion", //               1299                      432
            "trestrigintaquadringentillion", //               1302                      433
            "quattuortrigintaquadringentillion", //        1305                      434
            "quintrigintaquadringentillion", //              1308                      435
            "sestrigintaquadringentillion", //                1311                      436
            "septentrigintaquadringentillion", //           1314                      437
            "octotrigintaquadringentillion", //               1317                     438
            "noventrigintaquadringentillion", //            1320                     439
            "quadragintaquadringentillion", //              1323                      440
            "unquadragintaquadringentillion", //          1326                      441
            "duoquadragintaquadringentillion", //        1329                      442
            "tresquadragintaquadringentillion", //        1332                      443
            "quattuorquadragintaquadringentillion", // 1335                      444
            "quinquadragintaquadringentillion", //       1338                      445
            "sesquadragintaquadringentillion", //          1341                      446
            "septenquadragintaquadringentillion", //     1344                      447
            "octoquadragintaquadringentillion", //         1347                      448
            "novenquadragintaquadringentillion", //      1350                      449
            "quinquagintaquadringentillion", //              1353                      450
            "unquinquagintaquadringentillion", //          1356                      451
            "duoquinquagintaquadringentillion", //        1359                      452
            "tresquinquagintaquadringentillion", //        1362                      453
            "quattuorquinquagintaquadringentillion", // 1365                      454
            "quinquinquagintaquadringentillion", //       1368                      455
            "sesquinquagintaquadringentillion", //         1371                      456
            "septenquinquagintaquadringentillion", //    1374                      457
            "octoquinquagintaquadringentillion", //        1377                      458
            "novenquinquagintaquadringentillion", //     1380                      459
            "sexagintaquadringentillion", //                     1383                      460
            "unsexagintaquadringentillion", //                 1386                      461
            "duosexagintaquadringentillion", //               1389                      462
            "tresexagintaquadringentillion", //                 1392                      463
            "quattuorsexagintaquadringentillion", //        1395                      464
            "quinsexagintaquadringentillion", //              1398                      465
            "sesexagintaquadringentillion", //                  1401                      466
            "septensexagintaquadringentillion", //           1404                      467
            "octosexagintaquadringentillion", //              1407                      468
            "novensexagintaquadringentillion", //           1410                      469
            "septuagintaquadringentillion", //                  1413                      470
            "unseptuagintaquadringentillion", //              1416                      471
            "duoseptuagintaquadringentillion", //            1419                      472
            "treseptuagintaquadringentillion", //              1422                      473
            "quattuorseptuagintaquadringentillion", //     1425                      474
            "quinseptuagintaquadringentillion", //           1428                      475
            "seseptuagintaquadringentillion", //               1431                      476
            "septenseptuagintaquadringentillion", //        1434                      477
            "octoseptuagintaquadringentillion", //           1437                       478
            "novenseptuagintaquadringentillion", //        1440                        479
            "octogintaquadringentillion", //                     1443                        480
            "unoctogintaquadringentillion", //                 1446                        481
            "duooctogintaquadringentillion", //               1449                        482
            "tresoctogintaquadringentillion", //               1452                        483
            "quattuoroctogintaquadringentillion", //        1455                        484
            "quinoctogintaquadringentillion", //              1458                        485
            "sexoctogintaquadringentillion", //                1461                       486
            "septemoctogintaquadringentillion", //          1464                       487
            "octooctogintaquadringentillion", //               1467                      488
            "novemoctogintaquadringentillion", //           1470                      489
            "nonagintaquadringentillion", //                     1473                      490
            "unnonagintaquadringentillion", //                 1476                      491
            "duononagintaquadringentillion", //               1479                      492
            "trenonagintaquadringentillion", //                 1482                      493
            "quattuornonagintaquadringentillion", //        1485                      494
            "quinnonagintaquadringentillion", //              1488                      495
            "senonagintaquadringentillion", //                  1491                      496
            "septenonagintaquadringentillion", //             1494                      497
            "octononagintaquadringentillion", //              1497                       498
            "novenonagintaquadringentillion", //             1500                       499
            "quingentillion", //                                         1503                        500
            "unquingentillion", //                                     1506                        501
            "duoquingentillion", //                                   1509                        502
            "tresquingentillion", //                                    1512                       503
            "quattuorquingentillion", //                            1515                        504
            "quinquingentillion", //                                  1518                        505
            "sesquingentillion", //                                    1521                        506
            "septenquingentillion", //                               1524                        507
            "octoquingentillion", //                                  1527                        508
            "novenquingentillion", //                               1530                        509
            "deciquingentillion", //                                  1533                        510
            "undeciquingentillion", //                              1536                        511
            "duodeciquingentillion", //                            1539                        512
            "tredeciquingentillion", //                              1542                        513
            "quattuordeciquingentillion", //                     1545                        514
            "quindeciquingentillion", //                            1548                        515
            "sedeciquingentillion", //                                1551                        516
            "septendeciquingentillion", //                         1554                        517
            "octodeciquingentillion", //                            1557                        518
            "novendeciquingentillion", //                         1560                        519
            "vigintiquingentillion", //                               1563                        520
            "unvigintiquingentillion", //                           1566                        521
            "duovigintiquingentillion", //                         1569                        522
            "tresvigintiquingentillion", //                          1572                       523
            "quattuorvigintiquingentillion", //                   1575                       524
            "quinvigintiquingentillion", //                         1578                       525
            "sesvigintiquingentillion", //                           1581                       526
            "septemvigintiquingentillion", //                     1584                       527
            "octovigintiquingentillion", //                          1587                       528
            "novemvigintiquingentillion", //                      1590                       529
            "trigintaquingentillion", //                                1593                       530
            "untrigintaquingentillion", //                            1596                       531
            "duotrigintaquingentillion", //                          1599                       532
            "trestrigintaquingentillion", //                          1602                       533
            "quattuortrigintaquingentillion", //                   1605                       534
            "quintrigintaquingentillion", //                         1608                       535
            "sestrigintaquingentillion", //                           1611                       536
            "septentrigintaquingentillion", //                      1614                       537
            "octotrigintaquingentillion", //                         1617                       538
            "noventrigintaquingentillion", //                      1620                       539
            "quadragintaquingentillion", //                        1623                        540
            "unquadragintaquingentillion", //                    1626                        541
            "duoquadragintaquingentillion", //                  1629                        542
            "tresquadragintaquingentillion", //                  1632                        543
            "quattuorquadragintaquingentillion", //           1635                        544
            "quinquadragintaquingentillion", //                 1638                        545
            "sesquadragintaquingentillion", //                   1641                        546
            "septenquadragintaquingentillion", //              1644                        547
            "octoquadragintaquingentillion", //                  1647                       548
            "novenquadragintaquingentillion", //               1650                       549
            "quinquagintaquingentillion", //                       1653                       550
            "unquinquagintaquingentillion", //                   1656                       551
            "duoquinquagintaquingentillion", //                 1659                       552
            "tresquinquagintaquingentillion", //                 1662                       553
            "quattuorquinquagintaquingentillion", //          1665                      554
            "quinquinquagintaquingentillion", //                1668                      555
            "sesquinquagintaquingentillion", //                  1671                      556
            "septenquinquagintaquingentillion", //             1674                      557
            "octoquinquagintaquingentillion", //                1677                      558
            "novenquinquagintaquingentillion", //             1680                      559
            "sexagintaquingentillion", //                             1683                      560
            "unsexagintaquingentillion", //                         1686                      561
            "duosexagintaquingentillion", //                       1689                      562
            "tresexagintaquingentillion", //                         1692                      563
            "quattuorsexagintaquingentillion", //                1695                      564
            "quinsexagintaquingentillion", //                      1698                       565
            "sesexagintaquingentillion", //                          1701                       566
            "septensexagintaquingentillion", //                   1704                       567
            "octosexagintaquingentillion", //                       1707                       568
            "novensexagintaquingentillion", //                    1710                       569
            "septuagintaquingentillion", //                           1713                       570
            "unseptuagintaquingentillion", //                       1716                       571
            "duoseptuagintaquingentillion", //                     1719                       572
            "treseptuagintaquingentillion", //                       1722                       573
            "quattuorseptuagintaquingentillion", //              1725                       574
            "quinseptuagintaquingentillion", //                    1728                       575
            "seseptuagintaquingentillion", //                        1731                       576
            "septenseptuagintaquingentillion", //                 1734                       577
            "octoseptuagintaquingentillion", //                     1737                      578
            "novenseptuagintaquingentillion", //                  1740                      579
            "octogintaquingentillion", //                               1743                      580
            "unoctogintaquingentillion", //                           1746                      581
            "duooctogintaquingentillion", //                         1749                      582
            "tresoctogintaquingentillion", //                         1752                      583
            "quattuoroctogintaquingentillion", //                  1755                      584
            "quinoctogintaquingentillion", //                        1758                      585
            "sexoctogintaquingentillion", //                          1761                      586
            "septemoctogintaquingentillion", //                    1764                      587
            "octooctogintaquingentillion", //                         1767                      588
            "novemoctogintaquingentillion", //                     1770                      589
            "nonagintaquingentillion", //                               1773                      590
            "unnonagintaquingentillion", //                           1776                      591
            "duononagintaquingentillion", //                         1779                      592
            "trenonagintaquingentillion", //                           1782                      593
            "quattuornonagintaquingentillion", //                  1785                      594
            "quinnonagintaquingentillion", //                        1788                      595
            "senonagintaquingentillion", //                            1791                      596
            "septenonagintaquingentillion", //                       1794                      597
            "octononagintaquingentillion", //                        1797                      598
            "novenonagintaquingentillion", //                       1800                      599
            "sescentillion", //                                                 1803                      600
            "unsescentillion", //                                             1806                      601
            "duosescentillion", //                                           1809                      602
            "tresescentillion", //                                             1812                      603
            "quattuorsescentillion", //                                    1815                      604
            "quinsescentillion", //                                          1818                      605
            "sesescentillion", //                                              1821                      606
            "septensescentillion", //                                       1824                      607
            "octosescentillion", //                                          1827                       608
            "novensescentillion", //                                       1830                       609
            "decisescentillion", //                                          1833                       610
            "undecisescentillion", //                                      1836                       611
            "duodecisescentillion", //                                    1839                       612
            "tredecisescentillion", //                                     1842                        613
            "quattuordecisescentillion", //                            1845                        614
            "quindecisescentillion", //                                  1848                        615
            "sedecisescentillion", //                                      1851                        616
            "septendecisescentillion", //                               1854                        617
            "octodecisescentillion", //                                  1857                        618
            "novendecisescentillion", //                               1860                        619
            "vigintisescentillion", //                                     1863                        620
            "unvigintisescentillion", //                                 1866                        621
            "duovigintisescentillion", //                               1869                        622
            "tresvigintisescentillion", //                               1872                        623
            "quattuorvigintisescentillion", //                       1875                        624
            "quinvigintisescentillion", //                             1878                        625
            "sesvigintisescentillion", //                               1881                        626
            "septemvigintisescentillion", //                         1884                        627
            "octovigintisescentillion", //                             1887                        628
            "novemvigintisescentillion", //                         1890                        629
            "trigintasescentillion", //                                   1893                        630
            "untrigintasescentillion", //                               1896                        631
            "duotrigintasescentillion", //                             1899                        632
            "trestrigintasescentillion", //                             1902                        633
            "quattuortrigintasescentillion", //                      1905                        634
            "quintrigintasescentillion", //                            1908                        635
            "sestrigintasescentillion", //                              1911                        636
            "septentrigintasescentillion", //                         1914                        637
            "octotrigintasescentillion", //                            1917                        638
            "noventrigintasescentillion", //                         1920                        639
            "quadragintasescentillion", //                           1923                        640
            "unquadragintasescentillion", //                       1926                        641
            "duoquadragintasescentillion", //                     1929                        642
            "tresquadragintasescentillion", //                     1932                        643
            "quattuorquadragintasescentillion", //              1935                        644
            "quinquadragintasescentillion", //                    1938                        645
            "sesquadragintasescentillion", //                      1941                        646
            "septenquadragintasescentillion", //                 1944                        647
            "octoquadragintasescentillion", //                    1947                        648
            "novenquadragintasescentillion", //                 1950                        649
            "quinquagintasescentillion", //                         1953                        650
            "unquinquagintasescentillion", //                     1956                        651
            "duoquinquagintasescentillion", //                   1959                        652
            "tresquinquagintasescentillion", //                   1962                        653
            "quattuorquinquagintasescentillion", //           1965                        654
            "quinquinquagintasescentillion", //                 1968                        655
            "sesquinquagintasescentillion", //                   1971                        656
            "septenquinquagintasescentillion", //              1974                        657
            "octoquinquagintasescentillion", //                 1977                        658
            "novenquinquagintasescentillion", //              1980                        659
            "sexagintasescentillion", //                             1983                        660
            "unsexagintasescentillion", //                         1986                        661
            "duosexagintasescentillion", //                       1989                        662
            "tresexagintasescentillion", //                        1992                         663
            "quattuorsexagintasescentillion", //               1995                         664
            "quinsexagintasescentillion", //                     1998                         665
            "sesexagintasescentillion", //                         2001                         666
            "septensexagintasescentillion", //                  2004                         667
            "octosexagintasescentillion", //                     2007                         668
            "novensexagintasescentillion", //                  2010                         669
            "septuagintasescentillion", //                         2013                         670
            "unseptuagintasescentillion", //                     2016                        671
            "duoseptuagintasescentillion", //                   2019                        672
            "treseptuagintasescentillion", //                     2022                        673
            "quattuorseptuagintasescentillion", //            2025                        674
            "quinseptuagintasescentillion", //                  2028                        675
            "seseptuagintasescentillion", //                      2031                        676
            "septenseptuagintasescentillion", //               2034                        677
            "octoseptuagintasescentillion", //                  2037                        678
            "novenseptuagintasescentillion", //               2040                        679
            "octogintasescentillion", //                            2043                        680
            "unoctogintasescentillion", //                        2046                        681
            "duooctogintasescentillion", //                      2049                        682
            "tresoctogintasescentillion", //                      2052                        683
            "quattuoroctogintasescentillion", //              2055                        684
            "quinoctogintasescentillion", //                    2058                        685
            "sexoctogintasescentillion", //                      2061                        686
            "septemoctogintasescentillion", //                2064                        687
            "octooctogintasescentillion", //                    2067                        688
            "novemoctogintasescentillion", //                2070                        689
            "nonagintasescentillion", //                          2073                        690
            "unnonagintasescentillion", //                      2076                        691
            "duononagintasescentillion", //                    2079                        692
            "trenonagintasescentillion", //                      2082                        693
            "quattuornonagintasescentillion", //             2085                        694
            "quinnonagintasescentillion", //                   2088                        695
            "senonagintasescentillion", //                       2091                        696
            "septenonagintasescentillion", //                  2094                        697
            "octononagintasescentillion", //                   2097                         698
            "novenonagintasescentillion", //                  2100                         699
            "septingentillion", //                                     2103                        700
            "unseptingentillion", //                                 2106                        701
            "duoseptingentillion", //                               2109                        702
            "treseptingentillion", //                                 2112                        703
            "quattuorseptingentillion", //                        2115                        704
            "quinseptingentillion", //                              2118                        705
            "seseptingentillion", //                                  2121                        706
            "septenseptingentillion", //                           2124                        707
            "octoseptingentillion", //                              2127                        708
            "novenseptingentillion", //                           2130                        709
            "deciseptingentillion", //                              2133                        710
            "undeciseptingentillion", //                          2136                        711
            "duodeciseptingentillion", //                        2139                        712 
            "tredeciseptingentillion", //                          2142                        713
            "quattuordeciseptingentillion", //                 2145                        714
            "quindeciseptingentillion", //                       2148                        715
            "sedeciseptingentillion", //                           2151                        716
            "septendeciseptingentillion", //                    2154                        717
            "octodeciseptingentillion", //                       2157                        718
            "novendeciseptingentillion", //                    2160                        719
            "vigintiseptingentillion", //                          2163                        720
            "unvigintiseptingentillion", //                      2166                        721
            "duovigintiseptingentillion", //                    2169                        722
            "tresvigintiseptingentillion", //                    2172                        723
            "quattuorvigintiseptingentillion", //            2175                        724
            "quinvigintiseptingentillion", //                  2178                        725
            "sesvigintiseptingentillion", //                    2181                        726
            "septemvigintiseptingentillion", //              2184                        727
            "octovigintiseptingentillion", //                  2187                        728
            "novemvigintiseptingentillion", //              2190                        739
            "trigintaseptingentillion", //                        2193                        730
            "untrigintaseptingentillion", //                    2196                        731
            "duotrigintaseptingentillion", //                  2199                        732
            "trestrigintaseptingentillion", //                  2202                        733
            "quattuortrigintaseptingentillion", //          2205                        734
            "quintrigintaseptingentillion",//                 2208                        735
            "sestrigintaseptingentillion", //                  2211                        736
            "septentrigintaseptingentillion", //             2214                        737
            "octotrigintaseptingentillion", //                2217                        738
            "noventrigintaseptingentillion", //             2220                        739
            "quadragintaseptingentillion", //                2223                        740
            "unquadragintaseptingentillion", //            2226                        741
            "duoquadragintaseptingentillion", //          2229                        742
            "tresquadragintaseptingentillion", //          2232                        743
            "quattuorquadragintaseptingentillion", //  2235                        744
            "quinquadragintaseptingentillion", //        2238                        745
            "sesquadragintaseptingentillion", //          2241                        746
            "septenquadragintaseptingentillion", //     2244                        747
            "octoquadragintaseptingentillion", //         2247                        748
            "novenquadragintaseptingentillion", //      2250                        749
            "quinquagintaseptingentillion", //              2253                        750
            "unquinquagintaseptingentillion", //          2256                        751
            "duoquinquagintaseptingentillion", //        2259                        752
            "tresquinquagintaseptingentillion", //        2262                        753
            "quattuorquinquagintaseptingentillion", // 2265                        754
            "quinquinquagintaseptingentillion", //       2268                        755
            "sesquinquagintaseptingentillion", //         2271                        756
            "septenquinquagintaseptingentillion", //    2274                        757
            "octoquinquagintaseptingentillion", //        2277                        758
            "novenquinquagintaseptingentillion", //     2280                        759
            "sexagintaseptingentillion", //                    2283                         760
            "unsexagintaseptingentillion", //                2286                         761
            "duosexagintaseptingentillion", //              2289                         762
            "tresexagintaseptingentillion", //                2292                         763
            "quattuorsexagintaseptingentillion", //       2295                         764
            "quinsexagintaseptingentillion", //             2298                         765
            "sesexagintaseptingentillion", //                 2301                         766
            "septensexagintaseptingentillion", //          2304                         767
            "octosexagintaseptingentillion", //             2307                         768
            "novensexagintaseptingentillion", //          2310                         769
            "septuagintaseptingentillion", //                 2313                         770
            "unseptuagintaseptingentillion", //             2316                         771
            "duoseptuagintaseptingentillion", //           2319                        772
            "treseptuagintaseptingentillion", //             2322                        773
            "quattuorseptuagintaseptingentillion", //    2325                        774
            "quinseptuagintaseptingentillion", //          2328                        775
            "seseptuagintaseptingentillion", //              2331                        776
            "septenseptuagintaseptingentillion", //       2334                        777
            "octoseptuagintaseptingentillion", //          2337                        778
            "novenseptuagintaseptingentillion", //       2340                        779
            "octogintaseptingentillion", //                    2343                        780
            "unoctogintaseptingentillion", //                2346                        781
            "duooctogintaseptingentillion", //              2349                        782
            "tresoctogintaseptingentillion", //              2352                        783
            "quattuoroctogintaseptingentillion", //       2355                        784
            "quinoctogintaseptingentillion", //             2358                        785
            "sexoctogintaseptingentillion", //               2361                        786
            "septemoctogintaseptingentillion", //         2364                        787
            "octooctogintaseptingentillion", //              2367                        788
            "novemoctogintaseptingentillion", //          2370                        789
            "nonagintaseptingentillion", //                    2373                        790
            "unnonagintaseptingentillion", //                2376                        791
            "duononagintaseptingentillion", //              2379                        792
            "trenonagintaseptingentillion", //                2382                        793
            "quattuornonagintaseptingentillion", //       2385                        794
            "quinnonagintaseptingentillion", //             2388                        795
            "senonagintaseptingentillion", //                 2391                        796
            "septenonagintaseptingentillion", //            2394                        797
            "octononagintaseptingentillion", //             2397                        798
            "novenonagintaseptingentillion", //            2400                        799
            "octingentillion", //                                     2403                        800
            "unoctingentillion", //                                 2406                        801
            "duooctingentillion", //                               2409                        802
            "tresoctingentillion", //                               2412                        803
            "quattuoroctingentillion", //                       2415                        804
            "quinoctingentillion", //                             2418                        805 
            "sexoctingentillion", //                               2421                        806
            "septemoctingentillion", //                         2424                        807
            "octooctingentillion", //                             2427                        808
            "novemoctingentillion", //                         2430                        809
            "decioctingentillion", //                             2433                        810
            "undecioctingentillion", //                         2436                        811
            "duodecioctingentillion", //                       2439                        812
            "tredecioctingentillion", //                         2442                        813
            "quattuordecioctingentillion", //                2445                        814
            "quindecioctingentillion", //                       2448                       815
            "sedecioctingentillion", //                           2451                       816
            "septendecioctingentillion", //                    2454                       817
            "octodecioctingentillion", //                       2457                        818
            "novendecioctingentillion", //                    2460                        819
            "vigintioctingentillion", //                          2463                        820
            "unvigintioctingentillion", //                      2466                        821
            "duovigintioctingentillion", //                    2469                        822
            "tresvigintioctingentillion", //                    2472                        823
            "quattuorvigintioctingentillion", //             2475                        824
            "quinvigintioctingentillion", //                   2478                        825
            "sesvigintioctingentillion", //                     2481                        826
            "septemvigintioctingentillion", //               2484                       827
            "octovigintioctingentillion", //                   2487                        828
            "novemvigintioctingentillion", //               2490                        829
            "trigintaoctingentillion", //                         2493                        830
            "untrigintaoctingentillion", //                     2496                        831
            "duotrigintaoctingentillion", //                   2499                        832
            "trestrigintaoctingentillion", //                   2502                        833
            "quattuortrigintaoctingentillion", //            2505                        834
            "quintrigintaoctingentillion", //                  2508                        835
            "sestrigintaoctingentillion", //                    2511                        836
            "septentrigintaoctingentillion", //               2514                        837
            "octotrigintaoctingentillion", //                  2517                        838
            "noventrigintaoctingentillion", //               2520                        839
            "quadragintaoctingentillion", //                  2523                        840
            "unquadragintaoctingentillion", //              2526                        841
            "duoquadragintaoctingentillion", //            2529                        842
            "tresquadragintaoctingentillion", //            2532                        843
            "quattuorquadragintaoctingentillion", //     2535                        844
            "quinquadragintaoctingentillion", //           2538                        845
            "sesquadragintaoctingentillion", //             2541                        846
            "septenquadragintaoctingentillion", //        2544                        847
            "octoquadragintaoctingentillion", //           2547                        848
            "novenquadragintaoctingentillion", //        2550                        849
            "quinquagintaoctingentillion", //                2553                        850
            "unquinquagintaoctingentillion", //            2556                        851
            "duoquinquagintaoctingentillion", //          2559                        852
            "tresquinquagintaoctingentillion", //          2562                        853
            "quattuorquinquagintaoctingentillion", //  2565                        854
            "quinquinquagintaoctingentillion", //        2568                        855
            "sesquinquagintaoctingentillion", //          2571                        856
            "septenquinquagintaoctingentillion", //     2574                        857
            "octoquinquagintaoctingentillion", //        2577                        858
            "novenquinquagintaoctingentillion", //     2580                        859
            "sexagintaoctingentillion", //                     2583                        860
            "unsexagintaoctingentillion", //                 2586                        861
            "duosexagintaoctingentillion", //               2589                        862
            "tresexagintaoctingentillion", //                 2592                        863
            "quattuorsexagintaoctingentillion", //        2595                        864
            "quinsexagintaoctingentillion", //              2598                        865
            "sesexagintaoctingentillion", //                  2601                        866
            "septensexagintaoctingentillion", //           2604                        867
            "octosexagintaoctingentillion", //              2607                        868
            "novensexagintaoctingentillion", //           2610                        869
            "septuagintaoctingentillion", //                  2613                        870
            "unseptuagintaoctingentillion", //              2616                        871
            "duoseptuagintaoctingentillion", //            2619                        872
            "treseptuagintaoctingentillion", //              2622                        873
            "quattuorseptuagintaoctingentillion", //     2625                        874
            "quinseptuagintaoctingentillion", //           2628                        875
            "seseptuagintaoctingentillion", //               2631                        876
            "septenseptuagintaoctingentillion", //        2634                        877
            "octoseptuagintaoctingentillion", //            2637                       878
            "novenseptuagintaoctingentillion", //         2640                       879
            "octogintaoctingentillion", //                      2643                       880
            "unoctogintaoctingentillion", //                  2646                       881
            "duooctogintaoctingentillion", //                2649                       882
            "tresoctogintaoctingentillion", //                2652                       883
            "quattuoroctogintaoctingentillion", //        2655                       884
            "quinoctogintaoctingentillion", //              2658                       885
            "sexoctogintaoctingentillion", //                2661                       886
            "septemoctogintaoctingentillion", //          2664                       887
            "octooctogintaoctingentillion", //               2667                       888
            "novemoctogintaoctingentillion", //           2670                       889
            "nonagintaoctingentillion", //                     2673                       890
            "unnonagintaoctingentillion", //                 2676                       891
            "duononagintaoctingentillion", //               2679                       892
            "trenonagintaoctingentillion", //                 2682                       893
            "quattuornonagintaoctingentillion", //        2685                       894
            "quinnonagintaoctingentillion", //              2688                       895
            "senonagintaoctingentillion", //                  2691                       896
            "septenonagintaoctingentillion", //             2694                       897
            "octononagintaoctingentillion", //              2697                        898
            "novenonagintaoctingentillion", //             2700                        899
            "nongentillion", //                                       2703                        900
            "unnongentillion", //                                   2706                        901
            "duonongentillion", //                                 2709                        902
            "trenongentillion", //                                   2712                        903
            "quattuornongentillion", //                          2715                        904
            "quinnongentillion", //                                2718                        905
            "senongentillion", //                                    2721                        906
            "septenongentillion", //                               2724                        907
            "octonongentillion", //                                2727                        908
            "novenongentillion", //                               2730                        909
            "decinongentillion", //                                2733                        910
            "undecinongentillion", //                            2736                        911
            "duodecinongentillion", //                          2739                        912
            "tredecinongentillion", //                            2742                        913
            "quattuordecinongentillion", //                   2745                        914
            "quindecinongentillion", //                         2748                        915
            "sedecinongentillion", //                             2751                        916
            "septendecinongentillion", //                      2754                        917
            "octodecinongentillion", //                         2757                        918
            "novendecinongentillion", //                      2760                        919
            "vigintinongentillion", //                            2763                        920
            "unvigintinongentillion", //                        2766                        921
            "duovigintinongentillion", //                      2769                        922
            "tresvigintinongentillion", //                      2772                        923
            "quattuorvigintinongentillion", //               2775                        924
            "quinvigintinongentillion", //                     2778                        925
            "sesvigintinongentillion", //                       2781                        926
            "septemvigintinongentillion", //                 2784                        927
            "octovigintinongentillion", //                      2787                        928
            "novemvigintinongentillion", //                  2790                        929
            "trigintanongentillion", //                            2793                        930
            "untrigintanongentillion", //                        2796                        931
            "duotrigintanongentillion", //                      2799                        932
            "trestrigintanongentillion", //                      2802                        933
            "quattuortrigintanongentillion", //               2805                        934
            "quintrigintanongentillion", //                     2808                        935
            "sestrigintanongentillion", //                       2811                        936
            "septentrigintanongentillion", //                  2814                        937
            "octotrigintanongentillion", //                     2817                        938
            "noventrigintanongentillion", //                  2820                        939
            "quadragintanongentillion", //                     2823                        940
            "unquadragintanongentillion", //                 2826                        941
            "duoquadragintanongentillion", //               2829                        942
            "tresquadragintanongentillion", //               2832                        943
            "quattuorquadragintanongentillion", //        2835                       944
            "quinquadragintanongentillion", //              2838                        945
            "sesquadragintanongentillion", //                2841                        946
            "septenquadragintanongentillion", //           2844                        947
            "octoquadragintanongentillion", //               2847                       948
            "novenquadragintanongentillion", //            2850                        949
            "quinquagintanongentillion", //                    2853                       950
            "unquinquagintanongentillion", //                2856                       951
            "duoquinquagintanongentillion", //              2859                       952
            "tresquinquagintanongentillion", //              2862                        953
            "quattuorquinquagintanongentillion", //       2865                       954
            "quinquinquagintanongentillion", //             2868                        955
            "sesquinquagintanongentillion", //               2871                        956
            "septenquinquagintanongentillion", //          2874                        957
            "octoquinquagintanongentillion", //             2877                        958
            "novenquinquagintanongentillion", //          2880                        959
            "sexagintanongentillion", //                          2883                        960
            "unsexagintanongentillion", //                      2886                        961
            "duosexagintanongentillion", //                    2889                        962
            "tresexagintanongentillion", //                      2892                        963
            "quattuorsexagintanongentillion", //             2895                        964
            "quinsexagintanongentillion", //                   2898                        965
            "sesexagintanongentillion", //                       2901                        966
            "septensexagintanongentillion", //                2904                        967
            "octosexagintanongentillion", //                   2907                        968
            "novensexagintanongentillion", //                2910                        969
            "septuagintanongentillion", //                       2913                        970
            "unseptuagintanongentillion", //                   2916                        971 
            "duoseptuagintanongentillion", //                 2919                        972
            "treseptuagintanongentillion", //                   2922                        973
            "quattuorseptuagintanongentillion", //          2925                        974
            "quinseptuagintanongentillion", //                2928                        975
            "seseptuagintanongentillion", //                    2931                        976
            "septenseptuagintanongentillion", //             2934                        977
            "octoseptuagintanongentillion", //                2937                        978
            "novenseptuagintanongentillion", //             2940                        979
            "octogintanongentillion", //                          2943                        980
            "unoctogintanongentillion", //                      2946                        981
            "duooctogintanongentillion", //                    2949                        982
            "tresoctogintanongentillion", //                    2952                        983
            "quattuoroctogintanongentillion", //            2955                        984
            "quinoctogintanongentillion", //                  2958                        985
            "sexoctogintanongentillion", //                    2961                        986
            "septemoctogintanongentillion", //              2964                        987
            "octooctogintanongentillion", //                   2967                        988
            "novemoctogintanongentillion", //               2970                        989
            "nonagintanongentillion", //                         2973                        990
            "unnonagintanongentillion", //                     2976                        991
            "duononagintanongentillion", //                   2979                        992
            "trenonagintanongentillion", //                     2982                        993
            "quattuornonagintanongentillion", //            2985                        994
            "quinnonagintanongentillion", //                  2988                        995
            "senonagintanongentillion", //                      2991                        996
            "septenonagintanongentillion", //                 2994                        997
            "octononagintanongentillion", //                   2997                       998
            "novenonagintanongentillion", //                  3000                       999
            "millinillion", //                                             3003                     1000
            "millimillion", //                                            3006                     1001
            "millibillion", //                                             3009                     1002
            "millitrillion", //                                             3012                     1003
            "milliquadrillion", //                                      3015                     1004
            "milliquintillion", //                                       3018                     1005
            "millisextillion", //                                         3021                     1006
            "milliseptillion", //                                         3024                     1007
            "millioctillion", //                                           3027                     1008
            "millinonillion", //                                          3030                     1009
            "millidecillion", //                                          3033                      1010
            "milliundecillion", //                                      3036                      1011
            "milliduodecillion", //                                    3039                      1012
            "millitredecillion", //                                      3042                      1013
            "milliquattuordecillion", //                             3045                      1014
            "milliquindecillion", //                                   3048                      1015
            "millisedecillion", //                                       3051                      1016
            "milliseptendecillion", //                                3054                      1017
            "millioctodecillion", //                                   3057                      1018
            "millinovendecillion", //                                3060                      1019
            "millivigintillion", //                                      3063                      1020
            "milliunvigintillion", //                                  3066                      1021
            "milliduovigintillion", //                                3069                      1022
            "millitresvigintillion", //                                3072                      1023
            "milliquattuorvigintillion", //                         3075                      1024
            "milliquinvigintillion", //                               3078                      1025
            "millisesvigintillion", //                                 3081                      1026
            "milliseptemvigintillion", //                           3084                      1027
            "millioctovigintillion", //                                3087                     1028
            "millinovemvigintillion", //                            3090                     1029
            "millitrigintillion", //                                       3093                     1030
            "milliuntrigintillion", //                                   3096                     1031
            "milliduotrigintillion", //                                 3099                     1032
            "millitrestrigintillion", //                                 3102                     1033
            "milliquattuortrigintillion", //                         3105                     1034
            "milliquintrigintillion", //                               3108                     1035
            "millisestrigintillion", //                                 3111                      1036
            "milliseptentrigintillion", //                            3114                      1037
            "millioctotrigintillion", //                               3117                      1038
            "millinoventrigintillion", //                            3120                      1039
            "milliquadragintillion", //                               3123                      1040
            "milliunquadragintillion", //                           3126                      1041
            "milliduoquadragintillion", //                         3129                      1042
            "millitresquadragintillion", //                         3132                      1043
            "milliquattuorquadragintillion", //                  3135                      1044
            "milliquinquadragintillion", //                        3138                      1045
            "millisesquadragintillion", //                          3141                      1046
            "milliseptenquadragintillion", //                     3144                      1047
            "millioctoquadragintillion", //                        3147                      1048
            "millinovenquadragintillion", //                     3150                      1049
            "milliquinquagintillion", //                             3153                      1050
            "milliunquinquagintillion", //                         3156                      1051
            "milliduoquinquagintillion", //                       3159                      1052
            "millitresquinquagintillion", //                       3162                       1053
            "milliquattuorquinquagintillion", //                3165                       1054
            "milliquinquinquagintillion", //                      3168                       1055
            "millisesquinquagintillion", //                         3171                      1056
            "milliseptenquinquagintillion", //                    3174                      1057
            "millioctoquinquagintillion", //                       3177                      1058
            "millinovenquinquagintillion", //                     3180                     1059
            "millisexagintillion", //                                    3183                      1060  
            "milliunsexagintillion", //                                3186                      1061            
            "milliduosexagintillion", //                              3189                      1062
            "millitresexagintillion", //                                3192                      1063
            "milliquattuorsexagintillion", //                       3195                      1064
            "milliquinsexagintillion", //                             3198                      1065
            "millisesexagintillion", //                                 3201                      1066
            "milliseptensexagintillion", //                          3204                      1067
            "millioctosexagintillion", //                             3207                       1068
            "millinovensexagintillion", //                          3210                       1069
            "milliseptuagintillion", //                                 3213                       1070
            "milliunseptuagintillion", //                             3216                       1071
            "milliduoseptuagintillion", //                           3219                       1072
            "millitreseptuagintillion", //                             3222                       1073
            "milliquattuorseptuagintillion", //                    3225                       1074
            "milliquinseptuagintillion", //                          3228                        1075
            "milliseseptuagintillion", //                              3231                        1076
            "milliseptenseptuagintillion", //                       3234                        1077
            "millioctoseptuagintillion", //                           3237                        1078
            "millinovenseptuagintillion", //                        3240                        1079
            "millioctogintillion", //                                     3243                        1080
            "milliunoctogintillion", //                                 3246                        1081
            "milliduooctogintillion", //                               3249                        1082
            "millitresoctogintillion", //                               3252                        1083
            "milliquattuoroctogintillion", //                        3255                        1084
            "milliquinoctogintillion", //                              3258                        1085
            "millisexoctogintillion", //                                3261                        1086
            "milliseptemoctogintillion", //                          3264                        1087
            "millioctooctogintillion", //                               3267                        1088
            "millinovemoctogintillion", //                           3270                        1089
            "millinonagintillion", //                                     3273                        1090
            "milliunnonagintillion", //                                 3276                        1091
            "milliduononagintillion", //                               3279                        1092
            "millitrenonagintillion", //                                 3282                        1093
            "milliquattuornonagintillion", //                        3285                        1094
            "milliquinnonagintillion", //                              3288                        1095
            "millisenonagintillion", //                                  3291                        1096
            "milliseptenonagintillion", //                             3294                        1097
            "millioctononagintillion", //                              3297                        1098
            "millinovenonagintillion", //                             3300                        1099
            "millicentillion", //                                            3303                        1100
            "milliuncentillion", //                                        3306                        1101
            "milliduocentillion", //                                      3309                        1102
            "millitrescentillion", //                                      3312                        1103
            "milliquattuorcentillion", //                              3315                        1104
            "milliquincentillion", //                                    3318                        1105
            "millisexcentillion", //                                      3321                        1106
            "milliseptencentillion", //                                 3324                        1107
            "millioctocentillion", //                                    3327                        1108
            "millinovencentillion", //                                 3330                        1109
            "millidecicentillion", //                                    3333                        1110
            "milliundecicentillion", //                                3336                        1111
            "milliduodecicentillion", //                              3339                        1112
            "millitredecicentillion", //                                3342                        1113
            "milliquattuordecicentillion", //                       3345                        1114
            "milliquindecicentillion", //                             3348                        1115
            "millisedecicentillion", //                                 3351                        1116
            "milliseptendecicentillion", //                          3354                        1117
            "millioctodecicentillion", //                             3357                        1118
            "millinovendecicentillion", //                          3360                        1119
            "milliviginticentillion", //                                3363                        1120
            "milliunviginticentillion", //                            3366                        1121
            "milliduoviginticentillion", //                          3369                        1122
            "millitresviginticentillion", //                          3372                        1123
            "milliquattuorviginticentillion", //                   3375                        1124
            "milliquinviginticentillion", //                         3378                        1125
            "millisesviginticentillion", //                           3381                        1126
            "milliseptemviginticentillion", //                     3384                        1127
            "millioctoviginticentillion", //                          3387                       1128
            "millinovemviginticentillion", //                      3390                       1129
            "millitrigintacentillion", //                                3393                       1130
            "milliuntrigintacentillion", //                            3396                       1131
            "milliduotrigintacentillion", //                          3399                       1132
            "millitrestrigintacentillion", //                          3402                       1133
            "milliquattuortrigintacentillion", //                   3405                       1134
            "milliquintrigintacentillion", //                         3408                       1135
            "millisestrigintacentillion", //                           3411                       1136
            "milliseptentrigintacentillion", //                      3414                       1137
            "millioctotrigintacentillion", //                         3417                       1138
            "millinoventrigintacentillion", //                      3420                       1139
            "milliquadragintacentillion", //                        3423                        1140
            "milliunquadragintacentillion", //                    3426                        1141
            "milliduoquadragintacentillion", //                  3329                        1142
            "millitresquadragintacentillion", //                   3332                       1143
            "milliquattuorquadragintacentillion", //           3335                        1144
            "milliquinquadragintacentillion", //                  3338                       1145
            "millisesquadragintacentillion", //                    3341                       1146
            "milliseptenquadragintacentillion", //              3344                        1147
            "millioctoquadragintacentillion", //                 3447                        1148
            "millinovenquadragintacentillion", //              3450                        1149
            "milliquinquagintacentillion", //                      3453                        1150
            "milliunquinquagintacentillion", //                  3456                        1151
            "milliduoquinquagintacentillion", //                3459                        1152
            "millitresquinquagintacentillion", //                3462                        1153
            "milliquattuorquinquagintacentillion", //        3465                        1154
            "milliquinquinquagintacentillion", //               3468                        1155
            "millisesquinquagintacentillion", //                 3471                        1156
            "milliseptenquinquagintacentillion", //            3474                        1157
            "millioctoquinquagintacentillion", //                3477                       1158
            "millinovenquinquagintacentillion", //             3480                       1159
            "millisexagintacentillion", //                             3483                       1160
            "milliunsexagintacentillion", //                         3486                       1161
            "milliduosexagintacentillion", //                       3489                       1162
            "millitresexagintacentillion", //                         3492                       1163
            "milliquattuorsexagintacentillion", //                3495                       1164
            "milliquinsexagintacentillion", //                      3498                       1165
            "millisesexagintacentillion", //                          3501                       1166
            "milliseptensexagintacentillion", //                   3504                       1167
            "millioctosexagintacentillion", //                       3507                      1168
            "millinovensexagintacentillion", //                    3510                      1169
            "milliseptuagintacentillion", //                           3513                      1170                                                   
            "milliunseptuagintacentillion", //                       3516                      1171
            "milliduoseptuagintacentillion", //                     3519                      1172
            "millitreseptuagintacentillion", //                       3522                      1173
            "milliquattuorseptuagintacentillion", //              3525                      1174
            "milliquinseptuagintacentillion", //                    3528                      1175
            "milliseseptuagintacentillion", //                        3531                      1176
            "milliseptenseptuagintacentillion", //                 3534                      1177
            "millioctoseptuagintacentillion", //                    3537                       1178
            "millinovenseptuagintacentillion", //                 3540                       1179
            "millioctogintacentillion", //                              3543                       1180
            "milliunoctogintacentillion", //                          3546                       1181
            "milliduooctogintacentillion", //                        3549                       1182
            "millitresoctogintacentillion", //                        3552                       1183
            "milliquattuoroctogintacentillion", //                3555                       1184
            "milliquinoctogintacentillion", //                      3558                       1185
            "millisexoctogintacentillion", //                        3561                       1186
            "milliseptemoctogintacentillion", //                  3564                       1187
            "millioctooctogintacentillion", //                      3567                       1188                                                  
            "millinovemoctogintacentillion", //                  3570                       1189
            "millinonagintacentillion", //                            3573                       1190
            "milliunnonagintacentillion", //                        3576                       1191
            "milliduononagintacentillion", //                      3579                       1192
            "millitrenonagintacentillion", //                        3582                       1193
            "milliquattuornonagintacentillion", //               3585                       1194
            "milliquinnonagintacentillion", //                     3588                       1195
            "millisenonagintacentillion", //                         3591                       1196
            "milliseptenonagintacentillion", //                    3594                       1197
            "millioctononagintacentillion", //                     3597                       1198
            "millinovenonagintacentillion", //                    3600                       1199
            "milliducentillion" //                                        3603                       1200
/*         Re: https://kyodaisuu.github.io/illion/10000.html
            "milliunducentillion"                                       3606                       1201
            ...
            "millinovenonagintanongentillion"                 6000                                             */
        }; // End of s_shortScaleIlliNames
        #endregion s_shortScaleIlliNames
        public static ushort? s_lengthOfIntegerPart;
        public static string?
        s_integerPart,
        s_fractionalPart;
        public static bool // If private, not accessible at top-level.
        s_numberIsNegative,
         s_scaleSpecificationIsRequired,
        s_longScaleIsSpecified,
        s_numberIsDecimalFraction,
        s_ordinalIsApplicable,
        s_andInsertionIsApplicable,
        s_andInsertionForPseudo_scientificIsApplicable,
        s_andInsertionIsSpecified,
        s_aRepresenting1IsApplicable,
        s_aRepresenting1IsSpecified,
        s_aRepresenting1ForPseudo_scientificIsApplicable,
        s_substituting100For1000IsApplicable,
        s_substituting100For1000IsSpecified,
        s_pseudo_scientificFormIsApplicable;
/*     If integer part length > 9, expression must specify scale, long or short.
        Symbols used in comments
        ®               registered trademark
        ⏎              carriage return
        ¶               paragraph
        §              section
        ⇒             yields, transforms into, maps to
        ⬇              bold down arrow
        ⤋                down arrow with triple stem
            ▎             bold vertical bar
        ║               double stem vertical bar
        ≠                unequal
        ≥                greater than or equal to 
        ≤                less than or equal to
      | x |               absolute value of x
        ×                times, multiply by
        ≡                congruent (with respect to a modulus)
        ≅                is approximately equal to
        ≪               much less than
        ¬                not
        ˅                or
        ˄                and
        ∃                there exists
        ∄                there does not exist, there exists no 
        ⇔              is logically equivalent to
        {x, y, z}     the set containing the members (or elements) x, y, and z
        x ∈ S         x is a member of the set S.
        y ∉ S         y is not a member of the set S.
        T ⊆ S        T is a subset of S
        U ⊊  S       U is a proper (or strict) subset of S 
        R ⊇ S        R is a superset of S
        Q ⊋ S        Q is a proper (or strict) superset of S 
        ∴               Therefore, thus
        ...               and so forth; additional words are omitted.
        |                 such that
        ms             millisecond
        ℤ               the set of integers
        ℤ₊, ℤ*      the set of positive integers (excludes 0)
        ℤˍˍ            the set of negative integers (excludes 0)
        ℤ≤₀           the set of nonpositive integers (includes 0)DetermineE
        ℤ≥₀, ℕ₀,   the set of nonnegative integers (includes 0)
        ℤˍ*           
        Note that the natural numbers are conventionally defined as either:
            1) the set of nonnegative integers (includes 0)
            This concords with the standard ISO 80000-2.
            or, alternatively 
            2) the set of positive integers (excludes 0)
        Definition 1 will be used herein, since this is an ISO standard,
        and since the set of nonnegative integers, along with the decimal
        numbers, is what is represented by the decimal numeral system.
        Re: https://en.wikipedia.org/wiki/Decimal
        for a treatment of the decimal numeral system                                             
        ------------------------------------------------------------------------------------------------------  */
        #region Helper methods
        public static void Wait(ushort seconds)
            // Value of seconds is interpreted as milliseconds.
            => Thread.Sleep(1000 * seconds);
/*    The system of latinate illi names (million, milliard, trillion, etc.) denotes integers 
        that are powers n of 10, where n is divisible by 3.  It is adapted from Conway, John H. and 
        Guy, Richard K. "The Book of Numbers", 1996 Springer-Verlag New York, Inc., p. 15
        https://en.wikipedia.org/wiki/Cardinal_numeral                                                                                          */
        public static string GetLatinateCardinalNumeralFor1DigitInteger(string decimalNumeral)
        {
            byte? numericalValue = byte.Parse(decimalNumeral);
            return numericalValue switch
            {
/*             Values for 2, 3, 4, 6, 7, 8, and 9 are stems and are subject to modification in context. 
                The variant "quinqua" for 5 is used with fifty "quinquagenta".                                                                                                                             */
                1 => "un",
                2 => "duo",
                3 => "tre",
                4 => "qua",
                5 => "quin",
                6 => "ses",
                7 => "septe",
                8 => "oct",
                9 => "nove",
                _ => throw new ArgumentOutOfRangeException($"The integer argument " +
                        $"{TheEnglishCardinalNumeralForTheInteger(decimalNumeral)} " +
                            "is outside the correct range of one to nine."),
            };
        } // End of GetLatinateCardinalNumeralFor1DigitInteger
        public static string TheLatinateCardinalNumeralForThe1DigitInteger(string decimalNumeral)
            => GetLatinateCardinalNumeralFor1DigitInteger(decimalNumeral);
        public static string
            TransformSpellingOfLatinate1DigitCardinalNumeral(string decimalNumeral, string suffix)
        {
            byte? numericalValue = byte.Parse(decimalNumeral);
            string? subTenName =
                TheLatinateCardinalNumeralForThe1DigitInteger(decimalNumeral);
            // These rules do not apply to 1-digit numbers prepended to multiples of 10 and 100.
            // "un" is never transformed.
            if (numericalValue is 1) { }
            else if (numericalValue is 2)
            {
                if ((suffix[0] is 'c') && (suffix[1] is not 'e'))
                    // duo ⇒ du
                    subTenName = subTenName[..^1];
            }
            else if (numericalValue is 3)
            {
                if ((suffix[0] is not 'd') && (suffix[0] is not 'n') && (suffix[0] is not 's'))
                    // tre ⇒ tres
                    subTenName += 's';
            }
            else if (numericalValue is 4)
            {
                if (suffix[..2] is "gi")
                    // qua ⇒ quadra
                    subTenName += "dra";
                else if (suffix[..2] is "ge")
                    // qua ⇒ quadrin
                    subTenName += "drin";
                else
                    // qua ⇒ quattuor
                    subTenName += "ttuor";
            }
            else if (numericalValue is 5) { }
            else if (numericalValue is 6)
            {
                if ((suffix[0] is 'c') || (suffix[0] is 'o'))
                {
                    // ses ⇒ se ⇒ sex
                    subTenName = subTenName[..^1] + 'x';
                }
                else if ((suffix[0] is 'd') || (suffix[0] is 'n') || (suffix[0] is 's'))
                    // ses ⇒ se 
                    subTenName = subTenName[..^1];
            }
            else if (numericalValue is 7)
            {
                if ((suffix[0] is 'o') || (suffix[0] is 'v'))
                    // septe ⇒ septem
                    subTenName += 'm';
                // before n septe is unchanged.                            
                else if (suffix[0] is not 'n')
                    // before d, s, t  septe ⇒ septen
                    subTenName += 'n';
            }
            else if (numericalValue is 8)
            {
                if (suffix[0] is 'g')
                    // oct ⇒ octin
                    subTenName += "in";
                else
                    // oct ⇒ octo
                    subTenName += 'o';
            }
            else if (numericalValue is 9)
            {
                if ((suffix[0] is 'o') || (suffix[0] is 'v'))
                    // nove ⇒ novem
                    subTenName += 'm';
                else if (suffix[0] is 'g')
                {
                    // nove ⇒ non
                    subTenName = subTenName[..2] + 'n';
                }
                else if (suffix[0] is not 'n')
                    // before d, q, s, t  nove ⇒ noven
                    subTenName += 'n';
            }
            else
            {
                throw new ArgumentOutOfRangeException($"The integer value " +
                    $"{TheEnglishCardinalNumeralForTheInteger(decimalNumeral)} " +
                        "is outside the correct range of one to nine.");
            }
            return subTenName;
        } // End of TransformSpellingOfLatinate1DigitCardinalNumeral
        public static string
            TheLatinate1DigitCardinalNumeralWithTransformedSpellingFor
                (string decimalNumeral, string suffix)
                    => TransformSpellingOfLatinate1DigitCardinalNumeral(decimalNumeral, suffix);
        public static string GetLatinateCardinalNumeralFor10Multiple(string decimalNumeral)
        {
            byte? numericalValue = byte.Parse(decimalNumeral);
            return numericalValue switch
            {
                1 => "deci", // 10
                2 => "viginti", // 20...
                3 => "triginta",
                4 => "quadraginta",
                5 => "quinquaginta",
                6 => "sexaginta",
                7 => "septuaginta",
                8 => "octoginta",
                9 => "nonaginta", // 90
                _ => throw new ArgumentOutOfRangeException($"The integer argument " +
                            $"{TheEnglishCardinalNumeralForTheInteger(decimalNumeral)} " +
                                "is outside the correct range of one to nine."),
            };
        } // End of GetLatinateCardinalNumeralFor10Multiple
        public static string TheLatinateCardinalNumeralForThe10Multiple(string decimalNumeral)
            => GetLatinateCardinalNumeralFor10Multiple(decimalNumeral);
        public static string GetLatinateCardinalNumeralFor2DigitInteger(string decimalNumeral)
        {
            byte? numericalValue = byte.Parse(decimalNumeral);
            ushort? digitCount = (ushort?)decimalNumeral.Length;
            // Check whether index's length is incorrect.  If so, throw an exception.   
            if (digitCount is not 2)
            {
                BackgroundColor = White;
                ForegroundColor = DarkRed;
                throw new ArgumentOutOfRangeException($"The digit count " +
                    $"{TheEnglishCardinalNumeralForTheInteger(digitCount.ToString())} " +
                        "is unequal to the correct count of two.");
            }
            string? cardinalNumeral;
            switch (numericalValue)
            {
                case 10: cardinalNumeral = "decilli"; break;
                case 11: cardinalNumeral = "undecilli"; break;
                case 12: cardinalNumeral = "duodecilli"; break;
                case 13: cardinalNumeral = "tredecilli"; break;
                case 14: cardinalNumeral = "quattuordecilli"; break; // 14
                case 15: cardinalNumeral = "quindecilli"; break;
                case 16: cardinalNumeral = "sedecilli"; break;
                case 17: cardinalNumeral = "septendecilli"; break;
                case 18: cardinalNumeral = "octodecilli"; break;
                case 19: cardinalNumeral = "novendecilli"; break;
                case 20: cardinalNumeral = "vigintilli"; break; // E.g. unvigintilli 21
                case 30: cardinalNumeral = "trigintilli"; break;
                case 40: cardinalNumeral = "quadragintilli"; break;
                case 50: cardinalNumeral = "quinquagintilli"; break;
                case 60: cardinalNumeral = "sexagintilli"; break;
                case 70: cardinalNumeral = "septuagintilli"; break;
                case 80: cardinalNumeral = "octogintilli"; break;
                case 90: cardinalNumeral = "nonagintilli"; break;
                default:
                    // Handle index ∈ {21-29, 31-39, ... 91-99}.
                    string? // E.g. index is 21
                            //                 "2"
                    decimalNumeral_s1stCharAsString = decimalNumeral[..1],
                    //                "20"
                    decimalNumeral_s1stCharWith0Appended = decimalNumeral_s1stCharAsString + "0",
                    //                 "1"
                    decimalNumeral_s2ndCharAsString = decimalNumeral[1..2],
                    //       1                                         "1"
                    subTenNumeral = decimalNumeral_s2ndCharAsString,
                    //         20                                                 "20"
                    tenMultipleNumeral = decimalNumeral_s1stCharWith0Appended,
                    tenMultipleName =
                        //                            "viginti"                                                  20
                        TheLatinateCardinalNumeralForThe2DigitInteger(tenMultipleNumeral),
                    subTenName =
                        TheLatinate1DigitCardinalNumeralWithTransformedSpellingFor
                            //         1                      "viginti" 
                            (subTenNumeral, tenMultipleName);
                    //                                   "un"                  "viginti"
                    cardinalNumeral = subTenName + tenMultipleName;
                    break;
            }; // End of switch 
            return cardinalNumeral;
        } // End of GetLatinateCardinalNumeralFor2DigitInteger
        public static string TheLatinateCardinalNumeralForThe2DigitInteger(string decimalNumeral)
            => GetLatinateCardinalNumeralFor2DigitInteger(decimalNumeral);
        public static string GetLatinateCardinalNumeralFor100Multiple(string decimalNumeral)
        {
            byte? numericalValue = byte.Parse(decimalNumeral);
            return numericalValue switch
            {
                1 => "centilli", // 100
                2 => "ducentilli", // 200...
                3 => "trecentilli",
                4 => "quadringentilli",
                5 => "quingentilli",
                6 => "sescentilli",
                7 => "septingentilli",
                8 => "octingentilli",
                9 => "nongentilli", // 900
                _ => throw new ArgumentOutOfRangeException($"The integer argument " +
                            $"{TheEnglishCardinalNumeralForTheInteger(decimalNumeral.ToString())} " +
                                "is outside the correct range of one to nine."),
            };
        } // End of GetLatinateCardinalNumeralFor100Multiple
        public static string TheLatinateCardinalNumeralForThe100Multiple(string decimalNumeral)
            => GetLatinateCardinalNumeralFor100Multiple(decimalNumeral);
        public static string GetLatinateCardinalNumeralFor12Or3DigitInteger
            (string decimalNumeral)
        {
            string? illiName;
            ushort?
            numericalValue = ushort.Parse(decimalNumeral),
            indexLength = (ushort?)decimalNumeral.Length;
            if (indexLength > 3)
                throw new Exception();
            if (indexLength is 1)
                // "milli", "millinilli" ... "nonilli"
                illiName = TheLatinateCardinalNumeralForThe1000Multiple(decimalNumeral);
            else if (indexLength is 2)
            {
                //                                       nameIndex: 23 "tresvigintillion"  
                illiName = TheLatinateCardinalNumeralForThe2DigitInteger(decimalNumeral);
            }
/*                 Applies to indexLength values 1, 2, or 3.  Note: hyphens will not be included.
                    in the final expression. 
            nameIndex    divideBy100Remainder  divideBy100Remainder % 10            illi Name         Mnemonics                  
                     0                            -                                            -                                        nilli
                     3                            -                                            -                                        trilli
                    50                           -                                            -                                  quinquagintilli
                   103                           3                                           -                                     tres-centilli      's' is sum.
                   300                           0                                           0                                     tre-centilli       Concatenation is multiplication.                        
                   301                           1                                           1                                un-trecentilli                          
                   320                         20                                           0                             viginti-trecentilli                     
                   324                         24                                           4                          quattuor-viginti-trecentilli  
                                illiName = TheConcatenationOf(unitsPart, _10MultiplePart,  _100MultiplePart);                                     */
            else if (indexLength is 3)
            {
/*             The example values are for nameIndex = 324, for which illionName                         
                is quattuor-viginti-trecentillion (4-20-300). Note: hyphens will not be included
                in the final expression.                                                                                                     */
                byte?
                //           24                                                    324       24 
                divideBy100Remainder = (byte?)(numericalValue % 100),
                //         4                                           24                    4
                unitsPartValue = (byte?)(divideBy100Remainder % 10),
                //               2                                                      24              2
                _10MultiplePartValue = (byte?)(divideBy100Remainder / 10),
                //                 3                                            324          3
                _100MultiplePartValue = (byte?)(numericalValue / 100);
                string?
                _10MultiplePart = _10MultiplePartValue is not 0 ?
                    TheLatinateCardinalNumeralForThe10Multiple(_10MultiplePartValue.ToString())
                    :
                    string.Empty,
                // trecentilli (300)                      3
                _100MultiplePart = _100MultiplePartValue is not 0 ?
                    TheLatinateCardinalNumeralForThe100Multiple(_100MultiplePartValue.ToString())
                    :
                    string.Empty,
                //                                    viginti (20)           trecentilli (300)
                illiNameRightPart = _10MultiplePart + _100MultiplePart,
                unitsPart = unitsPartValue is not 0 ?
                    TheLatinate1DigitCardinalNumeralWithTransformedSpellingFor
                        (unitsPartValue.ToString(), illiNameRightPart)
                    :
                    string.Empty;
                //               quattuor (4)  vigintitrecentilli (320)
                illiName = unitsPart + illiNameRightPart;
            } // End of else if (indexLength is 3)
            // indexLength is 0 or > 3.
            else
            {
                throw new ArgumentOutOfRangeException($"indexLength " +
                    $"{TheEnglishCardinalNumeralForTheInteger(indexLength.ToString())} " +
                        "is outside the correct range of one to three.");
            }
            return illiName;
        } // End of GetLatinateCardinalNumeralFor12Or3DigitInteger
        public static string TheLatinateCardinalNumeralForThe12Or3DigitInteger
            (string decimalNumeral)
            => GetLatinateCardinalNumeralFor12Or3DigitInteger(decimalNumeral);
        public static string GetLatinateCardinalNumeralFor1000Multiple(string decimalNumeral)
        {
            byte? numericalValue = byte.Parse(decimalNumeral);
            return numericalValue switch
            { //                        Power of 10
                0 => "nilli", //          3 
                1 => "milli", //         6
                2 => "billi", //          9
                3 => "trilli", //        12
                4 => "quadrilli", // 15
                5 => "quintilli", //  18
                6 => "sextilli", //    21
                7 => "septilli", //    24
                8 => "octilli", //      27
                9 => "nonilli", //     30
                _ => throw new ArgumentOutOfRangeException($"The integer argument " +
                            $"{TheEnglishCardinalNumeralForTheInteger(decimalNumeral.ToString())} " +
                                "is outside the correct range of zero to nine."),
            };
        }
        public static string TheLatinateCardinalNumeralForThe1000Multiple(string decimalNumeral)
            => GetLatinateCardinalNumeralFor1000Multiple(decimalNumeral);
/*     This applies to short and long scale, and accords with the Conway-Wechsler system, as refined 
        by Olivier Miakinen.  
        Re: http://www.miakinen.net/vrac/zillions

        The "short scale" (SS) is the system of illion names used in the U.S., U.K., etc.  In this system 
        10^9, 1000 * 1000 * 1000, is called "billion", while in the "long scale" (LS), used in much of
        Europe and elsewhere, it is called "milliard".
        With SS illion names always (except for "thousand") end with -on, while with LS they
        end alternately with -on and -ard.
        nameIndex examples (short scale): 0: thousand, 1: million, 2: billion
        For indices greater than 999 the group name will have more than one occurrence of "illi".
        --------------------------------------------------------------------------------------------
        A          B     	       C			            D				 value              group name            				     
        nameIndex            suffix           power of 10 	                      SS              LS
        SS	 	   LS              LS	                                                      
                                0:"on" 1:"ard"
        ——————————————————————————————---
        0	 	    0			        -	 			       3			    10 ^  3	      thousand     thousand
        1	 		1			        0	 			       6			    10 ^  6	      million		  million
        2	 		1			        1		 		       9               10 ^  9	      billion		  milliard
        3	 		2			        0		 		     12               10 ^ 12 	  trillion		  billion
        4	 	    2			        1		 		     15               10 ^ 15		  quadrillion	  billiard
        5	 	    3			        0		 	  	     18			    10 ^ 18		  quintillion   trillion
        6	 	    3			        1		 		     21 		        10 ^ 21		  sextillion	  trilliard
        --------------------------------------------------------------------------------------------
        "id": integer division, where remainders are ignored and are not calculated.
        "sd": standard division.
        --------------------------------------------------------------------------------------------
        SS  
        A = (D - 3) / 3   true for id, sd
        D = (3 * A) + 3 
        ——————-----------------
        LS
        B = (A+1) / 2 true for id only
        B = (((D - 3) / 3) + 1 ) / 2 true for id only
        C = D % 2 = (3A + 3) % 2
        D = 6 * B + 3 * C
        The return value will not contain any spaces or other punctuations, and will
        contain an "on" or "ard" as a suffix.
        million, milliard, quadrillion, etc.
                                                Structure of a group name
                            1st illi group ... nth illi group (Where n is any positive integer.)
                                                Structure of an illi group
                        Each subgroup has a latinate name for an integer representing an index from 0 to 999
                                        0: nilli; 1: milli; 2: billi                                     
                                                                                    index    SS value
                            "milli"                                                 1       10 ^     6
                            "nonilli"                                              9       10 ^   30
                            "sestrigintilli"                                   36       10 ^  111
                            "septensexagintatrecentilli"            367      10 ^ 1104
                            "millinillion"                                 1000      10 ^ 3003
                            "millimillion"                                1001      10 ^ 3006

        index = (SS exponent / 3) - 1
        SS exponent = 3 * (index + 1)                                                                                                                              */
        public static string
            GetLatinateIlliNameFor10ToPowerMultipleOf3(string decimalNumeral)
        {
            ushort? numericalValue = ushort.Parse(decimalNumeral);
            if (numericalValue is 0)
                // Exceptional for having a non-latinate name.
                return "thousand";
            // nameIndex > 0.
            else
            {
                ushort? localizedNameIndex;
                if (s_longScaleIsSpecified)
                    localizedNameIndex = (ushort?)((numericalValue + 1) / 2);
                else 
                    localizedNameIndex = numericalValue;
                string?
                // Will contain one or more instances of "illi". "illiGroup" is a word like billion or millinillion.
                illiGroup = string.Empty,
                indexAsString = localizedNameIndex.ToString(),
                suffix = string.Empty;
                if (s_longScaleIsSpecified)
                {
                    if ((3 * (numericalValue + 1)) % 2 is 0)
                        suffix = "on";
                    else
                        suffix = "ard";
                }
                else 
                    suffix = "on";
                ulong? indexLength = IsNullOrEmpty(indexAsString) is false ?
                    (ulong?)indexAsString.Length : 0;
                // nameIndex ≤ 999                                                                                                               
                if (indexLength <= 3)
                {
                    // Just one "illi" and one "on" or "ard" will be returned.
                    return TheConcatenationOf(TheLatinateCardinalNumeralForThe12Or3DigitInteger
                        (localizedNameIndex.ToString()), suffix);
                }
/*             Starting from the right, indexAsString is partitioned into groups of
                three digits.  Each group is assigned a latinate phrase (billion, trilliard,
                novenonagintanongentillion (The value of this stem is 999, with individual
                values in the reverse order of those in English.), etc.) with "illi" as suffix,
                and so on, moving to the left until the leftmost group is encountered.  This
                will have 1, 2, or 3 digits.

                indexLength > 3  More than one "illi" is required.  E.g."millinillion", 10^3003, index = 1000                   */
                else
                {
                    string?
                    // In indexAsString the groups which are not the leftmost will contain three digits.
                    currentGroupOf1_2_Or3Digits,
                    currentIlliGroupForIndexUnder1000;
                    /*                 Initialized to the index of the rightmost character in indexAsString.                                    */
                    short? digitPointer = (short?)(indexLength - 1);
                    // This will run repeatedly, adding a new illi phrase each time.
                    do
                    {
                        currentGroupOf1_2_Or3Digits = digitPointer >= 3 ?
                            // Get groups other than the leftmost.
                            indexAsString[(int)(digitPointer - 2)..(int)(digitPointer + 1)]
                            :
                            // Get the leftmost group. digitPointer is 0, 1, or 2.
                            indexAsString[..(int)(digitPointer + 1)];
                        currentIlliGroupForIndexUnder1000 =
                            TheLatinateCardinalNumeralForThe12Or3DigitInteger
                                (currentGroupOf1_2_Or3Digits);
                        illiGroup = // A group with multiple illis will be formed.
                            TheConcatenationOf(currentIlliGroupForIndexUnder1000, illiGroup);
                        digitPointer -= 3;
                    } while (digitPointer >= 0);
                } // End of else indexLength > 3     "on" or "ard"            
                return TheConcatenationOf(illiGroup, suffix);
            } // End of else nameIndex is not 0
        } // End of GetLatinateCardinalNumeralFor10ToPowerMultipleOf3
        public static string TheLatinateIlliNameFor10ToPowerMultipleOf3(string decimalNumeral)
            => GetLatinateIlliNameFor10ToPowerMultipleOf3(decimalNumeral);
/*     The following methods with names containing the phrase "GetNameOfInteger" 
        express nonnegative cardinal numbers.
        https://en.wikipedia.org/wiki/Cardinal_numeral                                                                                      */
        // *************************************************************************

/*     E.g. 3,050 ⇒ three point zero five thousand  2500.1 ⇒ two point five zero zero one thousand
        Negative numbers may be expressed in this form.                                                                            */
        public static string ExpressNumberInPseudo_scientificFormWithSignificandAsWords
            (
                // If the number to be expressed is nonnegative, string.Empty is passed in.
                string negativePrefix,
                string integerPartOfNormalForm,
/*             "The fractional part or decimal part of a non‐negative real number x
                is the excess beyond that number's integer part."
                See: https://en.wikipedia.org/wiki/Fractional_part
                If the number to be expressed is an integer, pass in string.Empty.                                                          */
                string fractionalPartOfNormalForm
            )
        {
/*         For a definition of significant digits see https://en.wikipedia.org/wiki/Significant_figures
            However, note that in the Talk section of this article the scientific status of the concept
            of significant figures is called into question.
            See https://en.wikipedia.org/wiki/Talk:Significant_figures#This_article_is_terribly_misleading         */
            ushort?
            lengthOfIntegerPartOfNormalForm =
                (ushort?)integerPartOfNormalForm.Length,
            //                           Value of expression ≅ lengthOfIntegerPartOfNormalForm / 3
            exponent = (ushort)(((lengthOfIntegerPartOfNormalForm - 1) / 3) - 1);
            //                             Value is 1, 2, or 3.                                                                                                          
            byte? lengthOfIntegerPartOfPseudo_scientificForm =
                (byte?)(((lengthOfIntegerPartOfNormalForm - 4) % 3) + 1);
            string?
            // illiName is a word like million or billiard.
            illiName = TheLatinateIlliNameFor10ToPowerMultipleOf3(exponent.ToString()),
            integerPartOfPseudo_scientificFormAsDigits =
                integerPartOfNormalForm[..(int)lengthOfIntegerPartOfPseudo_scientificForm],
            fractionalPartOfPseudo_scientificFormAsDigits =
                fractionalPartOfNormalForm != string.Empty ?
                    TheConcatenationOf(integerPartOfNormalForm
                        [(int)lengthOfIntegerPartOfPseudo_scientificForm..], fractionalPartOfNormalForm)
                    :
                    // fractionalPartOfNormalForm is string.Empty, so trailing 0s are deleted.
                    integerPartOfNormalForm
                        [(int)lengthOfIntegerPartOfPseudo_scientificForm..].TrimEnd('0');
/*         indexOfLastNon0Digit is 2.
            Definition: "significand refers to the first (leftmost) part of a number in scientific
            notation ... "
            From: https://en.wikipedia.org/wiki/Significand
            Consider a number in scientific notation, such as 15.98 × 10³, representing the integer
            15,980. 15.98 is the significand.  We will here define "integer part" in pseudo-scientific
            expressions as the number to the left of the word "point".  The length of the multiplier may be
            1, 2, or 3; in this example it is 2, and the digit count is 5.                                                            */
            if
                (
                    fractionalPartOfNormalForm == string.Empty
                    &&
                    // Variable is a string of 0s.
                    fractionalPartOfPseudo_scientificFormAsDigits.TrimEnd('0') == string.Empty
                    &&
                    // Variable does not end with "0".
                    integerPartOfPseudo_scientificFormAsDigits[^1..] != "0"
                )
            {
                // Variable consisting of a string of 0s ⇒ single 0.    
                fractionalPartOfPseudo_scientificFormAsDigits = "0";
            }
            string?
            integerPartOfPseudo_scientificFormAsName =
                TheEnglishCardinalNumeralForThe12Or3DigitInteger
                    (integerPartOfPseudo_scientificFormAsDigits),
            fractionalPartOfPseudo_scientificFormAsName = string.Empty;
            ushort? lengthOfFractionalPartOfPseudo_scientificFormAsDigits =
                (ushort?)fractionalPartOfPseudo_scientificFormAsDigits.Length;
            for (var i = 0; i < lengthOfFractionalPartOfPseudo_scientificFormAsDigits; i++)
            {
                fractionalPartOfPseudo_scientificFormAsName =
                    TheConcatenationOf(fractionalPartOfPseudo_scientificFormAsName, Space,
                      TheEnglishCardinalNumeralForThe1DigitInteger
                             (fractionalPartOfPseudo_scientificFormAsDigits[i..(i + 1)])).TrimStart();
            }
            return TheConcatenationOf((negativePrefix + Space).TrimStart(),
                integerPartOfPseudo_scientificFormAsName, Space, "point", Space,
                    fractionalPartOfPseudo_scientificFormAsName, Space, illiName);
        } // End of ExpressNumberInPseudo_scientificFormWithSignificandAsWords
        public static string ThePseudo_scientificExpressionWithSignificandAsWordsOf
            (
                string negativePrefix,
                string integerPartOfNormalForm,
                string fractionalPartOfNormalForm
            )
            => ExpressNumberInPseudo_scientificFormWithSignificandAsWords
                    (negativePrefix, integerPartOfNormalForm, fractionalPartOfNormalForm);

/*     E.g. 3,050 ⇒ 3.05 thousand  2500.1 ⇒ 2.5001 thousand
        Negative numbers may be expressed in this form.
        These expressions do not include "and".                                                                                            */
        public static string ExpressNumberInPseudo_scientificFormWithSignificandAsDigits
            (
                string integerPartOfNormalForm,
/*             "The fractional part or decimal part of a non‐negative real number x
                is the excess beyond that number's integer part."
                See: https://en.wikipedia.org/wiki/Fractional_part
                If the number to be expressed is an integer, pass in string.Empty.                                                          */
                string fractionalPartOfNormalForm
            )
        {
/*         For a definition of significant digits see https://en.wikipedia.org/wiki/Significant_figures
            However, note that in the Talk section of this article the scientific status of the concept
            of significant figures is called into question.
            See https://en.wikipedia.org/wiki/Talk:Significant_figures#This_article_is_terribly_misleading         */
            ushort?
            lengthOfIntegerPartOfNormalForm =
                (ushort?)integerPartOfNormalForm.Length,
            //                           Value of expression ≅ lengthOfIntegerPartOfNormalForm / 3
            exponent = (ushort)(((lengthOfIntegerPartOfNormalForm - 1) / 3) - 1);
            //                             Value is 1, 2, or 3.                                                                                                          
            byte? lengthOfIntegerPartOfPseudo_scientificForm =
                (byte?)(((lengthOfIntegerPartOfNormalForm - 4) % 3) + 1);
            string?
            // illiName is a word like million or billiard.
            illiName = TheLatinateIlliNameFor10ToPowerMultipleOf3(exponent.ToString()),
            integerPartOfPseudo_scientificFormAsDigits =
                integerPartOfNormalForm[..(int)lengthOfIntegerPartOfPseudo_scientificForm],
            fractionalPartOfPseudo_scientificFormAsDigits =
                fractionalPartOfNormalForm != string.Empty ?
                    TheConcatenationOf(integerPartOfNormalForm
                        [(int)lengthOfIntegerPartOfPseudo_scientificForm..], fractionalPartOfNormalForm)
                    :
                    // fractionalPartOfNormalForm is string.Empty, so trailing 0s are deleted.
                    integerPartOfNormalForm
                        [(int)lengthOfIntegerPartOfPseudo_scientificForm..].TrimEnd('0');
/*         indexOfLastNon0Digit is 2.
            Definition: "significand refers to the first (leftmost) part of a number in scientific
            notation ... "
            From: https://en.wikipedia.org/wiki/Significand
            Consider a number in scientific notation, such as 15.98 × 10³, representing the integer
            15,980. 15.98 is the significand.  We will here define "integer part" in pseudo-scientific
            expressions as the number to the left of the period.  The length of the multiplier may be
            1, 2, or 3; in this example it is 2, and the digit count is 5.                                                                              */
            if
                (
                    fractionalPartOfNormalForm == string.Empty
                    &&
                    // Variable is a string of 0s.
                    fractionalPartOfPseudo_scientificFormAsDigits.TrimEnd('0') == string.Empty
                    &&
                    // Variable does not end with "0".
                    integerPartOfPseudo_scientificFormAsDigits[^1..] != "0"
                )
            {
                // Variable consisting of a string of 0s ⇒ single 0.    
                fractionalPartOfPseudo_scientificFormAsDigits = "0";
            }
            string negativePrefix = s_numberIsNegative ? MinusSignString : string.Empty;
            return TheConcatenationOf(negativePrefix, integerPartOfPseudo_scientificFormAsDigits,
                Period, fractionalPartOfPseudo_scientificFormAsDigits, Space, illiName);
        } // End of ExpressNumberInPseudo_scientificFormWithSignificandAsDigits
        public static string ThePseudo_scientificExpressionWithSignificandAsDigitsOf
            (
                string integerPartOfNormalForm,
                string fractionalPartOfNormalForm
            )
            => ExpressNumberInPseudo_scientificFormWithSignificandAsDigits
                    (integerPartOfNormalForm, fractionalPartOfNormalForm);

        /*     Constraints on engineering notation: The exponent is a multiple of 3; the part of the
                expression preceding the period has a value n | 1 ≤ | n | < 1000.
                Method and commentary for emgineering notation adapted from the result given by a query
                submitted at https://chatgpt.com.
                Explanation:
                1. Exponent Calculation:
                First calculate the base 10 logarithm of the absolute value of the number using Log10().
                This is then divided by 3 to determine how far to scale the number to get it between 1 and
                1000.  The result is then divided by 3 and is used as the exponent, which is the power of 10
                to scale the number.
                2. Scaling:
                The number is then scaled by dividing it by 10^exponent to ensure it falls within the desired range.
                3. Formatting:
                The result is formatted to six decimal places ({scaledValue:0.000000}).
                The exponent is attached, following "e".

                In normalized scientific notation (called "standard form" in the United Kingdom), one 
                non-zero decimal digit m precedes the decimal point. 

                For both of these forms the exponent n is negative for a number with absolute value
                between 0 and 1.  e.g. 0.5 is written as 5e-1, i.e. has the value 5×10^-1.
                https://en.wikipedia.org/wiki/Scientific_notation#Normalized_notation
                Code adapted from:
                https://codepal.ai/code-generator/query/cBn6w81U/convert-standard-numbers-to-scientific-notation   */
        public static string ExpressNumberInNormalizedScientificNotation
            (
                string integerPart,
                string fractionalPart
            )
        {
            if ((integerPart is "0") && (fractionalPart == string.Empty))
                return "0";
            double?
            inputAsDouble =
                double.Parse(TheConcatenationOf(integerPart, Period, fractionalPart));
            // exponent may be negative, and so have a leading minus sign.
            short? exponent = (short?)Floor(Log10(Abs((double)inputAsDouble)));
            double? mantissa = inputAsDouble / Pow(10, (double)exponent);
            string?
            polarityPrefix = s_numberIsNegative ? MinusSignString : string.Empty,
            expressionInScientificNotation =
                $"{polarityPrefix}{mantissa:0.000000}e{exponent}";
            return expressionInScientificNotation;
        } // End of ExpressNumberInNormalizedScientificNotation
        public static string TheNormalizedScientificNotationExpressionOf
            (
                string integerPart,
                string fractionalPart
            )
                => ExpressNumberInNormalizedScientificNotation(integerPart, fractionalPart);
        public static string ExpressNumberInEngineeringNotation
            (
                string integerPart,
                string fractionalPart
            )
        {
            if ((integerPart is "0") && (fractionalPart == string.Empty))
                return "0";
            double?
            inputAsDouble =
                double.Parse(TheConcatenationOf(integerPart, Period, fractionalPart));
            // exponent may be negative, and so have a leading minus sign.
            short? exponent = (short?)(Floor(Log10(Abs((double)inputAsDouble)) / 3) * 3);
            double? mantissa = inputAsDouble / Pow(10, (double)exponent);
            string?
            polarityPrefix = s_numberIsNegative ? MinusSignString : string.Empty,
            expressionInScientificNotation =
                $"{polarityPrefix}{mantissa:0.000000}e{exponent}";
            return expressionInScientificNotation;
        } // End of ExpressNumberInEngineeringNotation
        public static string TheEngineeringNotationExpressionOf
            (
                string integerPart,
                string fractionalPart
            )
                => ExpressNumberInEngineeringNotation(integerPart, fractionalPart);
/*     Words that form the basis for representations of integers are generated in the following methods.
        For representations of negative numbers the suffix “minus” or “negative” will be affixed 
        elsewhere in the program.                                                                                                               
        The following two methods are adapted from those in an article by Fred Byamugisha posted at
        https://www.codeproject.com/articles/15934/how-to-convert-a-numeric-value-or-currency-to-engl
        Definition: "A decimal numeral (also often just decimal or, less correctly, decimal number), 
        refers generally to the notation of a number in the decimal numeral system." 
        From: https://en.wikipedia.org/wiki/Decimal
        https://en.wikipedia.org/wiki/Cardinal_numeral                                                                                              */
        public static string
            GetEnglishCardinalNumeralFor1DigitInteger(string decimalNumeral)
        {
            byte? digitCount = (byte?)decimalNumeral.Length;
            // Check whether decimalNumeral's length is incorrect.  If so, throw an exception.  
            if (digitCount is not 1)
            {
                BackgroundColor = White;
                ForegroundColor = DarkRed;
                throw new ArgumentOutOfRangeException($"The digit count " +
                    $"({TheEnglishCardinalNumeralForTheInteger(digitCount.ToString())}) " +
                        $"is unequal to the correct count of one.");
            }
            byte? numericalValue = byte.Parse(decimalNumeral);
            return numericalValue switch
            {
                0 => "zero",
                1 => "one",
                2 => "two",
                3 => "three",
                4 => "four",
                5 => "five",
                6 => "six",
                7 => "seven",
                8 => "eight",
                9 => "nine",
                _ => throw new NotImplementedException(),
            }; // End of switch
        } // End of GetEnglishCardinalNumeralFor1DigitInteger
        public static string
           TheEnglishCardinalNumeralForThe1DigitInteger(string decimalNumeral)
                => GetEnglishCardinalNumeralFor1DigitInteger(decimalNumeral);
        //****************************************************************
        public static string
            GetEnglishCardinalNumeralFor2DigitInteger(string decimalNumeral)
        {
            byte? digitCount = (byte?)decimalNumeral.Length;
            if (digitCount is 1)
                return TheEnglishCardinalNumeralForThe1DigitInteger(decimalNumeral);
            // Check whether decimalNumeral's length is incorrect.  If so, throw an exception.   
            if (digitCount is not 2)
            {
                BackgroundColor = White;
                ForegroundColor = DarkRed;
                throw new ArgumentOutOfRangeException($"The digit count " +
                    $"{TheEnglishCardinalNumeralForTheInteger(digitCount.ToString())} " +
                        "is unequal to the correct count of two.");
            }
/*         digitCount is 2 
            This statement handles strings with an initial zero passed in when this method is called 
            from within theEnglishCardinalNumeralForTheDecimalNumeral or 
            theEnglishCardinalNumeralForThe3DigitInteger or from elsewhere.                                                                    */
            if (decimalNumeral[0] is '0')
                return TheEnglishCardinalNumeralForThe1DigitInteger(decimalNumeral[^1..]);
            byte? numericalValue = byte.Parse(decimalNumeral);
            return numericalValue switch
            {
                10 => "ten",
                11 => "eleven",
                12 => "twelve",
                13 => "thirteen",
                14 => "fourteen",
                15 => "fifteen",
                16 => "sixteen",
                17 => "seventeen",
                18 => "eighteen",
                19 => "nineteen",
                20 => "twenty",
                30 => "thirty",
                40 => "forty",
                50 => "fifty",
                60 => "sixty",
                70 => "seventy",
                80 => "eighty",
                90 => "ninety",
/*             Handle decimalNumeral ∈ {21-29, 31-39,... 91-99}, for which values a
                hyphen must be inserted.                                                                                                            */
                _ => TheConcatenationOf(TheEnglishCardinalNumeralForThe2DigitInteger
                            (decimalNumeral[..1] + "0"), Hyphen,
                                TheEnglishCardinalNumeralForThe1DigitInteger(decimalNumeral[1..2])),
            }; // End of switch
        } // End of GetEnglishCardinalNumeralFor2DigitInteger
        public static string
            TheEnglishCardinalNumeralForThe2DigitInteger(string decimalNumeral)
                => GetEnglishCardinalNumeralFor2DigitInteger(decimalNumeral);
/*     Words that form the basis for representations of integers are generated in this method.
        For representations of negative numbers the suffix “minus” or “negative” will be affixed 
        elsewhere in the program.                                                                                                               
        decimalNumeral may consist of three or fewer digits.                                                                           */
        public static string GetEnglishCardinalNumeralFor3DigitInteger(string decimalNumeral)
        {
            if (decimalNumeral is not "0")
                decimalNumeral = decimalNumeral.TrimStart(Zero);
            byte? digitCount = (byte?)decimalNumeral.Length;
            if (digitCount is 1)
                return TheEnglishCardinalNumeralForThe1DigitInteger(decimalNumeral);
            else if (digitCount is 2)
                return TheEnglishCardinalNumeralForThe2DigitInteger(decimalNumeral);
            // Check whether decimalNumeral's length > 3.  If so, throw an exception.
            else if (digitCount > 3)
            {
                throw new ArgumentOutOfRangeException($"The digit count " +
                    $"{TheEnglishCardinalNumeralForTheInteger
                        (digitCount.ToString())} exceeds the limit of three.");
            }
            // digitCount = 3
            else
            {
                bool? decimalNumeralIsA100Multiple = decimalNumeral[^2..] is "00";
                string?
                expressionOfInitial1 = (bool)s_aRepresenting1IsSpecified ? "a" : "one",
                _100multiplier = decimalNumeral[0] is '1' ?
                    expressionOfInitial1
                    :
                    TheEnglishCardinalNumeralForThe1DigitInteger(decimalNumeral[..1]),
                sub100NumberName = decimalNumeralIsA100Multiple is false ?
                    TheEnglishCardinalNumeralForThe2DigitInteger(decimalNumeral[^2..])
                    :
                    string.Empty,
                conjunction = string.Empty;
                if (decimalNumeralIsA100Multiple is false)
                    conjunction =
                        ((bool)s_andInsertionIsSpecified is true) && (sub100NumberName != string.Empty) ?
                            "and" : string.Empty;
                return _100multiplier + Space + "hundred" + (Space + conjunction).TrimEnd() +
                    (Space + sub100NumberName).TrimEnd();
            }  // End of else (digitCount = 3)      
        } // End of GetEnglishCardinalNumeralFor3DigitInteger 
        public static string TheEnglishCardinalNumeralForThe3DigitInteger(string decimalNumeral)
            => GetEnglishCardinalNumeralFor3DigitInteger(decimalNumeral);
        //****************************************************************
/*     Words that form the basis for representations of integers are generated in this method.
        For representations of negative numbers the suffix “minus” or “negative” will be affixed 
        elsewhere in the program.                                                                                                               */
        public static string
            GetEnglishCardinalNumeralFor12Or3DigitInteger(string decimalNumeral)
        {
            ushort? digitCount = (ushort?)decimalNumeral.Length;
            if (digitCount is 1)
                return TheEnglishCardinalNumeralForThe1DigitInteger(decimalNumeral);
            else if (digitCount is 2)
                return TheEnglishCardinalNumeralForThe2DigitInteger(decimalNumeral);
            else if (digitCount is 3)
                return TheEnglishCardinalNumeralForThe3DigitInteger(decimalNumeral);
            else
            {
                BackgroundColor = White;
                ForegroundColor = DarkRed;
                throw new ArgumentOutOfRangeException($"The digit count " +
                    $"({TheEnglishCardinalNumeralForTheInteger
                        (digitCount.ToString())}) is not in the range from 1 to 3.");
            }
        } // End of GetEnglishCardinalNumeralFor12Or3DigitInteger
        public static string
            TheEnglishCardinalNumeralForThe12Or3DigitInteger(string decimalNumeral)
                => GetEnglishCardinalNumeralFor12Or3DigitInteger(decimalNumeral);
        //************************************************************************
/*     This gets the English name for a string of digital characters representing a number n ∈ ℕ₀, 
        the set of natural numbers including '0'.  This is equivalent to ℤ≥₀, the set of 
        nonnegative integers.

        All commas alluded to in variable names are imaginary, in the sense that they are
        not included in the input string decimalNumeral.

        Definitions of decimal numeral do not specify whether the negative numbers are included.
        See https://en.wikipedia.org/wiki/Decimal

        Words that form the basis for representations of integers are generated in this method.
        For representations of negative numbers the prefix “minus” or “negative” will be affixed 
        elsewhere in the program.                                                                                                                          */
        public static string GetEnglishCardinalNumeralForInteger(string decimalNumeral)
        {
            decimalNumeral = decimalNumeral.WithOnly(Digits);
            ushort? digitCount = (ushort?)decimalNumeral.Length;
            if (digitCount <= 3)
                return TheEnglishCardinalNumeralForThe12Or3DigitInteger(decimalNumeral);
            if (digitCount is 4)
            {
/*             For examples see: Compiled Statutes of the United States, 1901
                re: https://books.google.com/books?id=sc-uwAB4_ZAC&pg=PA1273&lpg=PA1273&dq=twenty+hundred&source=bl&ots=jLg-pdzvND&sig=ACfU3U1VpDqm8QiIvWpjSZJ4rX7oZYtbGg&hl=en&sa=X&ved=2ahUKEwjtje6n7Mn7AhXYJUQIHUhIBgQQ6AF6BAg_EAM#v=onepage&q=twenty%20hundred&f=false             
                e.g. p. 1273: 5523 is expressed as "fifty-five hundred and twenty-three".  Here "hundred"
                takes the place of "thousand".                                                                                                              */
                s_substituting100For1000IsApplicable = true;
                if ((bool)s_substituting100For1000IsSpecified)
                {
                    if (decimalNumeral[^2..] is not "00")
                    {
                        string? conjunction1 = (bool)s_andInsertionIsSpecified ? "and" : string.Empty;
                        return (TheEnglishCardinalNumeralForThe2DigitInteger(decimalNumeral[..2]) +
                            Space + "hundred" + Space + conjunction1).TrimEnd() + Space +
                                TheEnglishCardinalNumeralForThe2DigitInteger(decimalNumeral[^2..]);
                    }
                    // decimalNumeral[^2..] is "00".
                    else
                    {
                        return TheEnglishCardinalNumeralForThe2DigitInteger
                                        (decimalNumeral[..2]) + Space +  "hundred";
                    }
                } // End of if (expressWithHundredNotThousand is true)
            } // End of if (digitCount is 4)
            // digitCount ≥ 4 
            string?
            englishCardinalNumeral = string.Empty,
            // Word ending in "illion" or "illiard"
            illiName,
            conjunction,
            expressionOfInitial1 = s_aRepresenting1IsSpecified ? "a" : "one",
            finalExpressionOfInitial1 = string.Empty;
            if (s_aRepresenting1IsSpecified is true)
            {
/*             digitCount:                    4, 5, 6 ⇒ "thousand";  7, 8, 9 ⇒ "million"; 10, 11, 12 ⇒ "billion" SS / "milliard" LS ...
                Illi name index:                 0                                  1                                  2
                ((digitCount - 1) / 3) - 1):  0                                  1                                  2                                                    
                ------------------------------------------------------------------------------------------------------------------------------------ */
                // Value of expression ≅ lengthOfIntegerPartOfNormalForm / 3
                ushort exponent = (ushort)((digitCount - 1) / 3 - 1);
                string? largestIlliNameForCurrentNumber =
                    TheLatinateIlliNameFor10ToPowerMultipleOf3(exponent.ToString());
                char currentGroupName_s1stLetter =
                    largestIlliNameForCurrentNumber[0];
                finalExpressionOfInitial1 = expressionOfInitial1 is "a" ?
                    // E.g. currentGroupName  is "octillion" or "undecilliard".
                    currentGroupName_s1stLetter is ('o' or 'u') ? "an" : "a"
                    :
                    "one";
            } // End of if (s_aRepresenting1IsSpecified is true)
/*         digitPointer initially points to the last digit of the final group 
            of 3 digits. It will conditionally be repeatedly decremented by 3,
            and will always point to the rightmost digit of a group of 3 digits.
            Since digitCount ≥ 5, initially digitPointer ≥ 4.  Thus for decimalNumeral = 13,256.
            digitPointer is initially 4; and for decimalNumeral = 134,256 digitPointer is initially 5.            */
            short? digitPointer = (short?)(digitCount - 1);
            // Group of 3 digits in decimalNumeral.  The groups start at the right end of the decimalNumeral.
            string?
            multiplierName,
            currentGroupOf1_2_Or3Digits;
            ushort? nameIndex;
            do
            {
/*            currentGroupOf1_2_Or3Digits is a group of 3 digits in the decimal numeral representation 
                of the integer.
                Groups of 1, 2, or 3 are processed starting from the rightmost and proceding leftward.
                digitPointer was initialized as digitCount - 1.                                                                                           */
                currentGroupOf1_2_Or3Digits = digitPointer >= 3 ?
/*                 Case 1. Not the leftmost group, and possibly the rightmost
                    digitPointer ≥ 3 implies that currentGroupOf1_2_Or3Digits is not the leftmost one,
                    and it is either between 2 commas, or to the right of the rightmost comma.
                    If digitPointer is digitCount -1, then this is the righmost group.                                                           */
                    decimalNumeral[(int)(digitPointer - 2)..(int)(digitPointer + 1)]
                    :
/*                 Case 2. Leftmost group
                    digitPointer ≤ 2 implies that currentGroupOf1_2_Or3Digits precedes the leftmost comma.
                    The while condition (see below) is digitPointer ≥ 0.                                                                        */
                    decimalNumeral[..(int)(digitPointer + 1)];
/*             On the 1st pass the rightmost group is computed. On subsequent passes the next group of 3 
                (or 1 or 2, if that is all that remain) digits to the left is selected.                                                       */
                #region Examples
                /*             For 85,906 on the 1st pass digitPointer is 4, get 
                                digits[(digitPointer - 2)..5], the 3 digits from index 2 
                                to 4 "906". On the 2nd pass digitPointer is 1, get 
                                decimalNumeral[..2], the 2 digits from index 0 to 1 "85". The
                                while condition below will then fail, and no more groups need
                                to be computed.

                                For 785,906 on the 1st pass digitPointer is 5, get
                                digits[3..6], the 3 digits from index 3 to 5 "906". On
                                the 2nd pass digitPointer is 2, get decimalNumeral[..2], the 2
                                digits from index 0 to 1 "785". The while condition will
                                then fail, and no more groups need to be computed.       

                                For 4,785,906 on the 1st pass digitPointer is 6, get
                                decimalNumeral[4..7], the 3 digits from index 4 to 6 "906". On
                                the 2nd pass digitPointer is 3, get decimalNumeral[1..4], the 3
                                decimalNumeral from index 1 to 3 "785". On the 3rd pass
                                digitPointer is 0, get decimalNumeral[..1], the digit at index
                                0 "4". The while condition will then fail, and no more
                                groups need to be computed.

                                For 34,785,906 on the 1st pass digitPointer is 7, get
                                decimalNumeral[5..8], the 3 digits from index 5 to 7 "906". On
                                the 2nd pass digitPointer is 4, get decimalNumeral[2..5], the 3
                                digits from index 2 to 4 "785". On the 3rd pass
                                digitPointer is 1, get decimalNumeral[..2], the 2 digits from
                                index 0 to 1 "34". The while condition will then fail,
                                and no more groups need to be computed.

                                For 34,000,906 on the 1st pass digitPointer is 7, get
                                decimalNumeral[5..8], the 3 digits from index 5 to 7 "906".  On
                                the 2nd pass digitPointer is 4, get decimalNumeral[2..5], the 3
                                digits from index 2 to 4 "000".  The condition
                                if (currentGroupOf1_2_Or3Digits is not "000") fails and englishCardinalNumeral
                                is not modified on this pass.  On the 3rd pass
                                digitPointer is 1, get decimalNumeral[..2], the 2 digits from
                                index 0 to 1 "34". The while condition will then fail,
                                and no more groups need to be computed.                     

                                For 834,785,906 on the 1st pass digitPointer is 8, get
                                decimalNumeral[6..9], the 3 digits from index 6 to 8 "906". On
                                the 2nd pass digitPointer is 5, get decimalNumeral[3..6], the 3
                                decimalNumeral from index 3 to 5 "785". On the 3rd pass
                                digitPointer is 2, get decimalNumeral[..3], the 3 digits from
                                index 0 to 2 "834".  The while condition will then fail, and no
                                more groups need to be computed.                                                                                     */
                #endregion
/*             If currentGroupOf1_2_Or3Digits is "000", this group will not be given a name;     
                "and" is inserted as appropriate.                                                                                                          */
                if (currentGroupOf1_2_Or3Digits is not "000")
                {
/*                 This works on the rightmost group of digits in decimalNumeral.  This is the first pass of "do".  
                    currentGroupOf1_2_Or3Digits contains 3 digits. If this group is between 001 and 099 
                    inclusive, "and" may precede it.                                                                                                        */
                    if (digitPointer == digitCount - 1)
                    {
                        if (currentGroupOf1_2_Or3Digits[0] is not '0')
                        {
                            if (currentGroupOf1_2_Or3Digits[^2..] is not "00")
                            {
                                englishCardinalNumeral =
                                    TheEnglishCardinalNumeralForThe3DigitInteger
                                        (currentGroupOf1_2_Or3Digits);
                            }
                            // currentGroupOf1_2_Or3Digits[^2..] is "00"
                            else
                            {
                                englishCardinalNumeral =
                                    TheEnglishCardinalNumeralForThe3DigitInteger
                                        (currentGroupOf1_2_Or3Digits);
                            }
                        } // End of currentGroupOf1_2_Or3Digits[0] is not '0'
                        // currentGroupOf1_2_Or3Digits[0] is '0'
                        else if (currentGroupOf1_2_Or3Digits is not "00")
                        // This (rightmost) group is between 001 and 099 inclusive.
                        {
                            conjunction = (bool)s_andInsertionIsSpecified ? "and" : string.Empty;
                            englishCardinalNumeral = (conjunction + Space).TrimStart() +
                               TheEnglishCardinalNumeralForThe3DigitInteger
                                    (currentGroupOf1_2_Or3Digits);
                        }
                        // currentGroupOf1_2_Or3Digits is "000"
                        //else englishCardinalNumeral will remain string.Empty
                    } // End of if (digitPointer == digitCount - 1) and of processing of the 1st (rightmost) group
/*                 This executes on the 2nd and subsequent passes of "do".
                    digitPointer is not digitCount - 1.
                    currentGroupOf1_2_Or3Digits is not the rightmost group in decimalNumeral.                        */
                    else
                    {
                        // E.g. three hundred and twenty-six                                                                                                      
                        multiplierName =
                            TheEnglishCardinalNumeralForThe3DigitInteger(currentGroupOf1_2_Or3Digits);
/*                     nameIndex + 2 is equivalent to a pass counter for  
                        "do" with the initial value of 2.  The counter value is 2
                        for the 2nd pass, the 1st pass being executed by the "if" group.
                        For the 2nd pass nameIndex is 0 (the index for "thousand").
                        For the 3rd pass nameIndex is 1 (the index for  "million"), etc.
                        Note that this block is not employed in the 1st pass, for no
                        multiplier or number group name is required there.                                       */
                        nameIndex = (ushort?)(((digitCount - digitPointer) / 3) - 1);
                        // E.g. billion                                                                                                                                             
                        illiName =
                            TheLatinateIlliNameFor10ToPowerMultipleOf3(nameIndex.ToString());
                        englishCardinalNumeral = TheConcatenationOf(multiplierName, Space,
                            // if englishCardinalNumeral is string.Empty, the space must be deleted.
                            illiName, TheConcatenationOf(Space, englishCardinalNumeral).TrimEnd());
                    } // End of else
                } // End of currentGroupOf1_2_Or3Digits is not "000"
/*             If currentGroupOf1_2_Or3Digits is "000", the current value of nameIndex
                will not be used to calculate a value for illiName,
                nor will a new value of englishCardinalNumeral be calculated.
                as an example, if decimalNumeral is 34,000,906, there will be no
                "thousand" term in the number name.                              
                For digit count = 5, digitPointer is 2. The decrement will set it to -1,
                and the do loop will exit.

                The decrement will make digitPointer point to the rightmost digit
                of the group of digits that precedes the current group.  If this is
                the initial group, it may contain 1, 2 or 3 digits.  In this case digitPointer
                will be set to 0, 1 or 2, resp.                                                                                                     */
                digitPointer -= 3;
                // End of do
            } while (digitPointer >= 0);
            if
                (
                    finalExpressionOfInitial1 != string.Empty
                    &&
                    // True if variable is "a" or "an".  If finalExpressionOfInitial1 is "one", the condition is false.
                    finalExpressionOfInitial1[..1] is "a"
                    &&
                    // "a hundred..."
                    englishCardinalNumeral[..3] is not "a h"
                )
            {
                englishCardinalNumeral = //    "a" or "an"                              
                    TheConcatenationOf(finalExpressionOfInitial1, Space,
                        // Delete initial "one ".  "one million" ⇒ "million" 
                        englishCardinalNumeral[4..]);
            }
/*         '!' is the null-forgiving, or null-suppression operator.
            Re: https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/null-forgiving     */
            return englishCardinalNumeral!;
        } // End of GetEnglishCardinalNumeralForInteger
        public static string TheEnglishCardinalNumeralForTheInteger(string decimalNumeral)
            => GetEnglishCardinalNumeralForInteger(decimalNumeral);
        // Re: https://en.wikipedia.org/wiki/Ordinal_numeral          
        // fourth, twenty-third, one hundred fifth
        public static string GetEnglishOrdinalNumeralAsWordGroup(string decimalNumeral)
        {
            string? englishCardinalNumeral =
                TheEnglishCardinalNumeralForTheInteger(decimalNumeral); 
            char[]? englishCardinalNumeralAsArray = englishCardinalNumeral.ToCharArray();
            short?
            positionOfFinalSpace =
                (short)LastIndexOf(englishCardinalNumeralAsArray, Space),
            positionOfFinalHyphen =
                (short)LastIndexOf(englishCardinalNumeralAsArray, Hyphen),
            positionOfFinalPunctuation =
                Max((short)positionOfFinalSpace, (short)positionOfFinalHyphen);
            bool? thereIsAFinalPunctuation = positionOfFinalPunctuation is not -1;
            string?
            finalWord = (bool)thereIsAFinalPunctuation ?
                englishCardinalNumeral[((int)positionOfFinalPunctuation + 1)..]
                :
                englishCardinalNumeral,
            englishOrdinalNumeral,
            baseGroup = (bool)thereIsAFinalPunctuation ?
                englishCardinalNumeral[..(int)positionOfFinalPunctuation] : string.Empty,
            punctuation = baseGroup != string.Empty ?
                // baseGroup: twenty, thirty, ...
                baseGroup[^1] is 'y' ? HyphenString : SpaceString
                :
                string.Empty;
            if (finalWord is "one")
                englishOrdinalNumeral = TheConcatenationOf(baseGroup, punctuation, "first");
            else if (finalWord is "two")
                englishOrdinalNumeral = TheConcatenationOf(baseGroup, punctuation, "second");
            else if (finalWord is "three")
                englishOrdinalNumeral = TheConcatenationOf(baseGroup, punctuation, "third");
            else if (finalWord is "five")
                englishOrdinalNumeral = TheConcatenationOf(baseGroup, punctuation, "fifth");
            else if (finalWord is "eight")
                englishOrdinalNumeral = TheConcatenationOf(baseGroup, punctuation, "eigth");
            else if (finalWord is "nine")
                englishOrdinalNumeral = TheConcatenationOf(baseGroup, punctuation, "ninth");
            else if (finalWord is "twelve")
                englishOrdinalNumeral = TheConcatenationOf(baseGroup, punctuation, "twelfth");
            // finalWord: twenty, thirty, ...
            else if (finalWord[^1] is 'y')
            {
                // forty ⇒ fort
                finalWord = finalWord[..^1];
                englishOrdinalNumeral =
                    TheConcatenationOf(baseGroup, punctuation, finalWord, "ieth");
            }
            else
            {
                // four ⇒ fourth
                englishOrdinalNumeral =
                    TheConcatenationOf(baseGroup, punctuation, finalWord, "th");
            }
            return englishOrdinalNumeral;
        } // End of GetEnglishOrdinalNumeralAsWordGroup
        public static string TheEnglishOrdinalNumeralAsWordGroupFor(string decimalNumeral)
            => GetEnglishOrdinalNumeralAsWordGroup(decimalNumeral);
        // 1st, 2nd, 5th, ...
        public static string GetEnglishOrdinalNumeralAsDecimalNumeral(string decimalNumeral)
        {
            ushort? lengthOfDecimalNumeral = (ushort?)decimalNumeral.Length;
            string? decimalNumeralAndCommas = decimalNumeral;
            // Insert commas at intervals of three digits, starting from the right.
            for (var i = 1; i <= (lengthOfDecimalNumeral - 1) / 3; i++)
            {
                decimalNumeralAndCommas = decimalNumeralAndCommas.
                    Insert((int)(lengthOfDecimalNumeral - 3 * i), CommaString);
            }
            char? input_sLastDigit = decimalNumeral[^1];
            return input_sLastDigit switch
            {
                '1' => decimalNumeralAndCommas + "st",
                '2' => decimalNumeralAndCommas + "nd",
                '3' => decimalNumeralAndCommas + "rd",
                _  => decimalNumeralAndCommas + "th",
            };
        }
        public static string TheEnglishOrdinalNumeralAsDecimalNumeralFor(string decimalNumeral)
            => GetEnglishOrdinalNumeralAsDecimalNumeral(decimalNumeral);
        public static string ExpressSequenceOfDigitsAsWords(string digits)
        {
            if (digits == string.Empty)
                throw new Exception();
            var sequenceExpressionAsSB = new StringBuilder();
            foreach (char ch in digits)
            {
                sequenceExpressionAsSB.Append
                    (TheEnglishCardinalNumeralForThe1DigitInteger(ch.ToString()))
                        .Append(Space);
            }
            // Delete the last element, which is a trailing space.
            sequenceExpressionAsSB.Length--;
            return sequenceExpressionAsSB.ToString();
        }
        public static string TheExpressionwithSignificandAsWordsOfTheDigitalSequence(string digits)
            => ExpressSequenceOfDigitsAsWords(digits);
 /*    For terminology of decimal numbers see:
                https://en.wikipedia.org/wiki/Decimal#Decimal_notation                                  */
        public static string ExpressDecimalFraction
            (string negationPrefix, string integerPart, string fractionalPart)
        {
            string ?
            // These variables are never string.Empty.
            fractionalPartName = TheExpressionwithSignificandAsWordsOfTheDigitalSequence(fractionalPart),
            integerPartName =
                TheEnglishCardinalNumeralForTheInteger(integerPart);
            //                                         May be string.Empty
            return TheConcatenationOf((negationPrefix + Space).TrimStart(), integerPartName,
                Space, "point", Space, fractionalPartName);
        } // End of ExpressDecimalFraction 
        public static string TheExpressionOfTheDecimalFraction
            (string negationPrefix, string integerPart, string fractionalPart)
                => ExpressDecimalFraction(negationPrefix, integerPart, fractionalPart);
        // Deletes commas and other extraneous characters.   
        public static string ExtractUsableCharacters(string chars)
        {
            string? usableChars = chars.WithOnly(Digits + Period + MinusSign);
            return !IsNullOrEmpty(usableChars) ? usableChars : string.Empty;
        }
        public static string TheUsableCharactersOf(string chars)
            => ExtractUsableCharacters(chars);
        public static bool ThisContainsNoDigits(string chars)
        {
            foreach (char ch in chars)
            {
                if (Digits.Contains(ch))
                    return false;
            }
            return true;
        } // End of ThisContainsNoDigits
        public static bool CheckForMultiplePeriods(string chars)
        {
            byte? periodCount =
                (byte)(from ch in chars where ch is Period select ch).Count();
            bool? thereAreMultiplePeriods = false;
            if (periodCount > 1)
            {
                string?
                periodCountAsString = periodCount.ToString(),
                periodCountInWords = IsNullOrEmpty(periodCountAsString) ?
                    string.Empty
                    :
                    TheEnglishCardinalNumeralForTheInteger(periodCountAsString);
                BackgroundColor = White;
                ForegroundColor = DarkRed;
                WriteLine($"The input contained {periodCountInWords} periods.  " +
                    $"Only one period is allowed.\nPlease enter another number.");
                ResetColor();
                thereAreMultiplePeriods = true;
            }
            return (bool)thereAreMultiplePeriods;
        } // End of CheckForMultiplePeriods
        public static bool ThisContainsMultiplePeriods(string chars)
            => CheckForMultiplePeriods(chars);
        public static bool ThisContainsErrors(string chars)
        {
            return // Affix ';' to final error listed.
                ThisContainsMultiplePeriods(chars);
            //  ||
            //  Other error; 
        }
/*     Inputs containing no nonzero digits may be integers, such as "0" or "00"; or decimal fractions,
        such as 0.00.  In any of these cases the inclusion of a minus sign will be ignored in the 
        computation.  This is justified since, by convention -0 is not expressed with a minus sign, and
        since -0 = 0.

        For decimal fractions, if the integer part consists of one or more 0's, exactly 
        one zero should remain.                                                                                                     */
        public static bool ThisContainsOnly0s(string chars)
            => chars.TrimStart('0') == string.Empty;

/*     chars                      28.35   .9    .90  0.9  00.76   2   23    2.   23.   0.0  0.  0034  089.3  .    ""
        index of period        2         0      0    1        2     -1   -1     1     2       1   1     -1       3      -*   -*
        rawIntegerPart        28       ""     ""   0       00     2   23     2    23     0   0   0034   089    -*   -*
        integerPart              28       0       0    0        0      2   23     2    23     0   0     34      89     0    0
        This works in cases where chars contains at most one period and no other non-digit characters.
            *- Index of period and rawIntegerPart have no value in the table, as they are not computed.    
        string.Empty is never returned.
        // Re: https://en.wikipedia.org/wiki/Decimal                                                                                        */
        public static string GetIntegerPart(string chars)
        {
            chars = chars.TrimStart('0');
            string? integerPart;
            // Interpret some unconventional inputs.
            if ((chars == string.Empty) || (chars == PeriodString))
                integerPart = "0";
            else
            {
                string? rawIntegerPart = chars.Contains(Period) ?
/*                 The 1st value is selected only if chars contains a period, so no negative index
                    ever occurs within the square brackets.                                                                         */
                    chars[..chars.IndexOf(Period)] : chars;
                if (rawIntegerPart == string.Empty)
                    integerPart = chars.Contains(Period) ? "0" : chars;
                else if (ThisContainsOnly0s(rawIntegerPart))
                    integerPart = "0";
                else
                    integerPart = rawIntegerPart.TrimStart('0');
            } 
            return integerPart;
        } // End of GetIntegerPart
        public static string TheIntegerPartOf(string chars)
            => GetIntegerPart(chars);
        // Re: https://en.wikipedia.org/wiki/Decimal
        // decimalNumeral contains at most one period.
        public static string GetFractionalPart(string decimalNumeral)
        {
            string? fractionalPart;
            if (decimalNumeral.Contains(Period) is false)
                fractionalPart = string.Empty;
            // A final period causes the user input to be treated as an integer.
            else if (decimalNumeral[^1] == Period)
                fractionalPart = string.Empty;
            // decimalNumeral contains a period, and its position is not final.
            else
            {
                short? positionOfPeriod =
                    (short?)decimalNumeral.IndexOf(Period);
                fractionalPart = decimalNumeral[(int)(positionOfPeriod + 1)..];
            }
            return fractionalPart;
        } // End of GetFractionalPart
        // decimalNumeral contains at most one period.
        public static string TheFractionalPartOf(string decimalNumeral)
            => GetFractionalPart(decimalNumeral);
        // This will precede each user input.
        public static void GiveInstructions()
        {
            BackgroundColor = DarkMagenta;
            ForegroundColor = White;
            WriteLine("Please enter a number in digital form, either a whole number (integer)\n" +
                "or a decimal to be expressed in English");
            // Thread.Sleep(5500);
            WriteLine();
            WriteLine("A whole number or the integer part\n" +
                    "of a decimal number may contain up to 3,604 digits.");
            // Thread.Sleep(4500);
            WriteLine();
            WriteLine("Commas may be included for readability when inputting numbers.");
            // Thread.Sleep(4000);
            WriteLine();
            WriteLine("You may also enter 'x' to exit the program.");
            // Thread.Sleep(3000);
            WriteLine();
            ResetColor();
        }
        public static void SignOff()
        {
            BackgroundColor = Magenta;
            ForegroundColor = DarkMagenta;
            WriteLine("Thank you for using \"Expressing Numbers With Words\"");
            Thread.Sleep(3500);
            // Re: https://learn.microsoft.com/en-us/dotnet/api/system.environment.exit
            Exit(0);
        }
        // This will compute and print a set of heading and expresing derived from a given input.
        public static void GetHeadingsAndExpressions()
        {
            string? negativePrefix = string.Empty;
/*         Key to codes  
            null  no options selected
            e  s_andInsertionIsSpecified
            f  s_substituting100For1000IsSpecified
            g  s_aRepresenting1IsSpecified                                                                                                       */
            ResetColor();
            WriteLine("");
            if (s_numberIsDecimalFraction is false)
            { 
                if (
                        // The values of these fields are determined by the input.
                        s_scaleSpecificationIsRequired is false
                        &&
                        s_numberIsNegative is false
                    )
                {
                    // null
                    WriteLine("Nonnegative Integer");
                    WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                    WriteLine("");
                    if (s_andInsertionIsApplicable)
                    {
                        // e
                        WriteLine("Nonnegative Integer with \"and\"");
                        s_andInsertionIsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        WriteLine("");
                    }
                    if (s_substituting100For1000IsApplicable)
                    { // f
                        WriteLine("Nonnegative Integer with 100 Substituted for 1000");
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_substituting100For1000IsApplicable))
                    {
                        // ef
                        WriteLine("Nonnegative Integer " +
                            "with \"and\" and 100 Substituted for 1000");
                        s_andInsertionIsSpecified = true;
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                    }
                    if (s_aRepresenting1IsApplicable)
                    {
                        // g
                        WriteLine("Nonnegative Integer with \"a\" Representing 1");
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                    {
                        // eg
                        WriteLine("Nonnegative Integer with \"and\" and \"a\" Representing 1");
                        s_andInsertionIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                } /* End of if (
                                            s_scaleSpecificationIsRequired is false
                                            &&
                                            s_numberIsDecimalFraction is false
                                            &&
                                            s_numberIsNegative is false
                                        )                                                                                                                         */
                if
                    (
                        s_scaleSpecificationIsRequired is false
                        &&
                        s_numberIsDecimalFraction is false
                        &&
                        s_numberIsNegative
                    )
                {
                    // null
                    WriteLine("Negative Integer with Prefix \"minus\"");
                    WriteLine(TheConcatenationOf("minus", Space,
                        TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                    WriteLine("");
                    if (s_andInsertionIsApplicable)
                    {
                        // e
                        s_andInsertionIsSpecified = true;
                        WriteLine("Negative Integer with Prefix \"minus\" and \"and\"");
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_substituting100For1000IsApplicable))
                    {
                        // ef
                        WriteLine("Negative Integer " +
                            "with Prefix \"minus\", \"and\", and 100 Substituted for 1000");
                        s_andInsertionIsSpecified = true;
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                    {
                        // eg
                        WriteLine("Negative Integer " +
                            "with Prefix \"minus\", \"and\", and \"a\" Representing 1");
                        s_andInsertionIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                    if (s_substituting100For1000IsApplicable)
                    {
                        // f
                        WriteLine("Negative Integer " +
                            "with Prefix \"minus\" and 100 Substituted for 1000");
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                    }
                    if (s_aRepresenting1IsApplicable)
                    {
                        // g
                        WriteLine("Negative Integer " +
                            "with Prefix \"minus\" and \"a\" Representing 1");
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                    // End of prefix is "minus"
                    // null
                    WriteLine("Negative Integer with Prefix \"negative\"");
                    WriteLine(TheConcatenationOf("negative", Space,
                        TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                    WriteLine("");
                    if (s_andInsertionIsApplicable)
                    {
                        // e
                        WriteLine("Negative Integer with Prefix \"negative\" and \"and\"");
                        s_andInsertionIsSpecified = true;
                        WriteLine(TheConcatenationOf("negative", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_substituting100For1000IsApplicable))
                    {
                        // ef
                        WriteLine("Negative Integer with Prefix \"negative\", \"and\", " +
                            "and 100 Substituted for 1000");
                        s_andInsertionIsSpecified = true;
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheConcatenationOf("negative", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                    {
                        // eg
                        WriteLine("Negative Integer " +
                            "with Prefix \"negative\", \"and\", and \"a\" Representing 1");
                        s_andInsertionIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheConcatenationOf("negative", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                    if (s_substituting100For1000IsApplicable)
                    {
                        // f
                        WriteLine("Negative Integer " +
                            "with Prefix \"negative\" and 100 Substituted for 1000");
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheConcatenationOf("negative", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                    }
                    if (s_aRepresenting1IsApplicable)
                    {
                        // g
                        WriteLine("Negative Integer " +
                            "with Prefix \"negative\" and \"a\" Representing 1");
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheConcatenationOf("negative", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                } /* End of if (
                                            s_scaleSpecificationIsRequired is false
                                            &&
                                            s_numberIsDecimalFraction is false
                                            &&
                                            s_numberIsNegative 
                                      )                                                                                                    */
                if
                (
                    s_scaleSpecificationIsRequired 
                    &&
                    s_numberIsDecimalFraction is false
                    &&
                    s_numberIsNegative is false
                )
                {
                    // null
                    WriteLine("Long Scale Expression of Nonnegative Integer");
                    s_longScaleIsSpecified = true;
                    WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                    WriteLine("");
                    WriteLine("Short Scale Expression of Nonnegative Integer");
                    s_longScaleIsSpecified = false;
                    WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                    WriteLine("");
                    if (s_andInsertionIsApplicable)
                    {
                        // e
                        WriteLine("Long Scale Expression of Nonnegative Integer " +
                            "with \"and\"");
                        s_longScaleIsSpecified = true;
                        s_andInsertionIsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        WriteLine("");
                        WriteLine("Short Scale Expression of Nonnegative Integer " +
                            "with \"and\"");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        WriteLine("");
                    }
                    if (s_aRepresenting1IsApplicable)
                    {
                        // g 
                        WriteLine("Long Scale Expression of Nonnegative Integer " +
                            "with \"a\" Representing 1");
                        s_longScaleIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        WriteLine("");
                        WriteLine("Short Scale Expression of Nonnegative Integer " +
                            "with \"a\" Representing 1");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        WriteLine("");
                        s_aRepresenting1IsSpecified = false;
                    }
                    if ((s_aRepresenting1IsApplicable) && (s_andInsertionIsApplicable))
                    {
                        // eg
                        WriteLine("Long Scale Expression of Nonnegative Integer " +
                            "with \"and\" and \"a\" Representing 1");
                        s_longScaleIsSpecified = true;
                        s_andInsertionIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        WriteLine("");
                        WriteLine("Short Scale Expression of Nonnegative Integer " +
                            "with \"and\" and \"a\" Representing 1");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheEnglishCardinalNumeralForTheInteger(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                } /* End of if
                            (
                                s_scaleSpecificationIsRequired 
                                &&
                                s_numberIsDecimalFraction is false
                                &&
                                s_numberIsNegative is false
                            )                                                                                                */
                if
                    (
                        s_scaleSpecificationIsRequired is false
                        &&
                        s_numberIsDecimalFraction is false
                        &&
                        s_numberIsNegative
                    )
                {
                    // null
                    WriteLine("Negative Integer with Prefix \"minus\"");
                    WriteLine(TheConcatenationOf("minus", Space,
                        TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                    WriteLine("");
                    if (s_andInsertionIsApplicable)
                    {
                        // e
                        WriteLine("Negative Integer with Prefix \"minus\" and \"and\"");
                        s_andInsertionIsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_substituting100For1000IsApplicable))
                    {
                        // ef
                        WriteLine("Negative Integer " +
                            "with Prefix \"minus\", \"and\", and 100 Substituted for 1000");
                        s_andInsertionIsSpecified = true;
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                    {
                        // eg
                        WriteLine("Negative Integer with Prefix \"minus\", \"and\", and \"a\" Representing 1");
                        s_andInsertionIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_andInsertionIsSpecified = false;
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                    if (s_substituting100For1000IsApplicable)
                    {
                        // f
                        WriteLine("Negative Integer " +
                            "with Prefix \"minus\" and 100 Substituted for 1000");
                        s_substituting100For1000IsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        s_substituting100For1000IsSpecified = false;
                        WriteLine("");
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Negative Integer " +
                                "with Prefix \"minus\" and 100 Substituted for 1000");
                            s_aRepresenting1IsSpecified = true;
                            WriteLine(TheConcatenationOf("minus", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_aRepresenting1IsSpecified = false;
                            WriteLine("");
                        }
                        // null
                        WriteLine("Negative Integer with Prefix \"negative\"");
                        WriteLine(TheConcatenationOf("negative", Space,
                            TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Negative Integer with Prefix \"negative\" and \"and\"");
                            s_andInsertionIsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_andInsertionIsSpecified = false;
                            WriteLine("");
                        }
                        if ((s_andInsertionIsApplicable) && (s_substituting100For1000IsApplicable))
                        {
                            // ef
                            WriteLine("Negative Integer " +
                                "with Prefix \"negative\", \"and\", and 100 Substituted for 1000");
                            s_andInsertionIsSpecified = true;
                            s_substituting100For1000IsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_andInsertionIsSpecified = false;
                            s_substituting100For1000IsSpecified = false;
                            WriteLine("");
                        }
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Negative Integer " +
                                "with Prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            WriteLine("");
                        }
                        if (s_substituting100For1000IsApplicable)
                        {
                            // f
                            WriteLine("Negative Integer " +
                                "with Prefix \"negative\" and 100 Substituted for 1000");
                            s_substituting100For1000IsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_substituting100For1000IsSpecified = false;
                            WriteLine("");
                        }
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Negative Integer " +
                                "with Prefix \"negative\" and \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_aRepresenting1IsSpecified = false;
                            WriteLine("");
                        }
                    } /* End of if
                               (
                                   s_scaleSpecificationIsRequired is false
                                   &&
                                   s_numberIsDecimalFraction is false
                                   &&
                                   s_numberIsNegative 
                               )                                                                                                                         */
                    if
                        (
                            s_scaleSpecificationIsRequired
                            &&
                            s_numberIsDecimalFraction is false
                            &&
                            s_numberIsNegative
                        )
                    {
                        ResetColor();
                        // null
                        WriteLine("Long Scale Expression of Negative Integer " +
                            "with Prefix \"minus\"");
                        s_longScaleIsSpecified = true;
                        WriteLine(TheConcatenationOf("minus", Space,
                                   TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        WriteLine("");
                        WriteLine("Short Scale Expression of Negative Integer " +
                            "with Prefix \"minus\"");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheConcatenationOf("minus", Space,
                                       TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Long Scale Expression of Negative Integer " +
                                "with Prefix \"minus\" and \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            WriteLine(TheConcatenationOf("minus", Space,
                                   TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            WriteLine("");
                            WriteLine("Short Scale Expression of Negative Integer " +
                                "with Prefix \"minus\" and \"and\"");
                            s_longScaleIsSpecified = false;
                            WriteLine(TheConcatenationOf("minus", Space,
                                   TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_andInsertionIsSpecified = false;
                            WriteLine("");
                        }
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Long Scale Expression of Negative Integer " +
                                "with Prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            WriteLine(TheConcatenationOf("minus", Space,
                                   TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            WriteLine("");
                            WriteLine("Short Scale Expression of Negative Integer " +
                                "with Prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            WriteLine(TheConcatenationOf("minus", Space,
                                   TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            WriteLine("");
                        }  
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Long Scale Expression of Negative Integer " +
                                "with Prefix \"minus\" with \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            WriteLine(TheConcatenationOf("minus", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            WriteLine("");
                            WriteLine("Short Scale Expression of Negative Integer " +
                                "with Prefix \"minus\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            WriteLine(TheConcatenationOf("minus", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_aRepresenting1IsSpecified = false;
                            WriteLine("");
                        }
                        // null
                        WriteLine("Long Scale Expression of Negative Integer " +
                            "with Prefix \"negative\"");
                        s_longScaleIsSpecified = true;
                        WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        WriteLine("");
                        WriteLine("Short Scale Expression of Negative Integer " +
                            "with Prefix \"negative\"");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Long Scale Expression of Negative Integer " +
                                "with Prefix \"negative\" and \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            WriteLine("");
                            // e
                            WriteLine("Short Scale Expression of Negative Integer " +
                                "with Prefix \"negative\" and \"and\"");
                            s_longScaleIsSpecified = false;
                            WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_andInsertionIsSpecified = false;
                            WriteLine("");
                        }
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Long Scale Expression of Negative Integer " +
                                "with Prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            WriteLine("");
                            WriteLine("Short Scale Expression of Negative Integer " +
                                "with Prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            WriteLine("");
                        }
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Long Scale Expression of Negative Integer " +
                                "with Prefix \"negative\" with \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            WriteLine("");
                            s_longScaleIsSpecified = false;
                            WriteLine("Short Scale Expression of Negative Integer " +
                                "with Prefix \"negative\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            WriteLine(TheConcatenationOf("negative", Space,
                                    TheEnglishCardinalNumeralForTheInteger(s_integerPart)));
                            s_aRepresenting1IsSpecified = false;
                            WriteLine("");
                        }
                    } // End of if 
                }/* End of if  
                                        (
                                            s_scaleSpecificationIsRequired
                                            &&
                                            s_numberIsDecimalFraction is false
                                            &&
                                            s_numberIsNegative
                                        )	                                                                                                     */
            } // End of if (s_numberIsDecimalFraction is false)
            WriteLine("");
            // End of integers

            // Decimal Fractions
/*         A decimal fraction will always include a fractional part that is not string.Empty,
            so indexOfPoint1 will never be negative.
            See:
            if (s_fractionalPart != string.Empty)
                s_numberIsDecimalFraction = true;
            else
                s_numberIsDecimalFraction = false;                                                                             */
            if (s_numberIsDecimalFraction)
            {
                ushort? indexOfPoint1;
                string?
                decimalFraction,
                integerPart1,
                fractionalPart1;
                if (s_numberIsNegative is false)
                {
                    if (s_scaleSpecificationIsRequired is false)
                    {
                        // null
                        ResetColor();
                        WriteLine("Nonnegative Decimal Fraction");
                        decimalFraction = // string.Empty stands in the place for the negative prefix if number were negative.
                            TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                        // To find "point" must search for "po" in order to bypass "pt" in "sept" (Latin for 7), as in "septillion".
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Nonnegative Decimal Fraction with \"and\"");
                            s_andInsertionIsSpecified = true;
                            decimalFraction = //  string.Empty stands in the place for the negative prefix if number were negative.
                                TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g
                            WriteLine("Nonnegative Decimal Fraction with \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction = //  string.Empty stands in the place for the negative prefix if number were negative.
                                TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg
                            ResetColor();
                            WriteLine("Nonnegative Decimal Fraction with \"and\" and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction = // string.Empty stands in the place for the negative prefix if number were negative.
                                TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                    } // End of if (s_scaleSpecificationIsRequired is false) 
                     // s_scaleSpecificationIsRequired 
                    else
                    {
                        // null
                        WriteLine("Long Scale Expression of Nonnegative Decimal Fraction");
                        s_longScaleIsSpecified = true;
                        decimalFraction = // string.Empty stands in the place for the negative prefix if number were negative.
                            TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        // null
                        WriteLine("Short Scale Expression of Nonnegative Decimal Fraction");
                        s_longScaleIsSpecified = false;
                        decimalFraction = // string.Empty stands in the place for the negative prefix if number were negative.
                            TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Long Scale Expression of Nonnegative Decimal Fraction " +
                                "with \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            decimalFraction = //  string.Empty stands in the place for the negative prefix if number were negative.
                                TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // e
                            WriteLine("Short Scale Expression of Nonnegative Decimal Fraction " +
                                "with \"and\"");
                            s_longScaleIsSpecified = false;
                            decimalFraction = //  string.Empty stands in the place for the negative prefix if number were negative.
                                TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        } // End of if (s_andInsertionIsApplicable)
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Long Scale Expression of Nonnegative Decimal Fraction " +
                                "with \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction = //      string.Empty stands in the place for the negative prefix if number were negative.
                            TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // g
                            WriteLine("Short Scale Expression of Nonnegative Decimal Fraction " +
                                "with \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            decimalFraction = //  string.Empty stands in the place for the negative prefix if number were negative.
                                TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        } // End of if (s_aRepresenting1IsApplicable)
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Long Scale Expression of Nonnegative Decimal Fraction " +
                                "with \"and\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction = //      string.Empty stands in the place for the negative prefix if number were negative.
                            TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // eg
                            WriteLine("Short Scale Expression of Nonnegative Decimal Fraction " +
                                "with \"and\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            decimalFraction = //  string.Empty stands in the place for the negative prefix if number were negative.
                                TheExpressionOfTheDecimalFraction(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        } // End of if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                    } // End of else (s_scaleSpecificationIsRequired)
                } // End of if (s_numberIsNegative is false))
                // s_numberIsNegative
                else
                {
                    if (s_scaleSpecificationIsRequired is false)
                    {
                        // null
                        WriteLine("Negative Decimal Fraction with prefix \"minus\"");
                        decimalFraction =
                            TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Negative Decimal Fraction " +
                                "with prefix \"minus\" and \"and\"");
                            s_andInsertionIsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        if(s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Negative Decimal Fraction with prefix \"minus\" and \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction =  
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Negative Decimal Fraction with prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction = 
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        // Prefix "negative"
                        // null
                        WriteLine("Negative Decimal Fraction with prefix \"negative\"");
                        decimalFraction =
                            TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e 
                            WriteLine("Negative Decimal Fraction with prefix \"negative\" and \"and\"");
                            s_andInsertionIsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Negative Decimal Fraction with prefix \"negative\" and \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction =  
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        WriteLine("");
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Negative Decimal Fraction with prefix \"negative\", \"and\" " +
                                "and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction =  
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                    } // End of if (s_scaleSpecificationIsRequired is false) 
                    // s_scaleSpecificationIsRequired
                    else
                    {
                        // null
                        WriteLine("Long Scale Expression of Negative Decimal Fraction with prefix \"minus\"");
                        s_longScaleIsSpecified = true;
                        decimalFraction =
                            TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1= decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        // null
                        WriteLine("Short Scale Expression of Negative Decimal Fraction with prefix \"minus\"");
                        s_longScaleIsSpecified = false;
                        decimalFraction =
                            TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Long Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"minus\" and \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // e
                            WriteLine("Short Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"minus\" and \"and\"");
                            s_longScaleIsSpecified = false;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Long Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"minus\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // g
                            WriteLine("Short Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"minus\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Long Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // eg
                            WriteLine("Short Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        }
                        // null
                        WriteLine("Long Scale Expression of Negative Decimal Fraction " +
                            "with prefix \"negative\"");
                        s_longScaleIsSpecified = true;
                        decimalFraction =
                            TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        // null
                        WriteLine("Short Scale Expression of Negative Decimal Fraction " +
                            "with prefix \"negative\"");
                        s_longScaleIsSpecified = false;
                        decimalFraction =
                            TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                        indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                        integerPart1 = decimalFraction[..(int)indexOfPoint1];
                        fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart1);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart1);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionIsApplicable)
                        {
                            // e
                            WriteLine("Long Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"negative\" and \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            ForegroundColor = DarkBlue;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // e
                            WriteLine("Short Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"negative\" and \"and\"");
                            s_longScaleIsSpecified = false;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        } // End of if (s_andInsertionIsApplicable)
                        if (s_aRepresenting1IsApplicable)
                        {
                            // g
                            WriteLine("Long Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"negative\" and\"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // g
                            WriteLine("Short Scale Expression of Negative Decimal Fraction " +
                                "with prefix \"negative\" and\"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        } // End of if (s_aRepresenting1IsApplicable)
                        if ((s_aRepresenting1IsApplicable) && (s_aRepresenting1IsApplicable))
                        {
                            // eg
                            WriteLine("Long Scale Expression of Negative Decimal Fraction " +
                                "with  prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                            // eg
                            WriteLine("Short Scale Expression of Negative Decimal Fraction " +
                                "with  prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            decimalFraction =
                                TheExpressionOfTheDecimalFraction("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint1 = (ushort?)decimalFraction.IndexOf("po");
                            integerPart1 = decimalFraction[..(int)indexOfPoint1];
                            fractionalPart1 = decimalFraction[(int)(indexOfPoint1 + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart1);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart1);
                            ResetColor();
                            WriteLine("");
                        } // End of if (s_aRepresenting1IsApplicable)
                    } // End of if (s_scaleSpecificationIsRequired)
                } // End of else (s_numberIsNegative)
            } // End of else (s_numberIsDecimalFraction)
            // End of Decimal Fractions
            WriteLine("");

            // Pseudo_scientific Expression with Significand as Wordss
    /*     E.g. 3,050 ⇒ three point zero five thousand  2500.1 ⇒ two point five zero zero one thousand
            Negative numbers may be expressed in this form.
            These expressions may include "and".                                                                                          */
            ushort? indexOfPoint;
            string?
            pseudo_scientificExpression,
            integerPart,
            fractionalPart;
            if (s_pseudo_scientificFormIsApplicable)
            { 
                if (s_scaleSpecificationIsRequired is false)
                { 
                    if (s_numberIsNegative is false)
                    {
                        // null
                        WriteLine("Nonnegative Pseudo_scientific Expression with Significand as Words");
                        pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable)
                        {
                            // e
                            WriteLine("Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"and\"");
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g 
                            WriteLine("Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionForPseudo_scientificIsApplicable) &&
                            (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg
                            WriteLine("Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"and\" and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                    } // End of if (s_numberIsNegative is false)
                    // s_numberIsNegative
                    else
                    {
                        // null
                        WriteLine("Negative Pseudo_scientific Expression with Significand as Words" +
                            "with Prefix \"minus\"");
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable)
                        {
                            // e 
                            ResetColor();
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\" and \"and\"");
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g 
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\" and \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionForPseudo_scientificIsApplicable) &&
                            (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg 
                            WriteLine("Negative Pseudo-scientific Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        // null
                        WriteLine("Negative Pseudo_scientific Expression with Significand as Words" +
                            "with Prefix \"negative\"");
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable) 
                        {
                            // e 
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"negative\" and \"and\"");
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g 
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"negative\" and \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionForPseudo_scientificIsApplicable) && (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg 
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                    } // End of else (s_numberIsNegative)                            
                } // End of if (s_scaleSpecificationIsRequired is false)            
                // s_scaleSpecificationIsRequired
                else
                {
                    if ((s_numberIsNegative is false) && (s_scaleSpecificationIsRequired))
                    {
                        // null
                        WriteLine("Long Scale Nonnegative Pseudo_scientific Expression with Significand as Words");
                        s_longScaleIsSpecified = true;
                        pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        // null
                        ResetColor();
                        WriteLine("Short Scale Nonnegative Pseudo_scientific Expression with Significand as Words");
                        s_longScaleIsSpecified = false;
                        pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable)
                        {
                            // e 
                            WriteLine("Long Scale Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // e
                            ResetColor();
                            WriteLine("Short Scale of Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"and\"");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g 
                            WriteLine("Long Scale Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // g
                            WriteLine("Short Scale Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionForPseudo_scientificIsApplicable) && (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg 
                            WriteLine("Long Scale Nonnegative Pseudo_scientific Expression with Significand as Words" +
                                "with \"and\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // eg
                            WriteLine("Short Scale Nonnegative Pseudo_scientific Expression with Significand as Words with \"and\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression = // string.Empty stands in the place of the negative prefix if the number were negative.
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf(string.Empty, s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                    } // End of if ((s_numberIsNegative is false) && (s_scaleSpecificationIsRequired))
                    if ((s_numberIsNegative) && (s_scaleSpecificationIsRequired is false))
                    {
                        // null
                        WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"minus\"");
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable)
                        {
                            // e
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"minus\" and \"and\"");
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            ResetColor();
                            WriteLine(fractionalPart);
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"minus\" and \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            ResetColor();
                            WriteLine(fractionalPart);
                        }
                        WriteLine("");
                        if ((s_andInsertionForPseudo_scientificIsApplicable) &&
                            (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"minus\", " +
                                "\"and\", and \"a\" Representing 1");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        // null
                        WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"negative\"");
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable)
                        {
                            // e
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"negative\" and \"and\"");
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"negative\", " +
                                "and \"a\" Representing 1");
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionForPseudo_scientificIsApplicable) &&
                            (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg
                            WriteLine("Negative Pseudo_scientific Expression with Significand as Words with Prefix \"negative\", " +
                                "\"and\", and \"a\" Representing 1 ");
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                    }
                    if ((s_numberIsNegative) && (s_scaleSpecificationIsRequired))
                    {
                        // null
                        WriteLine("Long Scale Negative Pseudo_scientific Expression with Significand as Words with Prefix \"minus\"");
                        s_longScaleIsSpecified = true;
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        // null
                        WriteLine("Short Scale Negative Pseudo_scientific Expression with Significand as Words with Prefix \"minus\"");
                        s_longScaleIsSpecified = false;
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable)
                        {
                            // e
                            WriteLine("Long Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\" and \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // e
                            WriteLine("Short Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\" and \"and\"");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart); ;
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if (s_aRepresenting1ForPseudo_scientificIsApplicable)
                        {
                            // g 
                            WriteLine("Long Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // g
                            WriteLine("Short Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\" and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionForPseudo_scientificIsApplicable) &&
                            (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg 
                            WriteLine("Long Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // eg 
                            WriteLine("Short Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"minus\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("minus", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        // null
                        WriteLine("Long Scale Negative Pseudo_scientific Expression with Significand as Words" +
                            "with Prefix \"negative\"");
                        s_longScaleIsSpecified = true;
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        // null
                        WriteLine("Short Scale Negative Pseudo_scientific Expression with Significand as Words" +
                            "with Prefix \"negative\"");
                        s_longScaleIsSpecified = false;
                        pseudo_scientificExpression =
                            ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                        indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                        integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                        fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                        ForegroundColor = DarkBlue;
                        Write(integerPart);
                        ForegroundColor = Red;
                        Write("point");
                        ForegroundColor = DarkBlue;
                        WriteLine(fractionalPart);
                        ResetColor();
                        WriteLine("");
                        if (s_andInsertionForPseudo_scientificIsApplicable)
                        {
                            // e 
                            WriteLine("Long Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"negative\" and \"and\"");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // e 
                            WriteLine("Short Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"negative\" and \"and\"");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        }
                        if ((s_andInsertionForPseudo_scientificIsApplicable) &&
                            (s_aRepresenting1ForPseudo_scientificIsApplicable))
                        {
                            // eg 
                            WriteLine("Long Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = true;
                            s_andInsertionIsSpecified = true;
                            s_aRepresenting1IsSpecified = true;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                            // eg 
                            WriteLine("Short Scale Negative Pseudo_scientific Expression with Significand as Words" +
                                "with Prefix \"negative\", \"and\", and \"a\" Representing 1");
                            s_longScaleIsSpecified = false;
                            pseudo_scientificExpression =
                                ThePseudo_scientificExpressionWithSignificandAsWordsOf("negative", s_integerPart, s_fractionalPart);
                            s_andInsertionIsSpecified = false;
                            s_aRepresenting1IsSpecified = false;
                            indexOfPoint = (ushort?)pseudo_scientificExpression.IndexOf("po");
                            integerPart = pseudo_scientificExpression[..(int)indexOfPoint];
                            fractionalPart = pseudo_scientificExpression[(int)(indexOfPoint + 5)..];
                            ForegroundColor = DarkBlue;
                            Write(integerPart);
                            ForegroundColor = Red;
                            Write("point");
                            ForegroundColor = DarkBlue;
                            WriteLine(fractionalPart);
                            ResetColor();
                            WriteLine("");
                        } // End of if ((s_andInsertionForPseudo_scientificIsApplicable) &&
                           //                          (s_andInsertionForPseudo_scientificIsApplicable))
                    } // End of else (s_numberIsNegative)
                } // End of else (s_scaleSpecificationIsRequired)
            } // End of if (s_pseudo_scientificFormIsApplicable)
            WriteLine("Pseudo_scientific Expression with Significand as Digits");
            negativePrefix = s_numberIsNegative ? MinusSignString : string.Empty;
            WriteLine(TheConcatenationOf(negativePrefix,
                ThePseudo_scientificExpressionWithSignificandAsDigitsOf(s_integerPart, s_fractionalPart)));
            WriteLine("");
            // End of Pseudo_scientific Expressions

            // Ordinal Numerals
            if (s_ordinalIsApplicable)
            {
                if (s_scaleSpecificationIsRequired is false)
                {
                    // null
                    WriteLine("Ordinal Numeral as Word Group");
                    WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                    WriteLine("");
                    // e
                    if (s_andInsertionIsApplicable)
                    {
                        WriteLine("Ordinal Numeral as Word Group with \"and\"");
                        s_andInsertionIsSpecified = true;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        WriteLine("");
                    }
                    // g
                    if (s_aRepresenting1IsApplicable)
                    {
                        WriteLine("Ordinal Numeral as Word Group with \"a\" Representing 1");
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                    // eg
                    if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                    {
                        WriteLine("Ordinal Numeral as Word Group with \"and\" and \"a\" Representing 1");
                        s_andInsertionIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        s_aRepresenting1IsSpecified = false; 
                        WriteLine("");
                    }
                }
                else
                // s_scaleSpecificationIsRequired
                {
                    // null
                    WriteLine("Long Scale Ordinal Numeral as Word Group");
                    s_longScaleIsSpecified = true;
                    WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                    WriteLine("");
                    // null
                    WriteLine("Short Scale Ordinal Numeral as Word Group");
                    s_longScaleIsSpecified = false;
                    WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                    WriteLine("");
                    if (s_andInsertionIsApplicable)
                    {
                        // e
                        WriteLine("Long Scale Ordinal Numeral as Word Group with \"and\"");
                        s_longScaleIsSpecified = true;
                        s_andInsertionIsSpecified = true;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        WriteLine("");
                        // e
                        WriteLine("Short Scale Ordinal Numeral as Word Group with \"and\"");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        WriteLine("");
                    }
                    if (s_aRepresenting1IsApplicable)
                    {
                        // g
                        WriteLine("Long Scale Ordinal Numeral as Word Group with \"a\" Representing 1");
                        s_longScaleIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        WriteLine("");
                        // g
                        WriteLine("Short Scale Ordinal Numeral as Word Group with \"a\" Representing 1");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                    if ((s_andInsertionIsApplicable) && (s_aRepresenting1IsApplicable))
                    {
                        // eg
                        WriteLine("Long Scale Ordinal Numeral as Word Group with \"and\" and \"a\" Representing 1");
                        s_longScaleIsSpecified = true;
                        s_andInsertionIsSpecified = true;
                        s_aRepresenting1IsSpecified = true;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        WriteLine("");
                        // eg
                        WriteLine("Short Scale Ordinal Numeral as Word Group with \"and\" and \"a\" Representing 1");
                        s_longScaleIsSpecified = false;
                        WriteLine(TheEnglishOrdinalNumeralAsWordGroupFor(s_integerPart));
                        s_andInsertionIsSpecified = false;
                        s_aRepresenting1IsSpecified = false;
                        WriteLine("");
                    }
                } // End of else (s_scaleSpecificationIsRequired)
                WriteLine("Ordinal Numeral as Decimal Numeral");
                WriteLine(TheEnglishOrdinalNumeralAsDecimalNumeralFor(s_integerPart));
                WriteLine("");
            } // End of if (s_ordinalIsApplicable)
            WriteLine("");
            // End of ordinals

            // Scientific Notation
            WriteLine("Scientific Notation:");
            WriteLine("Normalized Scientific Notation");
            WriteLine(TheNormalizedScientificNotationExpressionOf(s_integerPart, s_fractionalPart));
            WriteLine("");
            WriteLine("Engineering Notation");
            WriteLine(TheEngineeringNotationExpressionOf(s_integerPart, s_fractionalPart));
            WriteLine("");
        } // End of GetHeadingsAndExpressions()
        public static string ProcessNumberForNegativity(string input)
        {
            // Processing disregards quantity and positions of minus signs.
            if (input.Contains(MinusSign))
            {
                s_numberIsNegative = true;
                input = input.Replace(MinusSignString, string.Empty);
            }
            else
                s_numberIsNegative = false; 
            return input;
        }
        public static string TheInputProcessedForNegativity(string input)
            => ProcessNumberForNegativity(input);
        public static string SolicitInput()
        {
            GiveInstructions();
            string? userInputString = ReadLine();
            if (string.Equals(userInputString, "x", StringComparison.OrdinalIgnoreCase))
                SignOff();
            return IsNullOrEmpty(userInputString) is false ?
                userInputString : string.Empty;
        } // End of SolicitInput
        public static string TheSolicitedInput() => SolicitInput();
        public static string ProcessInput()
        {
            string?
            input,
            filteredInput;
            bool? resolicitationIsRequired;
            // Input will be resolicited indefinitely until it is free of errors.
            do
            {
                input = TheSolicitedInput();
                if (ThisContainsNoDigits(input))
                    return "0";
                filteredInput =
                    IsNullOrEmpty(input) is false ? TheUsableCharactersOf(input) : string.Empty;
                if (ThisContainsErrors(filteredInput))
                {
                    // https://learn.microsoft.com/en-us/dotnet/api/system.consolecolor
                    BackgroundColor = Blue;
                    ForegroundColor = DarkBlue;
                    WriteLine("Errors were found in the number you entered, and it must be reentered.");
                    ResetColor();
                    resolicitationIsRequired = true;
                }
                else
                    resolicitationIsRequired = false;
            } while ((bool)resolicitationIsRequired);
            filteredInput = TheInputProcessedForNegativity(filteredInput);
            return filteredInput;
        } // End of ProcessInput
        public static string TheProcessedInput() => ProcessInput();
        public static void ExpressWelcome()
        {
            BackgroundColor = Magenta;
            ForegroundColor = Black;
            WriteLine("Welcome to \"Expressing Numbers With Words\"");
            // Thread.Sleep(3000);
            WriteLine();
            WriteLine("Numbers entered as digits will be expressed in English words.");
            ResetColor();
            // Thread.Sleep(2500);
            WriteLine();
        }
        #endregion Helper methods
        // The main method.  Computes the name of an integer or a decimal fraction.
        public static void GetEnglishNumeral()
        {
            ExpressWelcome();
            string? digitsWithPossiblePeriod;
/*         The enclosed statements will execute an indefinite number of times, once 
            for each number entered by the user, until they enter 'x' as an input 
            or press the code window's Stop button.                                                                       */
            while (true)
            {
                digitsWithPossiblePeriod = TheProcessedInput();
/*             Inputs containing no nonzero digits may be integers (such as "0", "0.", or "00") 
                or decimal fractions, such as 0.00.

                At this point digitsWithPossiblePeriod contains at least one digit and at most one period.
                Possibly output English Pseudo_scientific Expression with Significand as Words.                                                                       */
                s_integerPart = TheIntegerPartOf(digitsWithPossiblePeriod);
                // Re: https://en.wikipedia.org/wiki/Decimal
                s_fractionalPart = TheFractionalPartOf(digitsWithPossiblePeriod);  
                if (s_fractionalPart != string.Empty)
                    s_numberIsDecimalFraction = true;
                else
                    s_numberIsDecimalFraction = false;
                s_lengthOfIntegerPart = (ushort)s_integerPart.Length;
                if (s_lengthOfIntegerPart > 9)
                    s_scaleSpecificationIsRequired = true;
                else
                    s_scaleSpecificationIsRequired = false;
/*             When s_lengthOfIntegerPart is 5, 8, 11, 14... , initial '1' may not expressed by "a" or "an".
                In such a case s_lengthOfIntegerPart % 3 is 2. 1,000: may; 10,000: may not; 100,000: may.                                                 */
                if
                    (
                        s_integerPart[0] is '1'
                        &&
                        s_lengthOfIntegerPart % 3 is 0 or 1
                        &&
                        s_lengthOfIntegerPart >= 3
                    )
                    s_aRepresenting1IsApplicable = true;
                else
                    s_aRepresenting1IsApplicable = false;
                if
                    (
                        s_integerPart[0] is '1'
                        &&
                        s_lengthOfIntegerPart % 3 is 0 
                        &&
                        s_lengthOfIntegerPart >= 4
                    )
                    s_aRepresenting1ForPseudo_scientificIsApplicable = true;
                else
                    s_aRepresenting1ForPseudo_scientificIsApplicable = false;
                // The applicability of "and" insertion in integers and decimal fractions will be tested.
                s_andInsertionIsSpecified = true;
                string? testExpression = TheEnglishCardinalNumeralForTheInteger(s_integerPart);
                s_andInsertionIsSpecified = false;
                // Ignore "thousand"; search only for the conjunction "and".⤋
                s_andInsertionIsApplicable = testExpression.Contains(" and") ? true : false;
                // Condition permitting the insertion of "and" in Pseudo_scientific Expression with Significand as Wordss
                if
                    (
                        s_lengthOfIntegerPart >= 3
                        &&
                        // length divisible by 3: 3, 6, 9, 12, ...
                        s_lengthOfIntegerPart % 3 is 0
                        &&
                        // Field may not be of the form "a00bcd ..."
                        s_integerPart[1..3] is not "00"
                    )
                    s_andInsertionForPseudo_scientificIsApplicable = true;
                else
                    s_andInsertionForPseudo_scientificIsApplicable = false;
                if (s_lengthOfIntegerPart >= 4)
                {
                    if (s_numberIsDecimalFraction is false)
                    {
                        ushort? numberOfTrailing0s =
                            (ushort?)(s_lengthOfIntegerPart - s_integerPart.TrimEnd('0').Length);
                        //                     Value is 1, 2, or 3.       
                        byte? numberOfDigitsPreceding1stComma =
                            (byte?)(((s_lengthOfIntegerPart - 4) % 3) + 1);
                        ushort? numberOfDigitsFollowing1stComma =
                            (ushort?)(s_lengthOfIntegerPart - numberOfDigitsPreceding1stComma);
/*                     If a number such as 15,000 cannot be expressed with "point"+ non-0 digit,
                        the pseudo-scientific variant will not be displayed.

                        integerPart qualifies for Pseudo_scientific Expression with Significand as Words?
                        integerPart = 1,100 ⇒ "one point one thousand": yes; 1,000: no; 11,000: no;
                        11,500 ⇒ "eleven point five thousand": yes; 115,000: no                                                                   */
                        if (numberOfDigitsFollowing1stComma > numberOfTrailing0s)
                            s_pseudo_scientificFormIsApplicable = true;
                    } // End of if (s_numberIsDecimalFraction is false)
                    // s_numberIsDecimalFraction is true.
                    else
                        s_pseudo_scientificFormIsApplicable = true;
                } // End of if s_lengthOfIntegerPart >= 4 
                else
                    s_pseudo_scientificFormIsApplicable = false;
                // Not applicable for Pseudo_scientific Expression with Significand as Wordss.
                s_substituting100For1000IsApplicable = s_lengthOfIntegerPart is 4 ? true : false;
                s_ordinalIsApplicable =
                    ((s_fractionalPart == string.Empty) && (s_numberIsNegative is false)) ?
                    true : false;
                GetHeadingsAndExpressions();
            } // End of while (true)
        } // End of GetEnglishNumeral
    } // End of static class NumberExpression
    public static class StringAndArrayProcessing
    {
/*     Adapted from: 
        How do I concatenate two arrays in C#?
        https://stackoverflow.com/questions/1547252/how-do-i-concatenate-two-arrays-in-c   
        There see "More efficient (faster) to use BlockCopy over Array.CopyTo"
        Also see: https://stackoverflow.com/questions/1389821/array-copy-vs-buffer-blockcopy   */
        public static char[] ConcatenateTwoCharacterArrays(char[] sourceArray1, char[] sourceArray2)
        {
            uint?
            length1 = (uint?)sourceArray1.Length,
            length2 = (uint?)sourceArray2.Length,
            combinedLength = length1 + length2;
            if (combinedLength < 22)
            {
                string?
                st1 = Concat(sourceArray1),
                st2 = Concat(sourceArray2),
                concatenatedStrings = st1 + st2;
                return concatenatedStrings.ToCharArray();
            }
/*         Byte count of the character type is 2.
            Re:
            https://condor.depaul.edu/sjost/nwdp/notes/cs1/CSDatatypes.htm
            https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/char                                        */
            const byte charByteCount = 2;
            // Re: https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/nullable-value-types
            ushort?
            block1ByteCount = (ushort?)(charByteCount * length1),
            block2ByteCount = (ushort?)(charByteCount * length2),
            initialOffset = 0,
            sourceArray1Offset = 0,
            sourceArray2Offset = block1ByteCount;
            char[]? destinationArray = new char[(int)combinedLength];
/*         "BlockCopy" copies a specified number of bytes from a source array starting 
            at a particular offset to a destination array, starting at another offset.
            Re: https://learn.microsoft.com/en-us/dotnet/api/system.array.copy                                                           */
            BlockCopy(sourceArray1, (int)initialOffset, destinationArray,
                (int)sourceArray1Offset, (int)block1ByteCount);
            BlockCopy(sourceArray2, (int)initialOffset, destinationArray,
                (int)sourceArray2Offset, (int)block2ByteCount);
            return destinationArray;
        } // End of ConcatenateTwoCharacterArrays
        public static char[] TheConcatenationOf(char[] sourceArray1, char[] sourceArray2)
            => ConcatenateTwoCharacterArrays(sourceArray1, sourceArray2);
        // objectArray may contain a mix of char, integer, string, or array types.  
        public static char[] ConcatenateObjectsToArray(params object[] objectArray)
        {
            char[]? destinationArray = Empty<char>();
            for (ushort objectIndex = 0; objectIndex < objectArray.Length; objectIndex++)
            {
                object currentObject = objectArray[objectIndex];
                // If currentObject is a char array, tempArray is set to currentObject.
                if (currentObject is char[] tempArray)
                {
                    for
                        (
                            ushort tempArrayIndex = 0;
                            tempArrayIndex < tempArray.Length;
                            tempArrayIndex++
                        )
                    {
                        char ch1 = tempArray[tempArrayIndex];
                        destinationArray = TheConcatenationOf
                            (destinationArray, ch1.ToString().ToCharArray());
                    }
                }
                if (currentObject is char ch2)
                {
                    destinationArray = TheConcatenationOf
                        (destinationArray, ch2.ToString().ToCharArray());
                }
                if (currentObject is string st)
                {
                    destinationArray =
                        TheConcatenationOf(destinationArray, st.ToCharArray());
                }
                if (currentObject is int intgr)
                {
                    destinationArray = TheConcatenationOf
                        (destinationArray, intgr.ToString().ToCharArray());
                }
            } // End of outer "for"
            return destinationArray;
        } // End of ConcatenateObjectsToArray 
        // The objects may be a char, integer type, string, or array.
        public static string TheConcatenationOf(params object[] objects)
            => Concat(ConcatenateObjectsToArray(objects));
        public static IEnumerable<char> ConcatenateObjectsToIE<TSource>
            (params IEnumerable<TSource>[] objects)
        {
            IEnumerable<char> result = TheConcatenationOf(objects);
            return result;
        }
/*     If an item is in itemsToDelete, delete it from original.
        Call like this.: 
        string? filteredString1 =
            (string?)DeleteItems(originalStringAsString, itemsToDeleteAsString);
        Or:
        string? filteredString2 =
            DeleteItems((originalStringAsIE), (itemsToDeleteAsIE));                                            */
        public static IEnumerable<char>? DeleteItems<TSource>
            (this IEnumerable<TSource> original, IEnumerable<TSource> itemsToDelete)
        {
            // See Nullable value types at
            // https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/nullable-value-types
            string?
            itemToDeleteAsString = Concat(itemsToDelete),
            originalAsString = Concat(original),
            // Initialization
            filteredString = originalAsString;
            foreach (char ch in originalAsString)
            {
                if (itemToDeleteAsString.Contains(ch))
                    filteredString = filteredString.Replace(ch.ToString(), string.Empty);
            }
            IEnumerable<char>? filteredStringAsIE = filteredString;
            return filteredStringAsIE;
        }
        public static IEnumerable<char>? _with_these_deleted<TSource>
            (this IEnumerable<TSource> original, IEnumerable<TSource> itemsToDelete)
                => DeleteItems(original, itemsToDelete);
        //-------------------------------------------------------------------------------------------------
/*     If an item is not in charsToPreserve, delete it from original.
        Call as follows: 
        string? purifiedString1 =
            (string?)DeleteItems(originalStringAsString, itemsToPreserveAsString);
        Or:
        string? purifiedString2 =
            DeleteItems((originalStringAsIE), (itemsToPreserveAsIE));*/
        public static string? Purify(this string original, string charsToPreserve)
        {
            string? result = null;
            foreach (char ch in original)
            {
                if (charsToPreserve.Contains(ch))
                    result += ch;
            }
            return result;
        }
        public static string? WithOnly(this string original, string charsToPreserve)
                => Purify(original, charsToPreserve);
        public static IEnumerable<char>? Purify<TSource>
            (this IEnumerable<TSource> original, IEnumerable<TSource> itemsToPreserve)
        {
            string?
            itemsToPreserveAsString = Concat(itemsToPreserve),
            originalAsString = Concat(original),
            resultAsString = null;
            foreach (char ch in originalAsString)
            {
                if (itemsToPreserveAsString.Contains(ch))
                    resultAsString += ch;
            }
            IEnumerable<char>? result = resultAsString;
            return result;
        }
/*     Replace(Char, Char)	Returns a new string in which all occurrences of a specified 
        Unicode character in this instance are replaced with another specified Unicode character.

        Replace(String, String)	Returns a new string in which all occurrences of a specified
        string in the current instance are replaced with another specified string.

        Remove(Int32, Int32)	Returns a new string in which a specified number (2nd parameter)
        of characters in the current instance beginning at a specified position (1st parameter)
        have been deleted.                                                                                                                                  */
        public static IEnumerable<char>? WithOnlyThese<TSource>
            (this IEnumerable<TSource> original, IEnumerable<TSource> itemsToPreserve)
                => Purify(original, itemsToPreserve);
        public static IEnumerable<char>? WithOnly<TSource>
            (this IEnumerable<TSource> original, IEnumerable<TSource> itemsToPreserve)
                => Purify(original, itemsToPreserve);
        // Replace every instance of itemToReplace with "replacement".
        public static IEnumerable<char>? Replace<TSource>
            (this IEnumerable<TSource> container,
                IEnumerable<TSource> itemsToReplace, IEnumerable<TSource> replacement)
                        => container.Replace(itemsToReplace, replacement);
        public static IEnumerable<char>? Replace<TSource>
            (this IEnumerable<TSource> container,
                char charToReplace, IEnumerable<TSource> replacement)
        {
            string?
            containerAsString = Concat(container),
            charToReplaceAsString = Concat(charToReplace),
            replacementAsString = Concat(replacement),
            resultAsString =
                containerAsString.Replace(charToReplaceAsString, replacementAsString);
            IEnumerable<char>? resultAsIE = resultAsString;
            return resultAsIE;
        }
        public static IEnumerable<char>? Replace<TSource>
            (this IEnumerable<TSource> container, char charToReplace,
                char replacement)
        {
            string? containerAsString = Concat(container);
            IEnumerable<char>? result =
                containerAsString.Replace(charToReplace, replacement);
            return result;
        }
        public static IEnumerable<char>? Replace<TSource>
            (this IEnumerable<TSource> container,
                IEnumerable<TSource> itemToReplace, char replacement)
        {
            IEnumerable<char>? result =
                container.Replace(itemToReplace, replacement);
            return result;
        }
        public static IEnumerable<char>? WithThisReplacedByThat<TSource>
             (this IEnumerable<TSource> container, IEnumerable<TSource> itemToReplace,
                IEnumerable<TSource> replacement)
            => Replace(container, itemToReplace, replacement);
        public static IEnumerable<char>? DeleteIE<TSource>
            (this IEnumerable<TSource> container, IEnumerable<TSource> itemToDelete)
        {
            string?
            containerAsString = Concat(container),
            itemToDeleteAsString = Concat(itemToDelete),
            resultAsString =
                containerAsString.Replace(itemToDeleteAsString, string.Empty);
            IEnumerable<char>? result = resultAsString;
            return result;
        }
        public static IEnumerable<char>? WithThisDeleted<TSource>
            (this IEnumerable<TSource> container, IEnumerable<TSource> itemToDelete)
            => DeleteIE(container, itemToDelete);
        public static bool ThisContainsSomeOfThat<TSource>
            (this IEnumerable<TSource> collection1, IEnumerable<TSource> collection2)
        {
            IEnumerable<TSource> intersectionOfTheCollections =
                collection1.Intersect(collection2);
            if (intersectionOfTheCollections.Count() is not 0)
                return true;
            return false;
        }
        public static bool ContainsAny<TSource>
            (this IEnumerable<TSource> collection1, IEnumerable<TSource> collection2)
                => ThisContainsSomeOfThat(collection1, collection2);
        public static bool ContainsSomeOf<TSource>
            (this IEnumerable<TSource> collection1, IEnumerable<TSource> collection2)
                => ThisContainsSomeOfThat(collection1, collection2);
        public static bool ContainAny<TSource>
            (this IEnumerable<TSource> collection1, IEnumerable<TSource> collection2)
                => ThisContainsSomeOfThat(collection1, collection2);
        public static bool DoesNotContainAny<TSource>
            (this IEnumerable<TSource> collection1, IEnumerable<TSource> collection2)
                => !ThisContainsSomeOfThat(collection1, collection2);
        // Do is 3rd person plural indicative mood, not imperative.
        public static bool DoNotContainAny<TSource>
            (this IEnumerable<TSource> collection1, IEnumerable<TSource> collection2)
                => DoesNotContainAny(collection1, collection2);
        // Type of set parameters may not be Char.
        public static bool IsASubsetOf<TSource>
            (this IEnumerable<TSource> subset, IEnumerable<TSource> superset)
                => !WithThisDeleted(subset, superset).Any();
        public static bool IsNotASubsetOf<TSource>
            (this IEnumerable<TSource> subset, IEnumerable<TSource> superset)
                => !IsASubsetOf(subset, superset);
        public static bool AreASubsetOf<TSource>
            (this IEnumerable<TSource> subset, IEnumerable<TSource> superset)
                => IsASubsetOf(subset, superset);
        public static bool AreNotASubsetOf<TSource>
            (this IEnumerable<TSource> set1, IEnumerable<TSource> set2)
               => !IsASubsetOf(set1, set2);
        public static bool ThisContainsElementsNotInThat<TSource>
            (this IEnumerable<TSource> set1, IEnumerable<TSource> set2)
                => !IsASubsetOf(set1, set2);
        public static bool ContainsElementsNotIn<TSource>
            (this IEnumerable<TSource> set1, IEnumerable<TSource> set2)
                => !IsASubsetOf(set1, set2);
        public static bool ContainElementsNoIn<TSource>
            (this IEnumerable<TSource> set1, IEnumerable<TSource> set2)
                => ThisContainsElementsNotInThat(set1, set2);
        public static bool IsASupersetOf<TSource>
            (this IEnumerable<TSource> superset, IEnumerable<TSource> subset)
                => IsASubsetOf(subset, superset);
        public static bool ContainsOnlyElementsOf_<TSource>
            (this IEnumerable<TSource> subset, IEnumerable<TSource> superset)
                => IsASubsetOf(subset, superset);
        public static char[] ThisAsArray(char ch)
            => ch.ToString().ToCharArray();
        public static string ThisAsString(char[] ar)
            => new string(ar);
        public static string ToString(char ch)
            => new string(ch.ToString());
        /*     From: https://stackoverflow.com/questions/588774/how-can-you-remove-duplicate-characters-in-a-string
                See "A Linq approach".                                                                                            */
        public static string RemoveDuplicateCharacters(string chars)
            => new string(chars.ToCharArray().Distinct().ToArray());
        public static string TheDistinctCharactersOf(string chars)
            => RemoveDuplicateCharacters(chars);
        public static string IsTheDistinctCharactersOf(string chars)
            => RemoveDuplicateCharacters(chars);
        public static string AreTheDistinctCharactersOf(string chars)
            => RemoveDuplicateCharacters(chars);
        public static string ConvertSequenceToSet(string chars)
            => RemoveDuplicateCharacters(chars);
        public static string IsTheSetDerivedFrom(string chars)
            => RemoveDuplicateCharacters(chars);
        public static string AreTheSetDerivedFrom(string chars)
            => RemoveDuplicateCharacters(chars);
        public static string TheSetFor(string chars)
            => RemoveDuplicateCharacters(chars);
        public static IEnumerable<char>? GetDistinctCharacters<TSource>
            (IEnumerable<TSource> original)
        {
            string?
            originalAsString = Concat(original),
            resultAsString = string.Empty;
            foreach (char ch in originalAsString)
            {
                if (resultAsString.Contains(ch) is false)
                    resultAsString += ch;
            }
            IEnumerable<char>? resultAsIE = resultAsString;
            return resultAsIE;
        }
        public static IEnumerable<char>? TheDistinctCharactersOf<TSource>
            (IEnumerable<TSource> original)
                => GetDistinctCharacters(original);
        // https://code-maze.com/csharp-how-to-delete-elements-from-an-array 
        public static char[]
            Delete1stOccurrenceOfCharInArray(char[] inputArray, char characterToRemove)
        {
            int? indexOfCharacterToRemove =
                 IndexOf(inputArray, StringComparison.OrdinalIgnoreCase, characterToRemove);
            // if inputArray does not contain characterToRemove 
            if (indexOfCharacterToRemove < 0)
                return inputArray;
            char[] newArray = new char[inputArray.Length - 1];
            Copy(inputArray, 0, newArray, 0, (int)indexOfCharacterToRemove);
            Copy(inputArray, (int)(indexOfCharacterToRemove + 1),
                newArray, (int)indexOfCharacterToRemove,
                     (int)(inputArray.Length - indexOfCharacterToRemove - 1));
            return newArray;
        } // End of DeleteArrayElement
        // From the second C# method: https://www.geeksforgeeks.org/power-set/
        // Get the set of all subsets of a set.
        public static List<string> GetPowerSet(string input)
        {
            byte? inputLength = (byte?)input.Length;
            List<string> powerSet = new List<string>();
/*         Power set contains 2^inputLength subsets.
            https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/bitwise-and-shift-operators#left-shift-operator-
            The left-shift operator << shifts its left-hand operand left by the number of bits
            defined by its right-hand operand.                                                                                      */
            for (ushort i = 0; i < (1 << inputLength); i++)
            {
                string? subset = string.Empty;
                for (ushort j = 0; j < inputLength; j++)
                {
                    // If the j-th bit is set in i, include the j-th character from s.
                    if ((i & (1 << j)) != 0)
                        subset += input[j];
                }
                powerSet.Add(subset);
            }
            return powerSet;
        } // End of GetPowerSet
        public static List<string> ThePowerSetOf(string input)
            => GetPowerSet(input);
    } // End of class StringAndArrayProcessing 
} // End of namespace ExpressionOfNumbersInEnglish
/*  
Appendix A
Capacities of types
                     Lower bound                          Upper bound                   
Integral types
sbyte:	                                   -128                                          127	            Signed 8-bit integer 
byte:	                                            0                                          255	            Unsigned 8-bit integer	 
short:	                              -32,768                                     32,767	            Signed 16-bit integer	 
ushort:	                                         0                                     65,535	            Unsigned 16-bit integer	 
int:	                       -2,147,483,648                         2,147,483,647	            Signed 32-bit integer	 
uint:	                                             0                         4,294,967,295	            Unsigned 32-bit integer	 
long: -9,223,372,036,854,775,808    9,223,372,036,854,775,807              Signed 64-bit integer	 
ulong:	                                         0  18,446,744,073,709,551,615	            Unsigned 64-bit integer	 
nint:	        Depends on platform (computed at runtime)	                            Signed 32-bit or 64-bit integer 
nuint:	    Depends on platform (computed at runtime) 
Floating-point types     
float:              -3.40282347 × 10³⁸                    3.40282347 × 10³⁸             6-9 digits      32 bits  4 bytes	 
double:	 -1.79769313486232 × 10³⁰⁸   1.79769313486232 × 10³⁰⁸  15-17 digits   64 bits  8 bytes	 
decimal: -7.9228162514264337593543950335 × 10²⁸                 28-29 digits 128 bits 16 bytes
                                         7.9228162514264337593543950335 × 10²⁸

Re: https://learn.microsoft.com/en-us/cpp/c-language/maximum-string-length
An individual quoted string cannot be longer than 2048 bytes, but a string literal
of roughly 65535 bytes can be constructed by concatenating strings.
Quoted string length:                                                1,024                   2,048 bytes
Concatenated string length:                                    32,767                 65,535 bytes

Appendix B  
De Morgan's laws
Re: https://en.wikipedia.org/wiki/De_Morgan's_laws
The complement of the union of two sets is the same as the intersection of their complements. 
 ¬(A ˅ B) ⇔ ¬A ˄ ¬B
!(A || B) is the same as !A && !B

The complement of the intersection of two sets is the same as the union of their complements.
 ¬(A ˄ B) ⇔ ¬A ˅ ¬B
!(A && B) is the same as !A || !B

Appendix C
Range operator notation
Examples
Let var st0 be "34567"
st0[..^2] is "345" Omit last 2.
st0[2..] is "567" Omit first 2.
st0[2..^1] is "56" Omit 1st 2 and last 1. Length is the difference in indices plus one if only one has ^.
st0[..3] is "345" Select 1st 3.
st0[2..4] is "56" Omit 1st 2 and include to index 3. Length is the difference in indices if neither has ^.
st0[^4..^2] is "45" Select from 4th from end to 3rd from end.
Length is the difference in indices if both do or don't have ^.
st0[^3..] is "567" Select last 3 chars.
If the value in [] contains two dots, a string is reported; if not, a character.
Except for [0], [] should not contain zeros.

Appendix D
https://learn.microsoft.com/en-us/dotnet/api/system.consolekey?view=net-8.0
Specifies the standard keys on a console, like enter and backspace.

Appendix E
Naming conventions and other rules for fields

Appendix F
Potential features
Fractions: one fourth
Bidding numbers: one sixty, twelve fifty, five and a quarter
12.3 => twelve and three tenths
scientific and engineering notation
Output all possible forms instead of just a certain form specified by answers to queries!

Appendix G
Unused formulae
ushort occurrencesOfAnd = (ushort)Regex.Matches(englishCardinalNumeral, "and").Count();
Appendix H
Sections under construction
2759 QueryForScientificNotation

Appendix I
Module under development

        ScientificNotation 
        {// May have more numerical form: 5.3 x 10^4
            BackgroundColor = DarkBlue;
            ForegroundColor = Yellow;
            WriteLine("Shall this number be expressed using \"normalized scientific notation\"?\n" +
                    "E.g. 987 ⇒ nine point eight seven times ten square or\n" +
                    "- 53,200 ⇒ minus five point three two times ten to the fourth");
            ResetColor();
            // Normalized scientific notation is selected.
            if (TheAnswerIsYes())
            {
                bool? scientificNotationSpecified = true;
                s_normalizedScientificNotationIsSpecified = true;
                WriteLine("Shall the number be expressed in word form, rather than in numerical form?\n" +
                    "Word form: 987 ⇒ nine point eight seven times ten square\n" +
                    "Numerical form: - 53,200 ⇒ 5.32 × 10⁴");
            }
        } // End of QueryForNormalizedScientificNotation

“In a field declaration, readonly indicates that assignment to the field can only occur
as part of the declaration or in a constructor in the same class. A readonly field can be
assigned and reassigned multiple times within the field declaration and constructor.”
https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/readonly

“A field is a variable of any type that is declared directly in a class or struct.”
https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/fields

“Generally, you should declare private or protected accessibility for fields. Data that
your type exposes to client code should be provided through methods, properties, and indexers.”
https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/fields

“The static keyword should be applied to all members of static classes.”
(in a static class fields should be declared as static)

“Private instance fields start with an underscore (_) and the remaining text is camelCased.”

“Use PascalCase for constant names, both fields and local constants.”

“Static fields start with s_. This convention isn't the default Visual Studio behavior, nor part
of the Framework design guidelines, but is configurable in editorconfig.”
https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/identifier-names

Pascal case used for public fields per:
https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions
******************************************************************************
Notes

https://michaelscodingspot.com/7-debugging-techniques-for-when-your-net-application-freezes-hangs/

Relevant technologies: Blazor, Maui, WPF, HTML, XML, XAML, GitHub Pages: static site hosting service provided by GitHub.

See I Chronicles 21:5 NIV
And is not colloquial: four hundred and seventy thousand 
one million one hundred thousand   large number in Bible

Model website for number calculation:
https://www.calculatorsoup.com/calculators/conversions/numberstowords.php

Power set of "bcefghijlm";// b , c, e, f, g, h, i, j, l, m
https://www.mathsisfun.com/sets/power-set-maker.html

*/
