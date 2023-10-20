---
title: Writing Python Scripts
teaching: 15
exercises: 0
---

::::::::::::::::::::::::::::::::::::::: objectives

- Write Python commands in to a file
- Execute the file as a program

::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::::::::::::::::::::::::::::::: questions

- How can I write and save complete Python programs?

::::::::::::::::::::::::::::::::::::::::::::::::::

Up until now we have been using the IPython interpreter to get to
grips with the basic use of Python. From now on, we will be focusing
on saving our code in to scripts and running them from the shell by
executing the `python` program with our script as an argument.

:::::::::::::::::::::::::::::::::::::::::  callout

## Switching to Shell Commands

In this lesson we are switching from typing commands in a Python interpreter to typing
commands in a shell terminal window (such as bash). When you see a `$` in front of a
command that tells you to run that command in the shell rather than the Python interpreter.

::::::::::::::::::::::::::::::::::::::::::::::::::

## Writing Your First Script

A script in python is almost exactly the same as a Shell script you’ve
already met, i.e. it is a plain text file that contains lines of
Python code that will be executed one after another.

To create and edit a Python script, it is almost essential to use a
text editor with syntax highlighting. For this course, we recommend
using VSCode as provided by Microsoft. It’s easily installed on
Windows either directly or through Anaconda and macOS users can
install and run it through Anaconda as well.

:::::::::::::::::::::::::::::::::::::::::  callout

## Choosing a Good Text Editor

When we write Python scripts, it is essential that it is written in **plain** text - this means
you can't use a Word Processor program like MS Word as it will add quite a bit of other information
to the created file that Python won't understand.
You also want to use an editor that knows about the programming language
you're using as then it can highlight different parts of the code, help with formatting and
show any syntax errors. There are many options out there but possible ones are:

* Visual Studio Code
* Spyder
* Notepad++
* PyCharm
* Emacs
* Vim

::::::::::::::::::::::::::::::::::::::::::::::::::

To write our first script then, start up your text editor, 
select 'New File' and create a new file called
`~/Desktop/swc-python/hello.py`. After this has been created and opened, type the following
and save it:

```python
print("Hello World")
```

As you can see, we have used the .py extension as this makes it easier to identify Python scripts from other file types.

From your shell prompt that you were running IPython in, make sure you are in the correct folder:

```bash
$ cd ~/Desktop/swc-python/
```

and then type:

```bash
$ python hello.py
```

Hopefully you should see what you would expect:

```output
Hello World
```

Congratulations! You’ve created your first Python script! Going forward in this course, we recommend writing the code in scripts and executing from the shell prompt just like this. You can continue to use the IPython interpreter if you’d prefer but as things increase in complexity, it will become harder to avoid typing errors, etc.

## Documenting your Code

Now we are starting to store code, we must start documenting it as
well. This is critical, not only for other users of your code but also
yourself who may come back to some code at a later date and not easily
remember what it did or how. This is where comments become essential
--- these are bits of human readable text, denoted by `#`, that Python
will ignore but can be used to explain the meaning behind certain bits
of code. Try changing the your `hello.py` file to the following:

```python
# A simple test to check everything's working
print("Hello World")
```

If you run this, you will see the same as before but now you've added some information about what
you were trying to achieve!

:::::::::::::::::::::::::::::::::::::::::  callout

## It's Not All About Comments

You shouldn't use comments as an excuse for poor variable names or
code structure/formatting.  Your code should be fairly readable
without comments. They should help with clarifications and overall
aims of a particular piece of code.

::::::::::::::::::::::::::::::::::::::::::::::::::


:::::::::::::::::::::::::::::::::::::::: keypoints

- Python commands can be written and stored in a plain text file
- This file can then be run by using the `python <scriptname>`
- Python scripts generally use the `.py` extension
- You should try to use a syntax-highlighting text editor to edit your Python scripts
- Use comments to improve the readability of your code and aid understanding for both other people and yourself in the future

::::::::::::::::::::::::::::::::::::::::::::::::::


