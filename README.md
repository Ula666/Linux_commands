# Linux Commands and Practices:

 1. how to check Hidden Files and Directories: `ls -a`, `dir -a` a - all
 2. The Manual, Flags `man` Shows manual pages for Linux commands.
 3. What are a wildecards and How to use Wildcards: 
- Wildcards (also referred to as meta characters) are symbols or special characters that represent other characters. You can use them with any command such as ls command or rm command to list or remove files matching a given criteria, receptively.
- An asterisk (*) – matches one or more occurrences of any character, including no character.
- Question mark (?) – represents or matches a single occurrence of any character.
- Bracketed characters ([ ]) – matches any occurrence of character enclosed in the square brackets. It is possible to use different types of characters (alphanumeric characters): numbers, letters, other special characters etc.  

 4. how can you do Process Management
- `ps` To display your currently active processes
- `ps aux` To see an incredibly detailed list of processes (a - all users, u - shows the user/owner, x - displays processes not executed in the terminal)  

 5. What is Currently Running on your system `ps`
 6. Killing a process/Crashed Process `ps aux | grep chrome` 
 7. How to check any process running in Foreground and Background Jobs:
- `sleep 10000` - example of the foreground process. This is just a simple sleep command that will return the prompt to the user only after it is completed.  
- Background process runs your process in the background and will not take control of your terminal prompt. You can start a session and you are free to use your terminal. To submit a command as a background process you have to add & symbol at the end of the command. `sleep 50000 &`  
- `jobs -l` - To get the list of jobs either in running or stopped state  

 8. How to stop/kill any process running in Foreground and Background Jobs
- `sudo pkill name` - is one of the commands that can directly kill a background process, using the process name.

 9. How to change permissions with chmod command

 - there are three types of users who can interact with a file:
Owner — the user who creates and owns a file or folder.
Group — all users who are members of the same group.
Others — all other users on the system who are neither the owner nor members of a group.
- The three characters after the file type represent the owner’s file permissions. ( read (r), write (w), and execute (x) the file).
- Let’s say we want to change Linux file permissions from -rwxrw-rw- to -rwx-r–r–. Simply enter this line: `chmod 744 [file name]`
- The number determines the file permissions. Read, write, and execute are represented by a numerical value:
r (read) – 4
w (write) – 2
x (execute) – 1  

![image](https://user-images.githubusercontent.com/47173937/116520390-91ecaf80-a8ca-11eb-81d2-b6c17288c62d.png)  


 10. How to check permission for files/dir
 - File permission can be viewd by using `ls -l filename` command   
 11. How to use head, tail, sort, nl (number line), wc (word count)
 - ![image](https://user-images.githubusercontent.com/47173937/116520696-f6a80a00-a8ca-11eb-8915-8c107fcbba2e.png)
 - `tail [OPTION]... [FILE]...` example: `tail /var/log/messages`
 - `tail -n <number_of_lines> /path/to/file` example: `tail -n 4 /etc/group` 
 - `head /etc/passwd` by default prints first 10 lines
 - `head -n 20 /etc/passwd | tail -n 5` comibination of head and tail command. To print 15th line to 20th line in /etc/passwd file.  
 
 12. What is pipping and redirection, HINT > indicates to the command line
 - Redirection
 - Every single process in Linux has at least 3 communication channels available:
 - Standard Input – STDIN
 - Standard Output – STDOUT
 - Standard Error – STDERR
 - The following command would store the text you type between the ” ” in a file. If the file doesn’t exist, it will be created:
 - `echo "Test Message" > testmessage`
 - The next command would send an email with the contents of that file, so only the text, not the file itself, to the user Peter:
 - `mail -s "testmsg" peter < testmessage` 
 
 13. What is STDIN standard input and output
 - 

