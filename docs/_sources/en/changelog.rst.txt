Lovely Composer - Changelog
#####################################################


.. _id-changelog-1-2-6-en:

ver.1.2.6 - 2022-07-20 
####################################################

List of changes
=====================================

Add

* Added help function: F1 key to open the display screen instructions, F2 key to open the user guide
* Added a function to input continuous copy of notes in the selected range by pressing Ctrl + D
* Added function to display the name of the currently selected scale and its component notes in text (when mouse cursor is placed on the scale key operation button)
* Added function limitation processing, etc. for making the new trial version*

Changes

* Changed default location of song data, etc. to LovelyComposer folder under user document folder (to simplify version upgrade)
* When using the eraser tool, pressing the tone icon in the tone selection tool always switches to the pen tool.

Fixes

* Fixed a problem that the maximum number of folders on the folder selection window was the number of chord patterns
* Fixed the problem that the USER_SFX folder was not set to the default settings for sound effects after song number 32.

Important Notices - Data folder moved!
===============================================
The most important change in version 1.2.6 is that the default location of song data has been changed from directly under the program folder to the LovelyComposer folder under the user document folder.

It's to facilitate program version upgrades for users. Previously, it was necessary to migrate song data each time the program was upgraded. After this version, you should only have to download the new program.

However, to inherit your song data from ver.1.2.5 or older, it requires manual operation only once. So if you need, please follow the steps below. (Make a backup of your song files before proceeding.)

#. At first, please boot new version of Lovely Composer app. The "LovelyComposer" data folder will be automatically created under your User Documents folder when the first time boot. (ex. C:/Users/user_name/Documents/ or /home/user_name/Documents/ or /home/user_name/ ).
#. When the startup is complete, please close Lovely Composer app.
#. Please overwrite the "music" folder and "app_settings.json"  file in the "LovelyComposer" folder under the user documents with your "music" folder and "app_settings.json" file. (From under the program folder of the previous version LovelyComposer. )

*If you still want to place the data under the program folder as before, it is possible to do so in the settings. (Explanation in preparation)

Other features
===================================
You can now open the manual directly from the application with the F1 and F2 keys. The manual has also been corrected to be easier to read!

Added a function to input continuous copy of notes in the selected range by pressing Ctrl + D.

Demo
=======================================
`Youtube <https://youtu.be/kw5izF6dYk4>`_



.. _id-changelog-1-2-5-en:

ver.1.2.5 - 2022-05-18
####################################################

List of changes
============================================================================

Add

* Added the system setting tool (Top right of the screen)
* Supports non-integer multiple enlargement display and linear interpolation display on the screen
* Added the song list window (Display by click the song number display)

Changes

* The maximum number of songs for each folder has been increased up to 100 songs from 32 songs.

Demo
=======================================
`Youtube <https://youtu.be/Pvl7DNT6hLE>`_


ver.1.2.4 - 2022-04-11
####################################################

Linux supported!
==================================

Lovely Composer now supported some of Linux, but the Mac and Raspberry Pi versions are beta versions and are not guaranteed to work.

Version 1.2.4 is mainly a modification for multi-platform support, with no major functional changes. 

Also the default value of audio buffer size has been changed from 2048 to 1024, which will reduces audio playback delay on many PCs, and smoothes the playback position bar and output waveform display. But may cause audio playback instability such as skips and petit noises on a small percentage of PCs. If you are having problems with audio playback, please change the audio buffer size to 2048 from the configuration tool.


Supported Linux
===================================
We have confirmed that the following operating systems work. (x86_64, with the latest updates applied)

* Ubuntu 20.04
* Fedora 34
* Slackware 15.0
* debian 11.3

Following os have checked some problems in the virtual environment, but may work on the actual device.

* Mint Linux 20.3 @ VirtualBox
* Fedora 35 @ VirtualBox

We confirmed that the following operating systems did not boot

* debian 10.10

The Linux version is compiled on Ubuntu 20.04 for now. Basically, it seems to need a newer version than this to work. 

* Linux kernel 5.13.0
* GCC 9.3.0
* GLIBC 2.31

Sounds
===================================
We cannot guarantee that the sound will play comfortably without delay, etc., as it depends on the hardware environment, but even if it does not sound correctly, the problem may be resolved by the settings.

Try using a configuration tool to increase the value of the audio buffer, for example.