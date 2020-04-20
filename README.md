# gnome-day-night-mode

Used to change theme at sunrise and sunset. When the sunsets changes to a dark mode when the sunrises changes the
theme to a light mode.

> Note: It uses [solunar](https://github.com/kevinboone/solunar_cmdline) to get sunrise/sunset times. If solunar isn't found it will attempt to install it.

## Demo

![](https://gfycat.com/milddelayedkob.gif)


## Prerequisites

- Running a gnome DE (only tested on gnome 3)
- git
- make

## Usage

```
wget https://gitlab.com/hmajid2301/gnome-day-night-mode/-/jobs/502692706/artifacts/download
unzip artifacts.zip
sudo dpkg -i gnome-day-night-mode*.deb
```

### Build from Source

You can also build the debian packages from source.

```bash
sudo apt install build-essential autoconf automake autotools-dev dh-make debhelper devscripts fakeroot xutils lintian \
                pbuilder
git clone https://gitlab.com/hmajid2301/gnome-day-night-mode.git
debuild -i -us -uc -b
sudo dpkg -i gnome-day-night-mode*.deb
```

## Appendix

- [Taken from here](https://www.reddit.com/r/unixporn/comments/5crgng/gnome_when_people_ask_why_i_use_gnulinux/)