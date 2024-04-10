# Lab Report 1

## `cd` command prompts


### *Without any Arguments*

```
samham@penguin:~/lecture1$ cd
samham@penguin:~/$
```

- The absolute path for this command prompt was `/home/samham/lecture1`.

- What the `cd` command does is change your directory, so when you have no directory stated after it, it just changes the directory to the user/home directory.

- This output is not an error as the command did what it needed to do.



### *With a directory*

```
samham@penguin:~/$ cd lecture1
samham@penguin:~/lecture1$
```

- The absolute path for this command prompt was `/home/samham`.

- This code changed the directory from `samham` to `lecture1`. This is due to a directory called `lecture1` being in `samham`.

- This output is not an error.



### *With a file*

```
samham@penguin:~/lecture1$ cd Hello.java
bash: cd: Hello.java: Not a directory
```

- The absolute path for this command prompt was `/home/samham/lecture1`.

- This code attempted to change the directory to a `Hello.java`, but it failed even though `Hello.java` is in `lecture1`

- This is an error because it doesn't do anything in the end and it comes with a message saying that `cd` doesn't work with `Hello.java` because it isn't a directory.



## `ls` command prompts


### *Without any Arguments*

```
samham@penguin:~/lecture1$ ls
Hello.class Hello.java messages README workspace.code-workspace
```

- The absolute path for this command prompt was `/home/samham/lecture1`.

- The `ls` command lists out the contents of whatever is used as its argument. In this case, since there was no argument, it defaulted to the current working directory, `lecture1`, and printed its contents out.

- This works properly and has no errors occuring.



### *With a directory*

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```

- The absolute path for this command prompt was `/home/samham`.

- Using the `ls` command in this case with a directory as an argument allows you to see the files and directories within it without having that directory as your working directory.

- This works properly and has no errors occuring.



### *With a file*

```
samham@penguin:~/lecture1$ ls Hello.java
Hello.java
```

- The absolute path for this command prompt was `/home/samham/lecture1`.

- Using the `ls` command with a file just prints out what you put as the argument, for example, if I put the entire path to the `Hello.java` file, it would just print out what I wrote.

- This works properly and has no errors occuring.



## `cat` command prompts


### *Without any Arguments*

```
samham@penguin:~/lecture1$ cat

```

- The absolute path for this command prompt was `/home/samham/lecture1`.

- When trying to use the `cat` command with no arguments, nothing is printed out.

- This is an error, though the terminal won't say that. Instead, it will wait for you to input something it recognizes, a file or a directory, forever unless you use `^C` to get out of the loop.



### *With a directory*

```
samham@penguin:~/$ cat lecture1
cat: lecture1: Is a directory
```

- The absolute path for this command prompt was `/home/samham`.

- Using `cat` with a directory as an argument ends up with the terminal printing an error message saying that `lecture1` is a directory.

- This results in an error as `cat` prints out the content of a file, and directories don't work with it as arguments.



### *With a file*

```
samham@penguin:~/lecture1$ cat messages/sv.txt
Hej världen! 
```

- The absolute path for this command prompt was `/home/samham/lecture1`.

- Using a file with `cat` will print out its contents, and in this case with `messages/sv.txt`, it prints out the greeting "Hello World!" in Swedish, which is "Hej världen!". In the case of a `.java` file, it would also print out the code within that file.

- This works properly and has no errors occuring.
