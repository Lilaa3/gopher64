# This fork does one thing, and one thing only, compile with base x86_64.

![](justonemore.png)

Image above is a joke, I understand fully why v3 makes sense for a project heavily relying on IPC to be good.
However, it is stupid to ask people everyone with competent hardware to compile stuff themselves for a minor performance boost.

Also the creator of gopher, Logan, is really cool and you should donate to them if you can, don't take my frustration the wrong way.

# gopher64 (but it respects your hardware)
Gopher64 is a cross-platform N64 emulator. Some notable features:
* Netplay
* Homebrew support
* Upscaling
* CRT shader
* Emulate CPU overclocking
* Cheats
* Savestates
* RetroAchievements

## download

Windows:
* Standalone executable: [gopher64-windows-x86_64.exe](https://github.com/Lilaa3/gopher64/releases/latest/download/gopher64-windows-x86_64.exe)

Linux:
* Standalone executable: [gopher64-linux-x86_64](https://github.com/Lilaa3/gopher64/releases/latest/download/gopher64-linux-x86_64)

## wiki

https://github.com/gopher64/gopher64/wiki

## discord

[Discord invite link](https://discord.gg/9RGXq8W8JQ)

## controls

Keys are mapped according to [these defaults](https://github.com/gopher64/gopher64/wiki/Default-Keyboard-Setup). Xbox-style controllers also have a [default mapping applied](https://github.com/gopher64/gopher64/wiki/Default-Gamepad-Setup).

## netplay

Gopher64 supports netplay (online play with others) via cloud hosted servers. You can also run the [server](https://github.com/gopher64/gopher64-netplay-server) yourself on a LAN.

## portable mode

If you would like to keep all the game data in the same folder as the executable, you just need to create a file called "portable.txt" in the same directory as the executable.

## building and usage

1. Linux only: [install the SDL3 dependencies](https://wiki.libsdl.org/SDL3/README-linux#build-dependencies). You may also need llvm and the fontconfig dev library. Look for the equivalents on your distro, for opensuse those would be `fontconfig-devel` and `llvm`
2. [Install rust](https://www.rust-lang.org/tools/install)
3. `git clone --recursive https://github.com/gopher64/gopher64.git`
4. `cd gopher64`
5. `cargo build --release`
6. `./target/release/gopher64 /path/to/rom.z64`

## contributing

I will only accept contributions to maintain this, code changes are intended to go to the actual project, don't submit issues to the base repo that you or someone can't repro in the original repo itself.

## license

Gopher64 is licensed under the GPLv3 license. Many portions of gopher64 have been adapted from mupen64plus and/or ares. The license for mupen64plus can be found [here](https://github.com/mupen64plus/mupen64plus-core/blob/master/LICENSES). The license for ares can be found [here](https://github.com/ares-emulator/ares/blob/master/LICENSE).
