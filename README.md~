ah: Augmented History for BASH environment
------------------------------------------
Maintain project specific bash command histories
------------------------------------------------

If you work on several software projects on your machine, maintaining the command history for each project separately can be a big headache. You can get an overall history through the 'history' command, but searching for individual project's history can be difficult. 'ah' helps to address this issue. 

With 'ah' you can store your project histories separately(can save them in a project directory). After the 'ah' session for a project is started for a terminal, remaining commands will be saved for the project separately. 'ah' seamlessly integrates with bash. The following command typescript is self-explanatory for its use.
```bash
user@telos:~$ # working on project 1
user@telos:~$ . ah resume proj1
proj1	/home/user/tmp/ahsamp/ah/proj1.git/ahlogs
Resuming proj1 project. Saving in directory:  /home/user/tmp/ahsamp/ah/proj1.git/ahlogs/proj1
user@telos:~[ah:proj1]$ ls
user@telos:~[ah:proj1]$ echo "this is a command for proj1"
this is a command for proj1
user@telos:~[ah:proj1]$ # stoping work on project 1
user@telos:~[ah:proj1]$ . ah exit
leaving ah project environment.. Bye...
user@telos:~$ # starting work on project 2
user@telos:~$ . ah resume proj2
proj2	/home/user/tmp/ahsamp/ah/proj2.git/ahlogs
Resuming proj2 project. Saving in directory:  /home/user/tmp/ahsamp/ah/proj2.git/ahlogs/proj2
user@telos:~[ah:proj2]$ echo "command in project 2"
command in project 2
user@telos:~[ah:proj2]$ # stopping project 2 work
user@telos:~[ah:proj2]$ . ah exit
leaving ah project environment.. Bye...
user@telos:~$ # back to work on project 1
user@telos:~$ . ah resume proj1
proj1	/home/user/tmp/ahsamp/ah/proj1.git/ahlogs
Resuming proj1 project. Saving in directory:  /home/user/tmp/ahsamp/ah/proj1.git/ahlogs/proj1
user@telos:~[ah:proj1]$ #oops! forgot last commands. Let me check.
user@telos:~[ah:proj1]$ . ah history
 . ah resume proj1
 ls
 echo "this is a command for proj1"
 # stoping work on project 1
 . ah resume proj1
 #oops! forgot last commands. Let me check.
user@telos:~[ah:proj1]$ # leaving project 1
user@telos:~[ah:proj1]$ . ah exit
leaving ah project environment.. Bye...
```

Install ah as follows:

```bash
cd src
sudo ./install
```

An overview of all possible commands is available in: [file](https://github.com/harisankarh/ah/blob/master/examples/commands.md)

