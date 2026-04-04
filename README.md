# SRB2 Cherry
SRB2 Cherry is a project containing the Reveries and Redberries source modifications of Sonic Robo Blast 2.

[Sonic Robo Blast 2](https://srb2.org/) is a 3D Sonic the Hedgehog fangame based on a modified version of [Doom Legacy](http://doomlegacy.sourceforge.net/).

## Installation
[![latest release](https://badgen.net/static/get/reveries/yellow)](https://mb.srb2.org/addons/reveries.4008/)
[![latest release](https://badgen.net/static/get/redberries/pink)](https://mb.srb2.org/addons/redberries.8043/)

Click either of the above badges to be redirected to the respective SRB2 Message Board release topic containing documentation, changelogs, and Windows downloads.

Reveries is available for Linux via the official flatpak: https://flathub.org/en/apps/io.github.srb2.rphys

## Compiling

This guide is only for Linux, I do not officially support compilation on other OS but https://github.com/Bijman/srb2bld may be able to help you with that.

You need `git`, `make`, `gcc` and development libraries for the following dependencies installed via your package manager: `libpng zlib libsdl2 libsdl2_mixer libgme libcurl libopenmpt libminiupnpc`

Here's a bunch of lists of the correct package names to install for certain distros, as of 04/04/2026:<br>
Debian: `make git gcc libsdl2-mixer-dev libpng-dev libcurl4-openssl-dev libgme-dev libopenmpt-dev libminiupnpc-dev`<br>
Arch: `base-devel git libpng zlib sdl2 sdl2_mixer libgme curl libopenmpt miniupnpc`<br>
Gentoo: `dev-vcs/git media-libs/libpng sys-libs/zlib media-libs/libsdl2 media-libs/sdl2-mixer media-libs/game-music-emu media-libs/libopenmpt net-misc/curl net-libs/miniupnpc`<br>
Alpine: `alpine-sdk zlib-dev libpng-dev curl-dev sdl2-dev sdl2_mixer-dev libgme-dev libopenmpt-dev miniupnpc-dev`<br>
Fedora: `make gcc git libpng-devel zlib-devel SDL2-devel SDL2_mixer-devel game-music-emu-devel libcurl-devel libopenmpt-devel miniupnpc-devel`

After `git clone`ing the repo, `git checkout` to either `cherry` for Reveries or `cherry-candied` for Redberries. Then, enter `make clean && make` to compile. Alpine Linux users must also append `NOEXECINFO=1` to work around an issue caused by lack of glibc.

## Disclaimer
Sonic Team Junior is in no way affiliated with SEGA or Sonic Team. We do not claim ownership of any of SEGA's intellectual property used in SRB2.
