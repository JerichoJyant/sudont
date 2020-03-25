# sudont
**DO NOT install this on your system, or anyone elses, under any circumstances**

# RISK AND DANGER
This is not some easy shortcut to always having root. By installing and configuring this, you are leaving your system vulnerable to anyone who knows you have `sudont` installed.

# Usage
## sudo
Some linux terminal commands can not be run without `root` privileges. In order to run them without having to switch users, the `sudo` command can be placed before the command in question. `sudo` prompts the user for their password, and then grants them access. For example, to do a software update as a typical user, running `apt upgrade` will not work. `sudo apt upgrade` will.

## sudont
```
sudont [command requiring root privileges]
```

Instead of typing, for example, `sudo apt upgrade` and having to enter your password, you can type `sudont apt upgrade` and your password will be given to sudo, allowing you to do whatever you want without the hassle of basic linux security

# Why did you build a hacking tool!?
This is not a hacking tool. To install and configure `sudont`, you need to already have your password. In basic terms, if a hacker can install `sudont`, you're already completely compromised. In fact, it's useless to a hacker. The only way this would help a hacker is if you foolishly ignored our warnings, installed it, and they knew you had it on your system.

# So why did you make it?
We thought it was funny. Su-"do"? No, su-"**don't**". **Don't** ask for my password. **Don't** install this (**Seriously**).

# Installation
Edit the `sudont` script and change the password variable to yours. Make it executable. Put it in your path. Say goodbye to your computer's security.