# Project Title
#### WORKS ONLY WITH QTILE WM (but can be used as a starter for other wm)

This program helps you to have a better desktop in 1 second with an image .

## Getting Started


### Prerequisites

You'll need some depedencies:

```bash
# for arch and arch based distro
sudo pacman -S qtile #of course you'll need qtile
sudo pacman -S feh

# for debian/ubuntu
sudo apt-get install qtile
sudo apt-get install feh

pip install --user colorz #generate colors scheme based on an image
```

### Installing

```bash
git clone https://github.com/BenoitPingris/qtile-desktop-wallpaper
cd qtile-desktop-wallpaper
# You can run the script from here or...
mkdir ~/bin
mv desktop_theme $_

export PATH=$PATH:$HOME/bin
```

### Usage
```bash
desktop_theme ~/Images/wallpaper/landscape.jpg
```
The script will set the image as a background using feh and it will write the main color in a file, then YOU have to use the file in your scripts.
You can use the Color class in the [color_schemes.py]('google.fr')
```python
from color_schemes import Color

bg = Color()

widget1(background=bg.get_next_color()) # Each call of 
widget2(background=bg.get_next_color()) # get_next_color return
widget3(background=bg.get_next_color()) # a new color.
```

#### Screenshots:
![Image1](https://raw.githubusercontent.com/BenoitPingris/qtile-desktop-wallpaper/master/image1.png)
![Image1](https://raw.githubusercontent.com/BenoitPingris/qtile-desktop-wallpaper/master/image2.png)
![Image1](https://raw.githubusercontent.com/BenoitPingris/qtile-desktop-wallpaper/master/image3.png)

Link of my [qtile config](https://github.com/BenoitPingris/qtile-config)
##


## Built With

* [Qtile](http://www.qtile.org/) - A full-featured, hackable tiling window manager written and configured in Python
* [colorz](https://github.com/metakirby5/colorz) - A k-means color scheme generator.

* [feh](https://feh.finalrewind.org/) - a fast and light image viewer

## Authors

* **Benoit Pingris** - [BenoitPingris](https://github.com/BenoitPingris)
