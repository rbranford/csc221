PROCESS MANAGEMENT

    ### If we would like to get a snapshot of what is currently happening on the system we may use a program called top.

        top

__Example__

    Tasks: 174 total, 3 running, 171 sleeping, 0 stopped
    KiB Mem: 4050604 total, 3114428 used, 936176 free
    Kib Swap: 2104476 total, 18132 used, 2086344 free
    
    PID USER %CPU %MEM COMMAND
    6978 ryan 3.0  21.2 firefox
    11 root 0.3   0.0 rcu_preempt
    6601 ryan 2.0   2.4 kwin
    ...

__Commands__

    ps[aux]
    ### ps stands for process
    ### aux shows a complete system view 

    kill [signal] <PID>
    ### used to kill a process 
    ### Normal users may only kill processes which they are       the owner for. The root user on the system may kill anyones processes.


    CTRL + ALT + F<Console>
    ### used to swicth between consoles in the event that your desktop locks up 


    CTRL + z 
    ### currently running foreground process will be paused and moved into the background

__Other programs__

    sleep - waits a given number of seconds then quits

    jobs - list currently running background jobs

    fg<job number> - brings background processes into the foreground 
    ### Example ###

        sleep 15 &
        [1] 21637
        sleep 10
        (you press CTRL + z, notice the prompt comes back.)
        jobs
        [1]- Running sleep 15 &
        [2]+ Stopped sleep 10
        fg 2
        [1] Done sleep 15

__Concepts__

    Control
        We have quite a bit of control over the running of our programs.
