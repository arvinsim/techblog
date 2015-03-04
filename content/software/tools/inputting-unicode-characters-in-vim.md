+++
title = "Inputting Unicode characters in Vim"
description = "An easy way to insert Unicode characters in Vim"
date = "2015-03-04T11:43:46+08:00"
articleTypes = ["tip"]
menu = ["main", "software", "tools"]
tags = ["vim", "unicode", "encoding"]
+++

# Setup

We need to make sure that Vim encoding is set to UTF-8.

To check what encoding you are currently using, run this command

    set encoding?

If it outputs something like this

    encoding=utf-8

Then you are good to go.

Otherwise, set this option in your .vimrc file

    set encoding=utf-8

# Inserting unicode characters

After doing the setup above, you are now ready to enter unicode characters.

1. Enter Insert or Replace Mode
2. Press *Control + v*
3. Press *u*
4. Enter the unicode number of the character 


---

I learned about this tip while I was customizing my [Syntastic](https://github.com/scrooloose/syntastic) linter options. My goal was to use unicode characters for the error and warning markers in the gutter.

