Detailed overview of ah commands
--------------------------------
```bash
user@telos:~$ # list all ah-supported projects
user@telos:~$ . ah ls
temp1	/home/user/tmp/ahsamp/ah/temp1
temp2	/home/user/tmp/ahsamp/ah/temp2
temp3	/home/user/tmp/ahsamp/ah/temp3
proj1	/home/user/tmp/ahsamp/ah/proj1.git/ahlogs
proj2	/home/user/tmp/ahsamp/ah/proj2.git/ahlogs
user@telos:~$ # add a project
user@telos:~$ # add a project (project name and log directory are arguments)
user@telos:~$ . ah add proj3 /home/user/tmp/ahsamp/ah/proj3/ahlogs 
Successfully created project  proj3  in  /home/user/tmp/ahsamp/ah/proj3/ahlogs
user@telos:~$ # start working on the project
user@telos:~$ . ah resume proj3
proj3	/home/user/tmp/ahsamp/ah/proj3/ahlogs
Resuming proj3 project. Saving in directory:  /home/user/tmp/ahsamp/ah/proj3/ahlogs/proj3
user@telos:~[ah:proj3]$ echo "command in proj3"
command in proj3
user@telos:~[ah:proj3]$ # see project history
user@telos:~[ah:proj3]$ . ah history
 . ah resume proj3
 echo "command in proj3"
 # see project history
user@telos:~[ah:proj3]$ #see detailed project history(with command issue time and corresponding directory)
user@telos:~[ah:proj3]$ . ah history -a
Wed Sep 10 15:14:56 IST 2014	/home/user	 . ah resume proj3
Wed Sep 10 15:15:13 IST 2014	/home/user	 echo "command in proj3"
Wed Sep 10 15:15:25 IST 2014	/home/user	 # see project history
Wed Sep 10 15:15:29 IST 2014	/home/user	 . ah history
Wed Sep 10 15:15:53 IST 2014	/home/user	 #see detailed project history(with command issue time and corresponding directory)
user@telos:~[ah:proj3]$ # exit project 
user@telos:~[ah:proj3]$ . ah exit
leaving ah project environment.. Bye...
user@telos:~$ # remove project from ah
user@telos:~$ . ah rm temp1
temp1	/home/user/tmp/ahsamp/ah/temp1
Successfully deleted project
user@telos:~$ # change project log directory
user@telos:~$ . ah edit temp2 /home/user/tmp/ahsamp/ah/temp4 
temp2	/home/user/tmp/ahsamp/ah/temp2
Successfully deleted project
Successfully created project  temp2  in  /home/user/tmp/ahsamp/ah/temp4
user@telos:~$ . ah exit
leaving ah project environment.. Bye...
```
