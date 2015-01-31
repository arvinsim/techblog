+++
title = "Reverting changes in Git"
description = "How to change files back to the latest commit in Git"
date = "2015-01-31T09:42:15+08:00"
article-type = ["tip"]
tags = ["git", "svn", "version-control"]
+++


## Unmodify changes 

To unmodify the changes in a modifed file

    git checkout -- [files]

If you pass files as arguments, it will change those files back to the latest commit. Any modification that you did after the latest commit would be lost. Use this with caution.

## Unmodify changes but save your current changes

On the other hand, if you want to change back to the latest commit copy but want to somehow save your current modifications

    git stash [message_name]

This will save your modifications to a file and revert your files back to the latest commit. Keep in mind that this applies to all files.

