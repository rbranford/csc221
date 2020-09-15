BASH SCRIPTING 

### A Bash script allows us to define a series of actions which the computer will then perform without us having to enter the commands ourselves. If a particular task is done often, or it is repetetive, then a script can be a useful tool.

### Anything you can run on the command line you may place into a script and they will behave exactly the same. Vice versa, anything you can put into a script, you may run on the command line and again it will perform exactly the same.

__Example__

    cat myscript.sh
    #!/bin/bash
    # A simple demonstration script
    # Ryan 15/9/2020
    
    echo Here are the files in your current directory:
    ls
    ls -l myscript.sh
    -rwxr-xr-x 1 ryan users 2 Jun 4 2012 myscript.sh
    ./myscript.sh
    Here are the files in your current directory:
    barry.txt bob example.png firstfile foo1 myoutput video.mpeg

__Programs__

    which<program> - locates our interpreter

__Additional info__

    comments - a note in a script that does not get run 

    $0 - The name of the script

    $1 - $9 - Any command line arguments given to the script
    $1 is the first argument, $2 the second and so on

    $# - How many command line arguments were given to the script

    $* - All of the command line arguments

### A script must have the execute permission before we may run it (even if we are the owner of the file). For safety reasons, you don't have execute permission by default so you have to add it. A good command to run to ensure your script is set up right is chmod 755 <script>.

__Variables example__

        cat variableexample.sh
        #!/bin/bash
        # A simple demonstration of variables
        # Ryan 15/9/2020
        
        name='Ryan'
        echo Hello $name
        ./variableexample.sh
        Hello Ryan

__If statement example__

        cat projectbackup.sh
    #!/bin/bash
    # Backs up a single project directory
    # Ryan 15/9/2020
    
    if [ $# != 1 ]
    then
        echo Usage: A single argument which is the directory to backup
        exit
    fi
    if [ ! -d ~/projects/$1 ]
    then
        echo 'The given directory does not seem to exist (possible typo?)'
        exit
    fi
    date=`date +%F`
    
    # Do we already have a backup folder for todays date?
    if [ -d ~/projectbackups/$1_$date ]
    then
        echo 'This project has already been backed up today, overwrite?'
        read answer
        if [ $answer != 'y' ]
        then
            exit
        fi
    else
        mkdir ~/projectbackups/$1_$date
    fi
    cp -R ~/projects/$1 ~/projectbackups/$1_$date
    echo Backup of $1 completed

__Concepts__

    Behaves the same
        Anything you may do on the command line you may do in a script and it will behave exactly the same
    Formatting
        Bash scripts are particularly picky when it comes to formatting. Make sure spaces are put where they are needed and not put when they are not needed