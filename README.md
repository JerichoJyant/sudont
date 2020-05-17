# sudont
**DON'T install this on your system, or anyone elses, under any circumstances.**

Sudon't is sudo with jokes and without passwords!

## Usage
```
sudont [command requiring root privileges]
```

You will be insulted, your password will be printed, and then your command will run as root.

## sudo vs sudont
### sudo -- the built in, sane way
Some linux commands are dangerous and require special permission to run. To run these commands without switching to the all-powerful `root` account, put `sudo` in front of them. `sudo` prompts the user for their password before granting access.

For example, running `apt upgrade` as a regular user will not work. `sudo apt upgrade` will.

### sudont -- the insane way
Instead of typing, for example, `sudo apt upgrade` and having to enter your password, you can type `sudont apt upgrade`. No password required!

## Why did you make this?
Two software engineers were joking around about linux, and one of them made a pun. They joked about what the new command would do. This script is the result of that conversation. 

Su-"do"? No, su-"**don't**". **Don't** ask for my password. **Don't** install this.

This is all for fun and practice writing bash scripts! However, it works as advertised, so don't actually use it!

## Installation
*See LICENSE file for full disclaimer and terms of use. More warnings are in the script's source code.*

Edit the `sudont` script and change the password variable to yours. Make it executable. Put it in your path. Say goodbye to your computer's security.

*Note:* You may safely use this script as long as you don't configure it with your password. It won't work, but you will be able to see the randomly chosen insults! You can also use it in a throwaway VM install if the VM is safely and securely sandboxed.

## How it works
`sudont` is a simple shell around `sudo`. The script pipes your pre-saved password into sudo through standard input and then sudo runs as usual. It's not a hacking tool and only has your password if you put it in the script source code yourself.

## Contributing
Feel free to suggest more jokes! (see jokes.txt). Please keep them lighthearted and somewhat professional.