# clipgrab

Slightly customized version of ClipGrab for macOS (http://clipgrab.org/)

ClipGrab is a GUI frontend for [youtube-dl](https://youtube-dl.org).

See [README](https://github.com/FreedomBen/clipgrab/blob/master/README) for build instructions if you are building yourself.

Unless you want to hack on the code, I would recommend [downloading a pre-built AppImage file](https://clipgrab.org/).

If you find this software useful, please consider making [a donation](https://clipgrab.org/donate).

## Compiling ClipGrab

Pre-compiled packages for ClipGrab are available on https://clipgrab.org
But compiling ClipGrab is really easy!


### Prerequisites

You need to install the Qt5 developer libraries in order to compile the program.

```sh
brew install qt@5
```

## Set env

For Intel Macs, set this as Environment.
```sh
export PATH="/usr/local/opt/qt@5/bin:$PATH"
```

For Apple Silicon Macs, set this as Environment.

```sh
export PATH="/opt/homebrew/opt/qt@5/bin:$PATH"
```

### Compiling

To compile ClipGrab, simply execute the following command:

```sh
qmake clipgrab.pro && make
```

This will create an executable "clipgrab".
