# The premise

> And now for our next trick, we're going to revive old Canon LaserShot LBP printer!

There are many ways to do that, so I've splitted them into two categories:

- Solutions involving Windows in some way
- Solutions involving GNU/Linux

The latter can also be used to make a printer visible for your local network,
so you might use Windows, MacOS, another Linux machine or even Android phone to
print off the main Linux machine.

## Warning: not ready just yet

## 🏠 Windows ways

- VirtualBox with Windows XP 32/64-bit, original driver from Canon,
  guest additions, usb passthrough and bidirectional drag'n'drop for
  the files and batch file for easy launch
- Naturally a Windows XP 32/64-bit installation

## 🐧 Linux ways

- Install CUPS and
  - build a specific reverse-engineered driver and use this machine directly
  - Or use static binaries for x86-64 systems
  - Or use .deb package with original drivers from the Canon
- Or as a print server

## TODOs

- [ ] Heavily refactor Linux capt driver for LBP-810 and LBP-1120
- [ ] Explain Windows ways (make a tutorial)
- [ ] Explain Linux ways (make a tutorial)
- [ ] Emojis all over the place for this README

## Acknowledgments

## ???

<!-- build-essential -->
