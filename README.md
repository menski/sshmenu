# sshmenu

A simple [`dmenu`][] script to select a host to start a ssh session in a new terminal.
It is highly inspired by [`passmenu`][].

## Installation

Add [`sshmenu`][] to your `PATH` and make it executable.

## Options

The script can be configured by the following environment variables:

- `SSH_CMD`: ssh command to use, e.g. `mosh` (default: `ssh`)
- `TERM_CMD`: command to start new terminal (default: `urxvt -e`)
- `SSH_CONFIG_FILE`: path to ssh config file (default: `$HOME/.ssh/config`)

## Usage

Call it from commandline:

```
$SSH_CMD=mosh sshmenu
```

or add a keyboard shortcut to your window manager, e.g. for [`i3`][]

```
bindsym $mod+m exec SSH_CMD=mosh sshmenu
```

## License

[WTFPL](LICENSE)


[`dmenu`]: http://tools.suckless.org/dmenu/
[`passmenu`]: http://git.zx2c4.com/password-store/tree/contrib/dmenu/passmenu
[`i3`]: https://i3wm.org/
[`sshmenu`]: sshmenu
