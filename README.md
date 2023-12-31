# Dwmblocks

Modular status bar for dwm written in c.

## Usage

To use dwmblocks first run 'make' and then install it with 'sudo make install'.
After that you can put dwmblocks in your xinitrc or other startup script to have it start with dwm.

```shell
git clone https://github.com/04burhanuddin/dwmblocks.git
cd dwmblocks
sudo make clean install
```

> Note: if you use dwm it doesn't support [statsu2d](https://dwm.suckless.org/patches/status2d/) color in the `config.h` file please delete it as an empty string, so it doesn't get an error when it's compiled

## Modifying blocks

The statusbar is made from text output from commandline programs.
Blocks are added and removed by editing the blocks.h header file.
By default the blocks.h header file is created the first time you run make which copies the default config from blocks.def.h.
This is so you can edit your status bar commands and they will not get overwritten in a future update.

## Patches

Here are some patches to dwmblocks that add features that I either don't want to merge in, or that require a dwm patch to work.
I do not maintain these but I will take pull requests to update them.

[dwmblocks-statuscmd-20200717-941f415.diff](https://gist.github.com/toniz4/41d168719e22bf7bc4ecff09d424b7d2)
