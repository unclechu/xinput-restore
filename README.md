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
It will save propetries of your device to file
with name as device name to `~/.xinput_configs/`.

You can specify custom file name:
```bash
$ xinput-restore --save %ID% red-mouse
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

Also you can redefine saved properties files directory:
```bash
$ env CONFIGS_PATH="$HOME/.custom-saved-xinput-props-dir" xinput-restore
```
