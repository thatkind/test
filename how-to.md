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
> [Note]
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
```bash
echo $VARIABLE_NAME
```

### 2. Set within a shell script
```bash shell script
#!/bin/bash

VARIABLE_NAME=value
```

Use the variable in your script by adding a dollar sign at the beginning to referencing it.

```bash shell script
#!/bin/bash

VARIABLE_NAME=value

echo "My variable is now set to $VARIABLE_NAME"
```