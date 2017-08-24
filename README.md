# Installation

	wget 'https://raw.githubusercontent.com/laurent22/wslpath/master/wslpath'
	sudo mv wslpath /usr/bin

# Features

- Auto-detects path - converts to a Unix path if it is a Windows path and vice-versa.
- Correctly handles symlinks (Since Windows does not know about the WSL symlinks, they are resolved and the link target is returned).
- Correctly handles paths under lxss directory (this is the hidden user directory under which WSL-only files and directories are located).
- Correctly handles :line:column suffix. For example, `subl $(wslpath /mnt/d/script.js:10:2)` would open D:\script.js at line 10, column 2 in Sublime Text

# License

MIT