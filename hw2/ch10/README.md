GREP AND REGULAR EXPRESSIONS

__eGrep__

    egrep is a program which will search a given set of data and print every line which contains a given pattern. It is an extension of a program called grep

    egrep [command line options] <pattern> [path]

__Examples__

cat mysampledata.txt
Fred apples 20
Susy oranges 5
Mark watermellons 12
Robert pears 4
Terry oranges 9
Lisa peaches 7
Susy oranges 12
Mark grapes 39
Anne mangoes 7
Greg pineapples 3
Oliver rockmellons 2
Betty limes 14

egrep 'mellon' mysampledata.txt
Mark watermellons 12
Oliver rockmellons 2

__Troubleshooting__

    1. First off, check for typo's. If you're like me then you're prone to making them.

    2. Re read the content here. Maybe what you thought a particular operator did was slightly different to what it actually does and re reading you will notice a point you may have missed the first time.

    3. Break your pattern down into individual components and test each of these individually. This will help you to get a feel for which parts of the pattern is right and which parts you need to adjust.

    4. Examine your output. Your current pattern may not have worked the way you want but we can still learn from it. Looking at what we actually did match and using it to help understand what actually did happen will help us to work out what we should try changing to get closer to what we actually want.

    ### Useful external tool * Debuggex *

__Regular Exptressions__

    . (dot) - a single character.
    ? - the preceding character matches 0 or 1 times only.
    * - the preceding character matches 0 or more times.
    + - the preceding character matches 1 or more times.
    {n} - the preceding character matches exactly n times.
    {n,m} - the preceding character matches at least n times and not more than m times.
    [agd] - the character is one of those included within the square brackets.
    [^agd] - the character is not one of those included within the square brackets.
    [c-f] - the dash within the square brackets operates as a range. In this case it means either the letters c, d, e or f.
    () - allows us to group several characters to behave as one.
    | (pipe symbol) - the logical OR operation.
    ^ - matches the beginning of the line.
    $ - matches the end of the line.

__Concepts__

    Regular Expressions
        A powerful way to identify particular pieces of information.



