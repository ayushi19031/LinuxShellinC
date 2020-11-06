# Basic-Linux-Shell-in-C

This is a very simple shell designed in C that performs basic operations of various commands in linux using linux system calls.


1. System calls: write and read for all the commands
ii. fork ,execv , waitpid for all external commands
 
i. cd: getcwd() and chdir()
ii. pwd: getpwd(), getcwd(), getenv()
iii. echo: read() and write(). for echo* : opendir();
iv. history: read() , open();
v. mkdir: mkdir(), read();
vi. rm: remove()
vii. cat: read(), write()
viii. date: time library of c. 
ix. ls: opendir() and read() and write();

options implemented in each command: 
1. cd - .. 
2. pwd: -L  and -P
3. echo -n and -E and *
4. history: -c and !! 
5. mkdir: -v and -p
6. rm: -i and -f 
7. cat: -n and -e
8. date: -u and -R
9. ls: -1 and -Q
10. exit: 

ERROR HANDLING: 
1. cd: the directory not found and invalid option 
2. rm: perror no. 2 and perror no. 39
3. ls: invalid option and directory not found
4. history: invalid option
5. echo: invalid option and unable to print the string
6. pwd: invalid option and unable to get the directory
7. mkdir: directory does not exist or it is a file
8. cat: file does not exist ad file is a directory
9. date: invalid option 
10. exit: any option will be considered invalid
11. fork: Not able to start child process
