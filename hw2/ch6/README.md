TEXT EDITOR

__Command line editor__

    1. insert mode
    2. edit mode

    vi <file> - edit a file 
    cat <file> - view a file
    less <file> - convenient for viewing large files

    ### You may go forward a whole page using the SpaceBar or back a page by pressing b. When you are done you can press q for quit.

__Saving and exiting__

    ZZ (Note: capitals) - Save and exit
    :q! - discard all changes, since the last save, and exit
    :w - save file but don't exit
    :wq - again, save and exit

__Navigating inside a vi file__

    Arrow keys - move the cursor around
    j, k, h, l - move the cursor down, up, left and right (similar to the arrow keys)
    ^ (caret) - move cursor to beginning of current line
    $ - move cursor to end of the current line
    nG - move to the nth line (eg 5G moves to 5th line)
    G - move to the last line
    w - move to the beginning of the next word
    nw - move forward n word (eg 2w moves two words forwards)
    b - move to the beginning of the previous word
    nb - move back n word
    { - move backward one paragraph
    } - move forward one paragraph

__Deleting and undoing content__

    x - delete a single character
    nx - delete n characters (eg 5x deletes five characters)
    dd - delete the current line
    dn - d followed by a movement command. Delete to where the movement command would have taken you. (eg d5w means delete 5 words)

    u - Undo the last action (you may keep pressing u to keep undoing)
    U (Note: capital) - Undo all changes to the current line

__Concepts__

    ### No mouse needed 
    ### Practice edit commands, there are many