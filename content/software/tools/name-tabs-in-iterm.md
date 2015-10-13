+++
title = "How to set terminal title in Bash"
description = "Do you want to make your text readable?"
date = "2015-10-14T07:04:00+08:00"
menu = ["main", "software", "tools"]
articleTypes = ["tip"]
tags = ["bash", "terminal", "shell"]

+++

1. Put this code in your `~/.bashrc` or your own custom source file

```bash
function title {
    echo -ne "\033]0;"$*"\007"
}
```

2. Call the function from the bash prompt

```bash
title Awesome title!
```

[Source](http://superuser.com/questions/419775/with-bash-iterm2-how-to-name-tabs)
