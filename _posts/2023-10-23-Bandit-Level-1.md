---
title: OverTheWire Bandit Level 1 Walkthrough
excerpt: In this article, I shall guide you through Level 1 of OverTheWire Bandit ...
date: 2023-10-23 13:00:00 +0000
categories: [OverTheWire, Bandit]
tags: [network, ssh, wargames, linux]
image:
    path: https://overthewire.org/img/domokitten.png
    alt: Image from https://overthewire.org
---

[Banit Level 1](https://overthewire.org/wargames/bandit/bandit1.html) <br><br>

## Level 1 Goal

The password for the next level is stored in a file called - located in the home directory

## Walkthrough

To commence, establish a connection to the server by utilizing the *ssh* command and the previously provided password as follows:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

The subsequent step involves seeking out files. Once more, employ the *ls* command for this purpose:
![OTWLvl2](/assets/img/OTW-L2-1.png)

Ah, splendid! We've located the file. Yet, you can't merely open it using *cat*. Here's the clever trick: utilize './' to open that file.

```bash
cat ./-
```

**Solution: r---------------------------------i**

