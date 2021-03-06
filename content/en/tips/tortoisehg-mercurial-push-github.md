/*
Title: How to use Tortoisehg (mercurial GUI) to push on Github
Description: 
Author: Sébastien Lucas
Date: 2011/11/12
Robots: noindex,nofollow
Language: en
Tags: git,mercurial
*/
# How to use Tortoisehg (mercurial GUI) to push on Github

## Why ?
I like git when working with Linux but in my opinion git is clearly not ready on Windows. As on my job I work with Windows and at home I mainly work with Linux, so overtime I got used to Mercurial.

In addition, It was actually fun to connect both worlds.

## Install tortoisehg

[http://tortoisehg.bitbucket.org/](http://tortoisehg.bitbucket.org/)

## Convert your Github private to be usable with pageant

[How to convert a private key generated by ssh-keygen](/en/tips/convert-private-key-openssl)

## Install hg-git

It's the plugin that allow to make it work :

```
hg clone http://bitbucket.org/durin42/hg-git c:\work\hg-git
```

## Enable the hg-git plugin

Edit your Mercurial.ini (in C:\Users\`<YourName>`) to add this line

```
[extensions]
hggit = C:\work\hg-git\hggit
```

## Check

Check that both Pageant and your private key are loaded

## Pull & Push

You can now try to pull a Github repository with this URL :

```
git+ssh://git@github.com/your-github-username/your-repo-name.git
```

Enjoy !

## Edit

In case of problem you can read [Error on cloning a Github repository with Mercurial](/en/tips/mercurial-github-error) to avoid wasting too much time.
