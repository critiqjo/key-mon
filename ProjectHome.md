# Keyboard Status Monitor (key-mon) #



Utility to show live keyboard and mouse status for teaching and screencasts.

![http://key-mon.googlecode.com/hg/docs/screenshot-blank.png](http://key-mon.googlecode.com/hg/docs/screenshot-blank.png)

![http://key-mon.googlecode.com/hg/docs/screenshot.png](http://key-mon.googlecode.com/hg/docs/screenshot.png)

--theme=apple, cool new theme.

![http://key-mon.googlecode.com/hg/docs/screenshot-apple.png](http://key-mon.googlecode.com/hg/docs/screenshot-apple.png)

--smaller parameter:

![http://key-mon.googlecode.com/hg/docs/screenshot-smaller.png](http://key-mon.googlecode.com/hg/docs/screenshot-smaller.png)

--larger parameter:

![http://key-mon.googlecode.com/hg/docs/screenshot-larger.png](http://key-mon.googlecode.com/hg/docs/screenshot-larger.png)

--scale=2.0, and --meta parameter (for 'Windows' key), and mouse turned off through menu.

![http://key-mon.googlecode.com/hg/docs/2x-no-mouse-meta.png](http://key-mon.googlecode.com/hg/docs/2x-no-mouse-meta.png)

You can show multiple presses (here up to 2) by using --old-keys.  Here I pressed 'Y', 'Y', 'P', which means something in vi.

--nomouse --old-keys 2:

![http://key-mon.googlecode.com/hg/docs/old-keys-2.png](http://key-mon.googlecode.com/hg/docs/old-keys-2.png)

--sticky

Support for sticky keys

--only\_combo

Show only combination keys like Ctrl-A



## Features: ##
  * The window and buttons are scalable to any size.
  * Different keyboard themes/styles supported, for example the Mac look.
  * Can start without a window border and semi transparent to take up less space and be less intrusive.
  * Right click provides an application menu.
  * Supports the META (aka Windows) key.
  * Supports the scroll wheel.
  * Supports all three mouse buttons.
  * Should support multiple mouses or keyboards.
  * Move the window by dragging from anywhere inside.
  * Swap the left and right mouse buttons for lefties.
  * Support for touch tablets.
  * Emulate middle click by clicking left and right mouse buttons.
  * When the dialog is smaller a different set of images are used for a better look.
  * Support for foreign keyboards.
  * Ability to make your own keyboard scancode maps, for when the defaults don't work.
  * Visible mouse click. Briefly show's a circle where you clicked.
  * Option to show only key combinations.
  * Support for accessibility feature, sticky keys
  * <h2><a href='http://key-mon.googlecode.com/hg/RELEASE.rst'>Release Notes</a></h2>

## Requirements: ##
  * Linux or equivalent.
  * GTK+
  * pyGtk 2.0 (python-gtk2)
  * XLib (python-xlib)
  * X.Org "record" module.
  * librsvg2-common library

## Distributions ##
  * Arch Linux (AUR): https://aur.archlinux.org/packages/key-mon/
  * Debian: <Scott knows for sure>
  * Fedora: <Ryan can fill in>
  * Linux Mint: http://community.linuxmint.com/software/view/key-mon
  * Mageia: http://mageia.madb.org/package/show/release/3/name/key-mon
  * Ubuntu: https://apps.ubuntu.com/cat/applications/key-mon/

## Installation: ##

From **zip**. Download the zip file and unzip into a directory.

```
unzip key-mon*.zip
cd key-mon*
sudo python setup.py install
```

From **deb** package.
```
sudo dpkg -i key-mon*.deb
```

Via **pip**.
```
% pip key-mon
```
or sometimes
```
% sudo pip key-mon
```

To run just type:
```
% key-mon
```

You can make the dialog --smaller or --larger.

Ex.
```
key-mon --smaller
```

Here's the help:

```
$ key-mon --help
Options:
  -h, --help            show this help message and exit
  -s, --smaller         Make the dialog 25% smaller than normal.
  -l, --larger          Make the dialog 25% larger than normal.
  -m, --meta            Show the meta (windows) key.
  --nomouse             Hide the mouse.
  --noshift             Hide the shift key.
  --noctrl              Hide the ctrl key.
  --noalt               Hide the alt key.
  --scale=SCALE         Scale the dialog. ex. 2.0 is 2 times larger, 0.5 is half the size.
  --kbdfile=KBD_FILE    Use this kbd filename instead running xmodmap.
  --swap                Swap the mouse buttons.
  --emulate-middle      When you press the left, and right mouse buttons at the same time, it displays as a middle mouse button click.
  -v, --version         Show version information and exit.
  -t THEME, --theme=THEME
                        The theme to use when drawing status images (ex. "-t apple").

  Developer Options:
    These options are for developers.

    -d, --debug         Output debugging information.
    --screenshot=SCREENSHOT
                        Create a "screenshot.png" and exit. Pass a comma separated list of keys to simulate (ex. "KEY_A,KEY_LEFTCTRL").
```

### Bugs/Features ###

  * If you found a bug please click [this link](http://code.google.com/p/key-mon/issues/entry?template=Defect%20report%20from%20user).
  * If you want to request a feature please click [this link](http://code.google.com/p/key-mon/issues/entry?template=Feature%20Request).
  * To see the list of outstanding bugs/feature requests [click here](http://code.google.com/p/key-mon/issues/).
  * Do you use key-mon, why don't you [add your name](http://code.google.com/p/key-mon/issues/entry?template=I%20Use%20Key-Mon) to the list of users?

### Thanks: ###

  * Original concept from from Daniel G. Taylor (from the program [key-status-monitor](http://programmer-art.org/projects/key-status-monitor)).
Daniel also contributed a lot of the pretty themes.
  * Original keyboard artwork by Jakub Steiner (jimmac).