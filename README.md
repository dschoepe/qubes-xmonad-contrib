# Overview

This repository is a fork of
[xmonad-contrib](https://www.github.com/xmonad/xmonad-contrib) and
contains patches to provide better integration with
[QubesOS](https://www.qubes-os.org/). The corresponding
[fork](https://www.github.com/dschoepe/qubes-xmonad) of the main
xmonad repository is needed for compiling and using this. Instructions
on building and running can be found in the old `README` file.

# Changes

- `XMonad.Layout.Decoration` has been modified to indicate which Qubes
  domain a window is running in. This also affects derived layouts,
  such as `XMonad.Layout.Tabbed`.

# Known Issues

- Only modules based on `XMonad.Layout.Decoration` indicate the domain
  of a window. Other modules making use of the normal border colors
  specified in the xmonad configuration are unchanged.
