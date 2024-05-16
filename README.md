# Wacom Tablet/Stylus Window Mapper

This utility allows you to quickly map your Wacom tablet/style to a specific
application window instead of the entire screen.

See the `wacom` bash script for configuration.

```text
              Monitor
+---------------------------------+
|                 +-----------+   |
|                 |  Drawing  |   |   After running the utlity,
|                 |  Program  |   |   the stylus is bound to the
|                 |           |   |   drawing program window.
|                 |           |   |
|                 |           |   |
|                 |           |   |
|                 +-----------+   |
+---------------------------------+
```

## Usage

```text
Usage: wacom [OPTION]...
Maps your stylus to a specified window.
Example: wacom -a "Lorien v0.6.0" -r none -s "Wacom One by Wacom M Pen stylus"
Maps the stylus to the Lorien v0.6.0 window using the default tablet orientation

Options:
 -a         Name of application stylus should be mapped to
            Use xprop to lookup the name
            (default: Lorien v0.6.0)
 -r         How the table is rotated (i.e. orientation of tablet)
            Options: [none|half|cw|ccw] (default: none)
 -s         Name of stylus.
            Use xsetwacom list devices for name.
            (default: Wacom One by Wacom M Pen stylus)
```
