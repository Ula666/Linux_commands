# Linux Commands and Practices:


### how to check Hidden Files and Directories: `ls -a`, `dir -a` a - all
### The Manual, Flags `man` Shows manual pages for Linux commands.
### what is a wildecards and How to use Wildcards: 
- Wildcards (also referred to as meta characters) are symbols or special characters that represent other characters. You can use them with any command such as ls command or rm command to list or remove files matching a given criteria, receptively.
- An asterisk (*) – matches one or more occurrences of any character, including no character.
- Question mark (?) – represents or matches a single occurrence of any character.
- Bracketed characters ([ ]) – matches any occurrence of character enclosed in the square brackets. It is possible to use different types of characters (alphanumeric characters): numbers, letters, other special characters etc.  

### how can you do Process Management
- `ps` To display your currently active processes
- `ps aux` To see an incredibly detailed list of processes (a - all users, u - shows the user/owner, x - displays processes not executed in the terminal)  

### What is Currently Running on your system `ps`
### Killing a process/Crashed Process `ps aux | grep chrome` 
### how to check any process running in Foreground and Background Jobs:
- `sleep 10000` - example of the foreground process. This is just a simple sleep command that will return the prompt to the user only after it is completed.  
- Background process runs your process in the background and will not take control of your terminal prompt. You can start a session and you are free to use your terminal. To submit a command as a background process you have to add & symbol at the end of the command. `sleep 50000 &`  
- `jobs -l` - To get the list of jobs either in running or stopped state  

### how to stop/kill any process running in Foreground and Background Jobs
- `sudo pkill name` - is one of the commands that can directly kill a background process, using the process name.

### How to change permissions with chmod command
### how to check permission for files/dir
### what does 777, 400, 600, r,w,x
### how to use head, tail, sort, nl (number line), wc (word count)
### what is pipping and redirection, HINT > indicates to the command line
### what is STDIN standard input and output


