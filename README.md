# Jazz
Dots for a lowkey, aesthetic Kali Linux setup with KDE Plasma.

---
## A word regarding compatibility
Kitty terminals like the one meant for this setup sometimes don't come with the necessary prerequisites to utilize certain services (like RDP)
If you find an error like this, try to utilize another terminal emulator or install the missing dependencies.

---
## Installation
We do not have an install.sh script (yet) however you will often find indication to install each components rice

### About changing Kali's default Gnome to KDE Plasma:
It's a great choice for a more pleasing desktop enviroment, and it can be done quite easily:

``` url
https://www.kali.org/docs/general-use/switching-desktop-environments/
```

Pokemon-Colorscripts also requires a manual installation on Debian-based distros:

``` url
https://gitlab.com/phoneybadger/pokemon-colorscripts
```
### Changing you shell to ZSH
ZSH is a much more flexible and overall customizable shell than Bash, here's how you can use it in Kali KDE:

``` bash
sudo apt update
sudo apt install zsh
chsh -s $(which zsh)
```

Then you will need to log out and back into your account.
You can see if your shell was changed using

``` bash
echo $SHELL
```

You should see the directory of ZSH, not bash.

### Setting up the default kitty theme
Copy:

``` bash
https://raw.githubusercontent.com/XoanOuteiro/KittyConfig/refs/heads/main/kitty.conf
```
(A slightly modified version of Catpuccin Mocha Theme)

And paste into
``` bash
nano ~/.config/kitty/kitty.conf
```
