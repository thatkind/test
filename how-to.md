---
title: Shell variables in Linux
description: How to work with shell variables in Linux
author: rallen
ms.topic: linux
ms.date: 03/26/2022
---

# How to work with shell variables in Linux

## Check your current environment variables

Login to your Linux server
```
ssh user@server
```

Check your current environment variables
```
env
```
> [!Note]
> Pay attention to variables which are already set.  They are set for a purpose.  You should generally leave them set to their default values and use unique variable names for your own needs.

## Two ways to set your own custom variables

### 1. Set from the command line
```bash
VARIABLE_NAME=value
```

Verify your variable is set
```bash
set | grep VARIABLE_NAME
```

Use your variable on the command line by adding a dollar sign at the beginning.

Example
```bash
print $VARIABLE_NAME
```

### 2. Set variable within a shell script
```bash shell script
#!/bin/bash

VARIABLE_NAME=value
```

To the variable in your script, you will also reference it by adding a dollar sign at the beginning.






# Setting environment variables in Linux (3 methods)

To check which shell your terminal session is set to use
```
env | grep SHELL
```




# Manual

x
# CLI

