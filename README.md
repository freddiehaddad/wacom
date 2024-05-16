# Wacom Tablet/Stylus Window Mapper

This utility allows you to quickly map your Wacom tablet/stylus to a specific
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
Usage: wacom [OPTIONS]
Maps your stylus to the specified window.
Example: wacom -a "Lorien v0.6.0" -r none -s "Wacom One by Wacom M Pen stylus"
Maps the stylus to the Lorien v0.6.0 window using the default tablet orientation

Options:
 -a        name of application stylus should be mapped to
           (use xprop to lookup the WM_NAME value)
           (default: Lorien v0.6.0)
 -r        how the tablet is rotated (orientation of tablet)
           options: [none|half|cw|ccw] (default: none)
 -s        name of stylus (use xsetwacom list devices)
           (default: Wacom One by Wacom M Pen stylus)
```
