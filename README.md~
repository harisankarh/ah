ah: Augmented History for BASH environment.
Maintain Maintain project specific bash command histories
---------------------------------------------------------

If you work on several software projects on your machine, maintaining the command history for each project separately can be big headache. You can get an overall through the 'history' command, but searching for invidual project's history can be a headache. 'ah' helps to address this issue. 

With 'am' you can store your project histories separately(can save them in a project directory). After the 'ah' session for a project is started for a terminal, remaining commands will saved for the prject separately. 'ah' seamlessly integrates with bash. The following command typescript is self-explanatory for its use

harisankarh@telos:~$ # adding project 1
harisankarh@telos:~$ . ah add proj1 /home/harisankarh/tmp/ahsamp/ah/proj1.git/ahlogs 
Successfully created project  proj1  in  /home/harisankarh/tmp/ahsamp/ah/proj1.git/ahlogs
harisankarh@telos:~$ # adding project 2
harisankarh@telos:~$ . ah add proj2 /home/harisankarh/tmp/ahsamp/ah/proj2.git/ahlogs 
Successfully created project  proj2  in  /home/harisankarh/tmp/ahsamp/ah/proj2.git/ahlogs
harisankarh@telos:~$ # working on project 1
harisankarh@telos:~$ . ah resume proj1
proj1	/home/harisankarh/tmp/ahsamp/ah/proj1.git/ahlogs
Resuming proj1 project. Saving in directory:  /home/harisankarh/tmp/ahsamp/ah/proj1.git/ahlogs/proj1
harisankarh@telos:~[ah:proj1]$ ls
harisankarh@telos:~[ah:proj1]$ echo "this is a command for proj1"
this is a command for proj1
harisankarh@telos:~[ah:proj1]$ # stoping work on project 1
harisankarh@telos:~[ah:proj1]$ . ah exit
leaving ah project environment.. Bye...
harisankarh@telos:~$ # starting work on project 2
harisankarh@telos:~$ . ah resume proj2
proj2	/home/harisankarh/tmp/ahsamp/ah/proj2.git/ahlogs
Resuming proj2 project. Saving in directory:  /home/harisankarh/tmp/ahsamp/ah/proj2.git/ahlogs/proj2
harisankarh@telos:~[ah:proj2]$ echo "command in project 2"
command in project 2
harisankarh@telos:~[ah:proj2]$ # stopping project 2 work
harisankarh@telos:~[ah:proj2]$ . ah exit
leaving ah project environment.. Bye...
harisankarh@telos:~$ # back to work on project 1
harisankarh@telos:~$ . ah resume proj1
proj1	/home/harisankarh/tmp/ahsamp/ah/proj1.git/ahlogs
Resuming proj1 project. Saving in directory:  /home/harisankarh/tmp/ahsamp/ah/proj1.git/ahlogs/proj1
harisankarh@telos:~[ah:proj1]$ #oops! forgot last commands. Let me check.
harisankarh@telos:~[ah:proj1]$ . ah history
 . ah resume proj1
 ls
 echo "this is a command for proj1"
 # stoping work on project 1
 . ah resume proj1
 #oops! forgot last commands. Let me check.
 . am history
harisankarh@telos:~[ah:proj1]$ # leaving project 1
harisankarh@telos:~[ah:proj1]$ . ah exit
leaving ah project environment.. Bye...



