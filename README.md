# Mac OS X 10.9 Fab Modules Installation Notes

## Dependencies (WXPython)

before you install dependencies with `brew install`, download development (2.9) build of wxpython from [http://www.wxpython.org/download.php](http://www.wxpython.org/download.php) with 2.8 you will probably experience an error like this

```
ImportError: dlopen(/usr/local/lib/wxPython-unicode-2.8.12.1/lib/python2.7/site-packages/wx-2.8-mac-unicode/wx/_core_.so, 2): no suitable image found.  Did find:
  /usr/local/lib/wxPython-unicode-2.8.12.1/lib/python2.7/site-packages/wx-2.8-mac-unicode/wx/_core_.so: no matching architecture in universal wrapper
```

## Installing fab modules

```
git clone http://github.com/johnrees/osx_friendly_fabmodules
cd osx_friendly_fabmodules
mkdir build
cd build
cmake ..
make
sudo make install
```

Then symlink the bin folder to your `PATH`