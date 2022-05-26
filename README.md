# Scripts

## Description

This Repository contains a collection of scripts I composed to automate/simplify tasks.

### <a href="./link">Link</a>
The 'link' script automates symlinking binaries to user's binary folder [$HOME/.local/bin]

### <a href="./dmenu">Dmenu</a>

Scripts in there utilize dmenu for execution.

- <a href="./dmenu/bin/keys">Keys</a> - Copies keys to xclip for simple encrypted password management.
#### Dependencies
- dmenu
- gnuGpg
- xclip

#### Usage
	- Make a directory - `mkdir ~/Documents/Keys`
	- Run the link script to add keys to path
	- Run `gpg --full-generate-key`
	- "create" creates keys
	- "remove" removes an existing key
	- "clear" clears the clipboard

### <a href="./bin">Bin</a>
General Purpose scripts will be stored here

#### [compile-kernel](./bin/compile-kernel)
#### Dependencies
- genkernel
- glibc
#### Standard Configuration
- Compiles Kernel.
	- 6 Jobs (12gb+ ram and at least six threads recommended).
- Installs all the kernel modules.
- Copies Kernel Binary to /boot directory.
	- Make sure /boot is mounted.
- Generates InitramFS.
	- LVM support.
  - Luks support.
  - Zstd Compression.
- Updates grub configuration in /boot.


#### Credits & Contact
- [My Website]("https://ddenobrega.github.io")
- [My Github]("https://github.com/ddenobrega")
- dcdenobrega@gmail.com
