---
layout: post
title:  "Copy a Website"
date:   2015-08-25 3:00:18
categories: web
---
**Do you want to save a webpage or a website on your computer ??**

The best tools availabe there are 'wget' and 'httrack'

we will talk about *wget*

<br>
**Wget**

GNU Wget is a free software package for retrieving files using HTTP, HTTPS and FTP, the most widely-used Internet protocols.

<br>
simply you can type the follwoing to get the file on the local drive
```
wget http://url
```

There's the `--recursive` parameter. It will download everything, sometimes more that what you want.
```
wget --recursive http://url
```

To filter for specific file extensions:

```
wget -A pdf,jpg -m -p -E -k -K -np http://url/path/
```

Or, if you prefer long option names:

```
wget --accept pdf,jpg --mirror --progress --adjust-extension --convert-links --backup-converted --no-parent http://url/path/
```

You can download a Full Website Using `wget --mirror`

```
wget --mirror -p --convert-links -P ./LOCAL-DIR WEBSITE-URL
```

>Options:
>
>`--mirror` turns on options suitable for mirroring.<br>
>`-p` downloads all files that are necessary to properly display a given HTML page.<br>
>`--convert-links` after the download, convert the links in document for local viewing.<br>
>`-P ./LOCAL-DIR` saves all the files and directories to the specified directory.

<br>
**Further Reading**

[GNU Wget 1.16.2 Manual](http://www.gnu.org/software/wget/manual/wget.html)

[15 Awesome Wget Examples](http://www.thegeekstuff.com/2009/09/the-ultimate-wget-download-guide-with-15-awesome-examples/)

[Overview About Wget Command](http://tech.queryhome.com/54364/overview-about-wget-command)

[Ubuntu Manuals Wget](http://manpages.ubuntu.com/manpages/vivid/en/man1/wget.1.html)