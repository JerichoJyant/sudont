# sudont
**DON'T install this on your system, or anyone elses, under any circumstances.**

`sudont` allows you to run any command as root, using a pre-saved password. The name is a play on
the traditional `sudo` command.

# Usage
```
sudont [command requiring root privileges]
```

You will be playfully insulted, your password will be displayed in plaintext, and then your command will run as root.

# `sudo` vs `sudont`
## sudo -- the built in, sane way
Some linux terminal commands can not be run without `root` privileges. In order to run them without having to switch users, the `sudo` command can be placed before the command in question. `sudo` prompts the user for their password, and then grants them access. For example, to do a software update as a typical user, running `apt upgrade` will not work. `sudo apt upgrade` will.

## sudont -- the insane way
Instead of typing, for example, `sudo apt upgrade` and having to enter your password, you can type `sudont apt upgrade` and your password will be given to sudo, allowing you to do whatever you want without the hassle of basic linux security.

# Why did you make this?
Two software engineers were joking around, and one of them made this pun. They joked about what the new command would do. This script is the result of that conversation. 

Su-"do"? No, su-"**don't**". **Don't** ask for my password. **Don't** install this (**Seriously**).

This is all for fun and practice writing bash scripts! However, it works as advertised, so be careful!

# Installation
*See LICENSE file for full disclaimer and terms of use. More warnings are in the script's comments.*

Edit the `sudont` script and change the password variable to yours. Make it executable. Put it in your path. Say goodbye to your computer's security.

# How it works
`sudont` is a bash script shell around `sudo`. The script sends your pre-saved password into sudo through standard input, then sudo behaves as if you had typed the password.