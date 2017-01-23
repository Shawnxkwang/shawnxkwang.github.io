---
layout: post
title: How to Compress and Extract Files Using the tar Command on Linux
---


## Compress

`tar -czvf name-of-archive.tar.gz /path/to/directory-or-file`

Here’s what those switches actually mean:

`-c`: Create an archive.

`-z`: Compress the archive with gzip.

`-v`: Display progress in the terminal while creating the archive, also known as “verbose” mode. The v is always optional in these commands, but it’s helpful.

`-f`: Allows you to specify the filename of the archive.


## Extract

`tar -xzvf archive.tar.gz`

use `-C` to extract to a specific directory,

`tar -xzvf archive.tar.gz -C /etc`
