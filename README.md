***Simple Shell In C***

This is a simple shell which handles 10 commands, 5 internal and 5
external. This handles a simple command and at most two flags.

****INTERNAL COMMANDS****

1.  cd command:

> options : cd &lt;filename&gt;
>
> cd
>
> cd ..
>
> cd \~

cd –P &lt;filename&gt;

cd –L &lt;filename&gt;

> Error handling: 1). Invalid path prompt when directories are not
> available.
>
> 2). Invalid option prompt when wrong flag is entered.

1.  *echo command:*

> *options: echo &lt;string&gt;*

*echo –n &lt;string&gt;*

*echo –E &lt;string&gt;*

*Assumptions: Only supports –n,-E and simple echo commands.*

1.  history command:

> options : history
>
> history &lt;integer number&gt;
>
> history –c
>
> error handling: invalid command if invalid command is passed followed
> by history.
>
> Assumptions: Positive integers should be passed.

This command will print the entire history when the simple history
command is entered. Is history followed by an integer then last n
command will be printed. To clear the history you just need to type
history –c.

1.  pwd command :

> options: pwd
>
> pwd –P
>
> pwd – L
>
> Error handling: Invalid command if command passed is other than the
> given options.

It prints the current working directory.

1.  exit command:

> options: exit
>
> It will terminate the process and exit he shell.

****EXTERNAL COMMANDS****

1.   ls command:

> options: ls
>
> ls –m
>
> ls -1
>
> ls command prints the files and folders in the current working
> directory. The –m flag prints the separated with coma and the –1 flag
> print the files and folders one per line.
>
> 2 mkdir command:
>
> Options: mkdir &lt;directory name&gt; It creates new directory and
> give an error if not possible to make a directory.
>
> mkdir -v &lt;directoryname&gt; It creates a directory and give a
> message of successful completion and give and error if not possible.
>
> mkdir -m &lt;file mode&gt; &lt;directoryname&gt; It creates a file
> with the given mode in the command and give error if not possible
>
> 3 rm command:
>
> Options:

rm &lt;filename&gt; deletes the file and give error if not possible.

rm -i &lt;filename&gt; ask user before deleting the file and give an
error if not possible.

rm -r &lt;directoryname&gt; delete directory and give an error if not
possible

4.   Date command

> Options: date displays the date in IST formate
>
> date -R displays the date in gmt +0530

date –I dispalys the date in yyyy-mm-dd format

5.  *Cat command:*

> *Options:*
>
> *Cat &lt;filename&gt;*prints the content of the file.

cat -E &lt;filename&gt; display \$ at end of each line.

> *Cat –n &lt;filename&gt; displays number of the all lines of the file*
