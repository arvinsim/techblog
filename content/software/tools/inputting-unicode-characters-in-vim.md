+++
date = "2015-03-04T11:43:46+08:00"
draft = true
title = "inputting unicode characters in vim"
+++

While I was looking to customize my [syntastic] linting options, I learned that you can actually put unicode characters in the gutter as indicators of errors and warnings.

# Setup

Make sure that you set your Vim encoding to UTF-8.

To check what encoding you are currently using, run this command

    set encoding?

If it outputs something like this

    encoding=utf-8

Then you are good to go.

Otherwise, enter this in your .vimrc file

    set encoding=utf-8

# Inserting unicode characters

This is how you do it

1. Enter Insert or Replace Mode
2. Press Control + v
3. Press u
4. Enter the unicode number of the character 
