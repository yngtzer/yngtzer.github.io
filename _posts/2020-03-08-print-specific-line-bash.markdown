---
layout: post
title: "Print specific line using Bash"
date: 2020-02-23  23:22:00 +0800
categories: Bash
---

# Given a file named index.txt, with 10 lines, output line 8 content

## Soln 1: Using sed
```
sed -n 8p index.txt
```

## Soln 2: Using awk
```
awk 'NR==8' file.txt
```