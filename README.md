# dotfiles
## Managing
These dotfiles are managed with [GNU Stow](http://www.gnu.org/software/stow/), a free, portable, lightweight symlink farm manager.
Stow is available for all Linux and most other UNIX like distributions via your package manager.

- `sudo pacman -S stow`
- `sudo apt-get install stow`
- `brew install stow`

You can also clone it [from source](https://savannah.gnu.org/git/?group=stow) and [build it](http://git.savannah.gnu.org/cgit/stow.git/tree/INSTALL) yourself.

## Installing

By default the stow command will create symlinks for files in the parent directory of the working directory.
So clone this repository inside your home directory (to `~/dotfiles`) and execute all stow commands from that folder.

To install the configuration for some software execute the stow command with the folder name as the only argument.

Thus, to install my **git** configuration use the command:

    stow git

To uninstall the configuration use:

    stow -D git
