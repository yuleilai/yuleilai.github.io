---
layout: post
title:  "Install Fonts on Ubuntu"
date:   2014-12-09 19:43:10
categories: Ubuntu
---

### Fonts list

- DejaVuSansMono.ttf
- Monaco.ttf

### Install

```bash
$ sudo apt-get install curl
$ curl -kL https://raw.githubusercontent.com/yuleilai/fonts/master/install.sh
$ ./install.sh
```

or you can clone my github repository

```bash
$ git clone https://github.com/yuleilai/fonts.git
$ ./font/install.sh
```

### Bash shell

```bash
#!/bin/bash

echo "Start install"
sudo mkdir -p /usr/share/fonts/truetype/custom

echo "Downloading fonts"
wget -c https://raw.githubusercontent.com/yuleilai/fonts\
        /master/DejaVuSansMono.ttf 
wget -c https://raw.githubusercontent.com/yuleilai/fonts\
        /master/Monaco.ttf

echo "Installing fonts"
sudo mv *.ttf /usr/share/fonts/truetype/custom/

echo "Updating fonts cache"
sudo fc-cache -f -v

echo "Enjoy"
```

