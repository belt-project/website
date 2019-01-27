---
layout: default
---

# belt.sh

Tool belt for simple devops in bash.

<div class="alert alert-success">CURRENT VERSION &mdash; v0.0.1</div>

## Usage

Add the following line to the top of your script:

    source /dev/stdin <<< "$(curl -Lsm 2 https://git.io/fh6kT)"

Below is an example of using `belt.sh` and the `hello` **tool**.

    #!/usr/bin/env bash
    set -eo pipefail

    source /dev/stdin <<< "$(curl -Lsm 2 https://git.io/fh6kT)"

    hello "$(whoami)"

So what does sourcing the script do?

1. It will check if `/usr/local/lib/belt` exists, and if not it will clone the
   git repository down
1. Sources the main `belt.sh` script that makes a number of functions available
   for loading **tools**
