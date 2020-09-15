FILTERS

### A filter, in the context of the Linux command line, is a program that accepts textual data and then transforms it in a particular way. Filters are a way to take raw data, either produced by another program, or stored in a file, and manipulate it to be displayed in a way more suited to what we are after

__Commands__

    head [-number of lines to print] [path] - view the first n lines of data

    tail [-number of lines to print] [path] - view the last n lines of data

    sort [-options] [path] - organize the data into order 

    nl [-options] [path] - number lines - print line numbers before data

    wc [-options] [path] - word count 

    cut [-options] [path] - cut the data into fields 

    sed <expression> [path] - stream editor

    uniq [options] [path] - unique

    tac [path]

    ###  Additional commands 

        awk
        diff

__Concepts__

    Processing
        Filters allow us to process and format data in interesting ways.
    man pages
        Most of the programs we looked at have command line options that allow you to modify their behaviour.

__Examples__

    * beginning 
    cat mysampledata.txt
    Fred apples 20
    Susy oranges 5
    Mark watermellons 10
    Robert pears 5
    Terry oranges 10
    Lisa peaches 10
    Susy oranges 15    
    Mark grapes 40
    Anne mangoes 5
    Greg pineapples 5
    Oliver rockmellons 5
    Betty limes 15

    * end

    tac mysampledata.txt
    Betty limes 14
    Oliver rockmellons 2
    Greg pineapples 3
    Anne mangoes 7
    Mark grapes 39
    Susy oranges 12
    Lisa peaches 7
    Terry oranges 9
    Robert pears 4
    Mark watermellons 12
    Susy oranges 5
    Fred apples 20