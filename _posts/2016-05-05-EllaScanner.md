---
layout: post
title: "EllaScanner - Passive web scanner"
---

EllaScanner is a simple passive web scanner. Using this tool you can simply check your site's security state.

{% highlight bash %}
./Start.py
Usage:
	./Start.py https:// or http://
{% endhighlight %}

Scanning of the site consists several phases:<br>
At first phase, you can get recommendations related to http/https headers.

{% highlight bash %}
./Start.py https://secrary.com

          ___           ___       ___       ___
         /  /\         /  /\     /  /\     /  /\
        /  /::\       /  /:/    /  /:/    /  /::\
       /  /:/\:\     /  /:/    /  /:/    /  /:/\:\
      /  /::\ \:\   /  /:/    /  /:/    /  /::\ \:\
     /__/:/\:\ \:\ /__/:/    /__/:/    /__/:/\:\_\:\
     \  \:\ \:\_\/ \  \:\    \  \:\    \__\/  \:\/:/
      \  \:\ \:\    \  \:\    \  \:\        \__\::/
       \  \:\_\/     \  \:\    \  \:\       /  /:/ passive
        \  \:\        \  \:\    \  \:\     /__/:/ scanner
         \__\/         \__\/     \__\/     \__\/ v0.1

    
[-]Do you want to get recommendations related to http/https headers? (y/[n]) 
{% endhighlight %}

![ellascanner_headers](https://i.imgur.com/4Cgi18z.png)

The Second phase depends on information gather in the first phase, you can get CVEs related to server's version.

![cve](https://i.imgur.com/ik7Mv03.png)

After this, the scanner uses sucuri.net and prints information about defaces, malicious codes, etc.

![sucuri](https://i.imgur.com/GZos7L7.png)

![deface](https://i.imgur.com/GDQLXEF.png)

And last but not least, if the site is Georgian you can get information from checknet.ge about site's historical states.

![checkent](https://i.imgur.com/8t7q6Hy.png)

![checknet](https://i.imgur.com/TtgwLKh.png)

**Requirements:**<br>
Ubuntu 16.04 x64 (or any ubuntu version)<br>
Python<br>
[Download](https://github.com/secrary/EllaScanner)
