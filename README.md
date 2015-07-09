xinput-restore
==============

Saving and restoring xinput devices properties utility.

Usage
=====

Find the ID of your device in the list:

```bash
$ xinput list
```

Save properties of your device
(replace %ID% to ID number of your device from `xinput list`):

```bash
$ xinput-restore --save %ID%
```

You can change some properties in `~/.xinput_configs/`

Restore properties for specific device:

```bash
$ xinput-restore --restore red-mouse
```
or by device id:
```bash
$ xinput-restore --restore '1452, 781'
```

Restore properties by all saved configs:

```bash
$ xinput-restore
```
