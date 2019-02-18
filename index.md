---
layout: default
---

# belt.sh

The tool belt for simple devops in bash.

## Usage

Add the following line to the top of your script:

    source /dev/stdin <<< "$(curl -Lsm 2 https://get.belt.sh)"

So what does sourcing the script do?

1. It will check if `/usr/local/lib/belt` exists, and if not it will clone the
   git repository down
1. Sources the main `belt.sh` script that makes a number of functions available
   for loading **tools**

<div class="alert alert-warning">belt.sh is currently under active development</div>
