/*
Title: apt-get VS aptitude
Description: 
Author: Sébastien Lucas
Date: 2011/02/07
Robots: noindex,nofollow
Language: en
Tags: debian
*/
# apt-get VS aptitude

## The fact
aptitude is newer and better than apt-get so it's simple : use aptitude.

## Under the change

aptitude by default install recommended packages. So if you want to have only what's necessary and nothing more 

 * Create a file in /etc/apt/apt.conf.d (in my case /etc/apt/apt.conf.d/20apt-nosuggested)
 * Add these line :

```
APT::Install-Recommends "0";
APT::Install-Suggests "0";
```





