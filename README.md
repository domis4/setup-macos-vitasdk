# IMPORTANT NOTE:
there is an official vitasdk setup instruction on 
https://vitasdk.org/
which should be prefered to this.


# vitasdk exports for fish shell (works on linux too)
https://gist.github.com/domis4/0bce4407ec89c6662fa61862dd8fb248#file-config-fish

# setup-macos-vitasdk
build, install and setup vitasdk on macOS Sierra. 

Note: 
Tested Version was fc475ba6f57e247deca2457de65c3c98c8fb9085
https://github.com/vitasdk/buildscripts/commit/fc475ba6f57e247deca2457de65c3c98c8fb9085

project url: https://github.com/vitasdk

## Build from Source
this took on my Macbook White 2010 7,1 about 2 hours

### prerequisits
- macOS Sierra (older OS X Versions might work too)
- brew http://brew.sh/ 

### install needed packages
- cmake
- git
- autoconf
- texinfo
- bison
- flex

` brew install cmake git autoconf texinfo bison flex`

create a directory for your dependencies. E.G.: `Documents/vitasdk`

`cd Documents/vitasdk`

`git clone https://github.com/vitasdk/buildscripts.git`

`mkdir build`

`cd build`

`cmake ..`

`make -j4`

Lean back and wait cmake to finish. This took me 2 hours. Now vitasdk is compiled in `Documents/vitasdk/build/`


## Installing vitasdk

1. as suggested in https://henkaku.xyz/developer/ move the `vitasdk/build` to `/usr/local/vitasdk`
2. edit `sudo nano /etc/paths` and add the location of your `vitasdk/bin` folder. In case you copied it to `usr/local/vitasdk` it would be: 
`/usr/local/vitasdk/vitasdk/bin`

## Setup a workspace

For project files, e.G.
`mkdir Documents/workspace/vita`

## Build and install Vita Portlibs

1. clone github repo 
`git clone https://github.com/xerpi/vita_portlibs`
2. build and install Vita Portlibs. It will be installed to $VITASDK Directory. 
`sudo make all`

More: TBD
