# Emacs Setup

## Download source

http://www.gnu.org/software/emacs/#Obtaining

## Build & Install

### Build Commands

```
$ ./configure —prefix=/home/seanh/local --with-x=no --without-sound --without-xpm --without-jpeg --without-tiff --without-gif --without-png --with-ns=no --disable-ns-self-contained

$ make

$ make install
```

Note: Use `—prefix` only on boxes where you can't install locally

`--with-ns=no` disables OSX extensions, and `--disable-ns-self-contained` stops creation of an OSX `.app` package.

The last bit enables the install process to put things in /usr/local/bin like normal.

### Linux subtleties

Try this next one if you're missing dependencies on Ubuntu. Perhaps emacs24 would work too.

```
sudo apt-get build-dep emacs23
```

However, I’m pretty sure this is usually all you need, so try it first:

```
sudo apt-get install libncurses5-dev
```

Don't forget to update your path in .bashrc if you installed locally.

## Saving my config

Simple command to update tarball:

```
tar -czf emacs_config.tgz .emacs.d .emacs
```
