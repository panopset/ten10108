

# Linux Mint Development PC Preparation

## Prerequisites

    sudo apt install vim git nginx
   
You should have an open JVM installed with Linux Mint, if you don't, [install](https://openjdk.java.net/) it.

* [panopset.jar](https://panopset.com/download) in your home directory.

## Environment Variables

    vim ~/.bashrc

Add the following lines:

    # Environment variables required for ten10108 developers:
    export HTTP_HOME=/var/www/html
    export T8_USER=$USER
    export T8_DOMAIN=ten10108.com
    export T8_SERVER=prod

exit and launch another terminal window.

## Git

You've probably already done this, but if you are on a brand new machine, [enter](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) the following commands:

    git config --global user.name="<your full name>"
    git config --global user.email=<your email address>

... replacing everything within and including the <> brackets.



## Update docs

This step also generates your initial nginx server block file in the temp directory, which won't
work unless you have properly set up the environment variables above.

    ./dd.sh

