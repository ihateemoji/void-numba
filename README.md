# void-numba
This repository contains XBPS templates for packaging numba and its dependency llvmlite for Void Linux.

It provides `python3-numba` and `python3-llvmlite`.

## Installation
Clone this repository:
```sh
git clone https://github.com/ihateemoji/void-numba.git
```

Copy the package directories into the srcpkgs directory of your Void Packages repository:

```sh
cp -r void-numba/srcpkgs/* /path/to/void-packages/srcpkgs/
```

Build the packages (llvmlite first, then numba):

```sh
./xbps-src pkg python3-llvmlite
./xbps-src pkg python3-numba
```

Install the packages:

``sh
xi python3-llvmlite python3-numba
``
