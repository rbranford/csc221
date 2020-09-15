PERMISSIONS

__Different permissions__

    r read - you may view the contents of the file
    w write - you may change the contents of the file
    x execute - you may execute or run the file if it is a program or script

    ### Specific permissions

        owner - a single person who owns the file (typically the person who created the file but ownership 
        may be granted to some one else by certain users)

        group - every file belongs to a single group

        others - everyone else who is not in the group or the owner

        1. * To view permissions (ls -l [path]) *
        2. * To change permissions (chmod [permissions] [path]) *
            2a. made up of 3 components 

    ### Directory permissions

        r - you have the ability to read the contents of the directory (ie do an ls)
        w - you have the ability to write into the directory (ie create files and directories)
        x - you have the ability to enter that directory (ie cd)


__Concepts__

    Security
        Correct permissions are important for the security of a system.
    Usage
        Setting the right permissions is important in the smooth running of certain tasks on Linux. (we will 
        see an example of this in Section 13 on scripting)
