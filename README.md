# OpenEmbedded/Yocto rPI (poky-pi.git)

Manifest-project for Raspberry-Pi builds using native Yocto/OE

This manifest manages projects, including tool dependencies etc, needed
to set up a layered structure for Yocto/OE based builds of rPI


## Usage

```bash
mkdir poky-pi && cd poky-pi
repo init -u https://github.com/mambrus/manifest-rpi.git
repo sync -j6
```

The above will fetch the `default.xml` manifest. To chose another, append
the `-m <manifest>` or `-b <branch>` options.

## Links

* ![Repo manpage](http://manpages.ubuntu.com/manpages/bionic/man1/repo.1.html)

