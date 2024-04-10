# Lab Report 1


## `cd` command prompts
---

*Without any Arguments*
---
![cd without args](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cd%20command%20with%20no%20args.png)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- What the `cd` command does is change your directory, so when you have no directory stated after it, it just changes the directory to the user/home directory.

- This output is not an error as the command did what it needed to do.


*With a directory*
---
![cd with directory](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cd%20command%20with%20directory%20as%20arg.png)

- The absolute path for this command prompt was `/home/samham`.

- This code changed the directory from `samham` to `lecture1`. This is due to a directory called `lecture1` being in `samham`.

- This output is not an error.


*With a file*
---
![cd with file](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cd%20with%20Hello.java%20as%20arg.png)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- This code attempted to change the directory to a `Hello.java`, but it failed even though `Hello.java` is in `lecture1`

- This is an error because it doesn't do anything in the end and it comes with a message saying that `cd` doesn't work with `Hello.java` because it isn't a directory.


## `ls` command prompts
---

*Without any Arguments*
---
![ls without args](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/ls%20command%20with%20no%20args.png)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- The `ls` command lists out the contents of whatever is used as its argument. In this case, since there was no argument, it defaulted to the current working directory, `lecture1`, and printed its contents out.

- This works properly and has no errors occuring.


*With a directory*
---
![ls with directory](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/ls%20command%20with%20directory%20as%20arg.png)

- The absolute path for this command prompt was `/home/samham`.

- hello

- This works properly and has no errors occuring.

*With a file*
---
![ls with file](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/ls%20command%20with%20Hello.java%20as%20arg.png)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- hello

- This works properly and has no errors occuring.

## `cat` command prompts
---

*Without any Arguments*
---
![cat without args](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cat%20command%20with%20no%20args1.png)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- hello

- hello

*With a directory*
---
![cat with directory](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cat%20command%20with%20directory%20command.png)

- The absolute path for this command prompt was `/home/samham`.

- hello

- This works properly and has no errors occuring.

*With a file*
---
![cat with file](https://github.com/Sam-Ham-UCSD/cse15l-lab-reports/blob/main/cat%20command%20with%20file%20as%20arg.png)

- The absolute path for this command prompt was `/home/samham/lecture1`.

- hello

- hello
