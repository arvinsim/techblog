+++
title = "Using port 80 with Django's runserver command"
description = "Django's runserver could not normally run on port 80. But there is a way to circumvent it."
date = "2015-01-27T23:30:54+08:00"
article-type = ["tip"]
language = ["python"]
tags = ["python", "django", "runserver"]

+++

If you want to test your Django application on port 80, you would probably do something like this

    python manage.py runserver yourdomain.com:80

Unfortunately, this would not work. It would cause an error.

To force the usage of port 80, make sure you follow this steps

1. Make sure that no other application is using port 80. Examples of applications that do are local webservers like Apache and Tomcat. Here are some tips to check what programs are running on port 80 in [Windows](http://stackoverflow.com/questions/1960750/how-to-find-which-program-is-using-port-80-in-windows), [Linux](http://www.cyberciti.biz/faq/find-linux-what-running-on-port-80-command/) and [Mac](http://www.databasically.com/2011/06/02/mac-os-x-find-the-program-running-on-a-port/)

2. After verifying that there no other application is using port 80, run the command above as root

<!-- This comment is needed so that the command below will be shown in code form -->

    sudo python manage.py runserver yourdomain.com:80

*Important*: Only use this tip for testing purposes only.
