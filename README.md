# Shell Color Scripts

![Screenshot of shell-color-scripts](https://gitlab.com/dwt1/dotfiles/raw/master/.screenshots/dotfiles12.png)

A collection of terminal color scripts DistroTube accumulated over the years.
Included 52 beautiful terminal color scripts.

This is a fork that removes (and maybe might add more) color scripts

# Installing shell-color-scripts on Arch Linux

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

# Installing shell-color-scripts on other Linux distributions

Download the source code from this repository or use a git clone:

	```zsh
    git clone https://gitlab.com/dwt1/shell-color-scripts.git
	cd shell-color-scripts
    sudo make install

    # Removal
    sudo make uninstall

    # optional for zsh completion
    sudo cp completions/_colorscript /usr/share/zsh/site-functions

    # optional for fish shell completion
    sudo cp completions/colorscript.fish /usr/share/fish/vendor_completions.d
    ```

# Usage

    ```zsh
    colorscript --help
    Description: A collection of terminal color scripts.

    Usage: colorscript [OPTION] [SCRIPT NAME/INDEX]
    -h, --help, help        	Print this help.
    -l, --list, list        	List all installed color scripts.
    -r, --random, random    	Run a random color script.
    -e, --exec, exec        	Run a specified color script by SCRIPT NAME or INDEX.
    -a, --all, all          	List the outputs of all colorscripts with their SCRIPT NAME
    -b, --blacklist, blacklist	Blacklist a color script by SCRIPT NAME or INDEX.
    ```

# The Scripts Are Located in /opt/shell-color-scripts/colorscripts

The source for shell-color-scripts is placed in:

	```zsh
    /opt/shell-color-scripts/colorscripts
    ```

For even more fun, add the following line to your .bashrc or .zshrc and you will run a random color script each time you open a terminal:

	```zsh
    ### RANDOM COLOR SCRIPT ###
	colorscript random
    ```
