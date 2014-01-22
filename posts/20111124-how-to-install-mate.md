.. link: 
.. description: 
.. tags: MATE,Debian,Ubuntu,Linux Mint
.. date: 2011/11/24 13:17:00
.. title: How to install MATE in Debian, Ubuntu and Linux Mint
.. slug: 2011-11-24-how-to-install-mate-in-debian-ubuntu-and-linux-mint
.. author: Stefano Karapetsas

To install experimental MATE packages, add the following line to your /etc/apt/sources.list file.

For Debian Wheezy/Sid and Linux Mint LMDE:

```
deb http://tridex.net/repo/debian/ sid main
```

For Ubuntu Oneiric and Linux Mint Lisa:

```
deb http://tridex.net/repo/ubuntu/ oneiric main
```

Once updated apt, type in a terminal:

```
sudo apt-get install mate-core
```
