# Shell Color Scripts

![Screenshot of shell-color-scripts](https://gitlab.com/dwt1/dotfiles/raw/master/.screenshots/dotfiles12.png)


# NOTE: THIS PROJECT IS ABANDONED
Use the original version instead [Gitlab](https://gitlab.com/dwt1/shell-color-scripts).

# About
This is a fork of DistroTube's Color Scripts on [Gitlab](https://gitlab.com/dwt1/shell-color-scripts).

This fork adds and removes color scripts based on my preferences

# Installing shell-color-scripts on Arch Linux

NOTE: This is the only distro that this is actually tested and used on.

What you need to do in order to install on Arch Linux:

Firstly, you need to git clone this repository:

```zsh
https://github.com/redkittty/shell-color-scripts.git
```

Secondly, you need to cd into the directory:

```zsh
cd shell-color-scripts
```

Finally run the pkgbuild:

```zsh
makepkg -si
```

Or, to do it in one command, do this:

```zsh
git clone https://github.com/redkittty/shell-color-scripts.git && cd shell-color-scripts && makepkg -si
```

# Installing shell-color-scripts on other Linux distributions

Download the source code from this repository or use a git clone:

    git clone https://gitlab.com/dwt1/shell-color-scripts.git
	cd shell-color-scripts
    sudo make install

    # Removal
    sudo make uninstall

    # optional for zsh completion
    sudo cp completions/_colorscript /usr/share/zsh/site-functions

    # optional for fish shell completion
    sudo cp completions/colorscript.fish /usr/share/fish/vendor_completions.d

# Usage

    colorscript --help
    Description: A collection of terminal color scripts.

    Usage: colorscript [OPTION] [SCRIPT NAME/INDEX]
    -h, --help, help        	Print this help.
    -l, --list, list        	List all installed color scripts.
    -r, --random, random    	Run a random color script.
    -e, --exec, exec        	Run a specified color script by SCRIPT NAME or INDEX.
    -a, --all, all          	List the outputs of all colorscripts with their SCRIPT NAME
    -b, --blacklist, blacklist	Blacklist a color script by SCRIPT NAME or INDEX.

# The Scripts Are Located in /opt/shell-color-scripts/colorscripts

The source for shell-color-scripts is placed in:

    /opt/shell-color-scripts/colorscripts

For even more fun, add the following line to your .bashrc or .zshrc and you will run a random color script each time you open a terminal:

    ### RANDOM COLOR SCRIPT ###
	colorscript random
