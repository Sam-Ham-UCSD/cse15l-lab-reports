# Lab Report 1


## `cd` command prompts
---

*Without any Arguments*
---
![cd with no args](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cd%20command%20with%20no%20args.JPG)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- What the `cd` command does is change your directory, so when you have no directory stated after it, it just changes the directory to the user/home directory.

- This output is not an error as the command did what it needed to do.


*With a directory*
---
![cd with directory](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cd%20command%20with%20directory%20as%20arg.JPG)

- The absolute path for this command prompt was `/home/samham`.

- This code changed the directory from `samham` to `lecture1`. This is due to a directory called `lecture1` being in `samham`.

- This output is not an error.


*With a file*
---
![cd with file](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cd%20with%20Hello.java%20as%20arg.JPG)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- This code attempted to change the directory to a `Hello.java`, but it failed even though `Hello.java` is in `lecture1`

- This is an error because it doesn't do anything in the end and it comes with a message saying that `cd` doesn't work with `Hello.java` because it isn't a directory.


## `ls` command prompts
---

*Without any Arguments*
---
![ls without args](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/ls%20command%20with%20no%20args.JPG)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- The `ls` command lists out the contents of whatever is used as its argument. In this case, since there was no argument, it defaulted to the current working directory, `lecture1`, and printed its contents out.

- This works properly and has no errors occuring.


*With a directory*
---
![ls with directory](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/ls%20command%20with%20directory%20as%20arg.JPG)

- The absolute path for this command prompt was `/home/samham`.

- Using the `ls` command in this case with a directory as an argument allows you to see the files and directories within it without having that directory as your working directory.

- This works properly and has no errors occuring.

*With a file*
---
![ls with file](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/ls%20command%20with%20Hello.java%20as%20arg.JPG)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- Using the `ls` command with a file just prints out what you put as the argument, for example, if I put the entire path to the `Hello.java` file, it would just print out what I wrote.

- This works properly and has no errors occuring.

## `cat` command prompts
---

*Without any Arguments*
---
![cat without args](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cat%20command%20with%20no%20args1.JPG)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- When trying to use the `cat` command with no arguments, nothing is printed out.

- This is an error, though the terminal won't say that. Instead, it will wait for you to input something it recognizes, a file or a directory, forever unless you use `^C` to get out of the loop.

*With a directory*
---
![cat with directory](https://sam-ham-ucsd.github.io/cse15l-lab-reports/cat%20command%20with%20directory%20command.JPG)

- The absolute path for this command prompt was `/home/samham`.

- Using `cat` with a directory as an argument ends up with the terminal printing an error message saying that `lecture1` is a directory.

- This results in an error as `cat` prints out the content of a file, and directories don't work with it as arguments.

*With a file*
---
![cat with file](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cat%20command%20with%20file%20as%20arg.JPG)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- Using a file with `cat` will print out its contents, and in this case with `messages/sv.txt`, it prints out the greeting "Hello World!" in Swedish, which is "Hej världen!". In the case of a `.java` file, it would also print out the code within that file.

- This works properly and has no errors occuring.
