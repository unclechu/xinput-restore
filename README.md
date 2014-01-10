xinput-restore
==============

Saving and restoring xinput devices properties by device ID

Usage
=====

Find the ID of your device in the list:

    xinput list

Save properties of your device (replace %ID% to ID number of your device from xinput list):

    xinput-restore --save %ID%

You can change some properties in ~/.xinput_configs/%DEVICE_PRODUCT_ID%

Restore properties:

    xinput-restore
