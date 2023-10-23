---
title: OverTheWire Bandit Level 0 Walkthrough
excerpt: This is my post description
date: 2023-10-22 20:00:00 +0000
categories: [OverTheWire, Bandit]
tags: [network, ssh, wargames, linux]
image:
    path: https://overthewire.org/img/domokitten.png
    alt: Image from https://overthewire.org
---

[Banit Level 0](https://overthewire.org/wargames/bandit/bandit0.html) <br><br>

## Level 0 Goal

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

## Walkthrough

This level is rather straightforward, my dear friends. Simply employ *ssh* to establish a connection with bandit.labs.overthewire.org, using port 2220. The command takes on the following appearance:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
If you're prompted for a password, do make use of the one specified in the Level Goal. It should look like this:
![OTWLevel0](/assets/img/OTW-L0-1.png)

Now that we are in we can pivot to level 1.

[Bandit Level 0 → Level 1](https://overthewire.org/wargames/bandit/bandit1.html)

## Level 1 Goal

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Walkthrough

Once again, this is rather straightforward. Begin by employing the 'ls' command to peruse the contents of the directory, and then proceed to employ the 'cat' command to display the content of the 'readme' file, as follows
![OTWLevel1](/assets/img/OTW-L1-1.png)

**Solution: N---------------------------------L**