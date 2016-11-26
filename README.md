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

`brew install cmake git`

create a directory for your dependencies. E.G.: `Documents/vitasdk`

`cd Documents/vitasdk`

`git clone https://github.com/vitasdk/buildscripts.git`

`mkdir build`

`cd build`

`cmake ..`

Lean back and wait cmake to finish. This took me 2 hours. Now vitasdk is compiled in `Documents/vitasdk/build/`

More: TBD
