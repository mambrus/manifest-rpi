# OpenEmbedded/Yocto rPI (poky-pi.git)

Manifest-project for Raspberry-Pi builds using native Yocto/OE

This manifest manages projects, including tool dependencies etc, needed
to set up a layered structure for Yocto/OE based builds of rPI


## Usage

```bash
mkdir poky-pi && cd poky-pi
repo init -u https://github.com/mambrus/manifest-rpi.git
repo sync -j6
source $(pwd)/.env
time bitbake core-image-base
```

The above will fetch the `default.xml` manifest. To chose another, append
the `-m <manifest>` or `-b <branch>` options.

Valid branch-names are short-versions of the MACHINE in non-capital letters,
i.e.:

* rpi
* rpi0
* rpi0-wifi
* rpi2
* <b>rpi3</b>
* rpi4
* rpi-cm
* rpi-cm3

<i>The default is in bold</i>

## Links

* ![Repo manpage](http://manpages.ubuntu.com/manpages/bionic/man1/repo.1.html)

