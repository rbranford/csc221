# Part 1

**Searching for words across files**

    - The best way to search for words in multiple files was using the grep command

    - The user needs to cd into the location of the files they are wanting to search

    - Next the user will use the command grep -l <word you are searching for> f*

    - -l prints the file(s) containing the word searched for

    - f* tells the command to search for the word whose file names begin with an f ex. file00000, file00102, etc. 

**Moving files**

    - The command I used to move the files matching my search was mv

    - mv $(grep -l <word> f*) ../<word>

    - The above command while place all file instances in the directory I choose at the end of the command 

    - ../<word> and word is considered my directory in this example 

    - I could also list out the exact location of the directory as well 


# Part 2

**Task 1**

    - The command beginning with the word sort, allows me to place my list in alphabetical order

    - Even if the words repeat it will list all instances before continuing to the next set of words in order

    - The > allows me to create a new .txt file with my new sorted list of words 
    
    - The command I ran in my bash terminal was 
    
        sort shuffled-words.txt > shuffled-words-sorted.txt

**Task 2**

    - As listed in the previous task, the sort command sorts my list in alphabetical order

    - The list I am using is a rand-words.txt

    - I use the uniq -c command after typing the file I am wanting to use

    - The uniq -c counts my words 

    - -nr will make my list sort numerically in a reverse fashion for example:

        dog 10
        cat 5
        bird 3

    - head -10 will list my top 10 words in reverse numerical order with how many times each of those words occured 

    - Lastly as listed in task 1, the > allows me to create a new .txt file with my new sorted list of words 

    - The command I ran was 
    
        sort rand-words.txt | uniq -c | sort -nr |head -10 > common-words.txt

**Task 3**

    - This task is very similar to the previous task only using numbers in a .txt file

    - I ran this command once using only the -n and it gave me a list of 10 numbers but only showing that each of them occured once

    - Be sure to use the -nr portion so that you get the numerically reverse sorted listed of most occurences of each number  

    - The command I ran was 

        sort rand-numbers.txt | uniq -c | sort -nr | head -10 > common-numbers.txt

**Task 4**

    - The previous command of 

        sort rand-numbers-2.txt | uniq -c | sort -nr| head -10 > common-2.txt

        Has the same functionality and allows for me to check on the pairs of numbers

    The only difference I have between task 3 and 4 is the .txt file to pull info from and to send the new info to

**Task 5**

    - I was unable to sort out by columns as listed in the instructions

        1, 2, 3
        2, 3, 4
        3, 4, 5
        1, 3, 4
        1, 4, 5
        1, 3, 5
        2, 4, 5

    - I was able to create a list of the top 10 of each set of five numbers like in task 4 