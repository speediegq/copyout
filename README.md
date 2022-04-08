# copyout
Dmenu script which copies the output of a command WITHOUT the use of a terminal.

## Preview
You can see a [Video Preview](https://youtu.be/txgUKwvHeZ4) [here](https://youtu.be/txgUKwvHeZ4).

## Usage
Install the script (see installation) and run it using dmenu. Make sure to edit the config file to match your system.

## Installation
Download the [script](https://raw.githubusercontent.com/speediegamer/copyout/main/copyout) and save it to /usr/bin, /usr/local/bin, or any other path specified in your shell's $PATH variable. Then chmod +x it to make sure it's executable.

If /bin/sh isn't an alias then edit the script and change #!/bin/sh to a shell on your Linux system.

## Notes
- This script IS fully POSIX compliant.
- This script has dmenu as a dependency
- Rofi support might become a patch later on.

## Configuration
Create ~/.config/copyout and open copyoutrc in Vim. Now change these variables to what's present on your system:
- COPYOUT_BIN_DIR=/usr/bin # Only change this if your binary directory isn't /usr/bin (such as NixOS)
- COPYOUT_DOTDIR=~/.config/copyout # The directory where dotfiles for copyout are located. Probably don't change.
- COPYOUT_DMENU=/usr/bin/dmenu # Set this to the path where your dmenu binary is.
- COPYOUT_HISTORY_FILE=~/.config/zsh/dotfiles/history # Set this to the path to your HISTORY file. (Example: ~/.bash_history for bash)
- COPYOUT_SHELL="/bin/sh -c" # No need to change if /bin/sh is an alias.
- COPYOUT_CLIPBOARD_COMMAND="xclip -selection clipboard" # No need to change unless you won't be using xclip.

## Credits
- Me
- The awesome people who have contributed

## Have issues?
Report any issues to the GitHub page Issues.

## License
This dmenu script is licensed under MIT.
See the "about" or LICENSE file for more information.
