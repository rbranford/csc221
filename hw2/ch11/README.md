PIPING AND REDIRECTION

__Data Streams__

    STDIN (0) - Standard input (data fed into the program)

    STDOUT (1) - Standard output (data printed by the program, defaults to the terminal)

    STDERR (2) - Standard error (for error messages, also defaults to the terminal)


__Redirecting from a file__

    ### Example
        wc -l myoutput
        8 myoutput
        wc -l < myoutput
        8

        wc -l < barry.txt > myoutput
        cat myoutput
        7
        
__Piping__

    ### Example
        barry.txt bob example.png firstfile foo1 myoutput video.mpeg
        ls | head -3
        barry.txt
        bob
        example.png

        ls | head -3 | tail -1
        example.png

__Summary__

    >
        Save output to a file.
    >>
        Append output to a file.
    <
        Read input from a file.
    2>
        Redirect error messages.
    |
        Send the output from one program as input to another program.

__Concepts__

    Streams
        Every program you may run on the command line has 3 streams, STDIN, STDOUT and STDERR.


