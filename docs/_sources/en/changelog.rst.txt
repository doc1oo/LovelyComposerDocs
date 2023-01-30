Lovely Composer - Changelog
#####################################################

 
.. _id-changelog-1-3-0-en:

ver.1.3.0 - 2023-01-30 
####################################################

 
List of changes
=====================================

* **New tones (23 patterns)** ... Organ-like triangle wave, Phaser triangle wave, Tilted sawtooth wave, and Slow Drop effects, and fast arpeggio tones.

* **Note Extension Line** ... In addition to making the note edit process easier, several tones are changed sound when extended. (e.g., Piano like tone, with enveloping)

* **Multi Function Pen** ... Note input / Extension line input / Note deletion / Note movement can be done with one pen according to the cursor operation.

* **Fast arpeggio support** ... There are two ways to use fast arpeggio tones or to specify fast arpeggios in rhythm patterns (select ∞).

* **Random Composition Function** ... Simple automatic composition can be easily performed with a single click by setting melody, chord, scales, and rhythm patterns at random. Scales are also set automatically, so it is easy to rewrite melodies. Beginners can use it as a finished product, and advanced users can use it to get ideas for their compositions.

* **Various note manipulation buttons** ... Convenient one-click operation of octave up/down, etc.

* **Instruments arrangement function**

* **Song title / author name / file name setting** ... Currently only alphanumeric characters and a few one-byte symbols are available (US Keyboard base). The file name will be displayed on the song editing screen and can be used as the file name when file exporting.

* **Open in Browser button** ... You can open the user guide (manual), #LovelyComposer tag on twitter, and LovelyComposer server on Discord with one button (upper right corner of the screen)

* **Additional scales (13 types)** ... additional typical scales such as Dorian Scale, Lydian Scale, etc.

* **Additional chord progression patterns (7 types)**

* **New sample songs (21 user-created songs)** ... The amazing songs created with 1.3.0 by ordinary users as sample songs. (See the included Readme for more information about each song and author.)

Changes

* **Improved MIDI export quality** ... The connected notes are now output as one long note. Volume and panning have also been improved.

* Slight changes to UI and button layout

* Window size is now slightly larger

* Changed folder selection dialog to show sample song folders at the bottom

* Volume of bomb button lowered.

Fixes

* **Fixed a bug that the arpeggio rate value of rhythm patterns affected rhythm pattern parts other than chords**

* Fixed a bug that file paths failed when exporting if they contain Japanese characters, etc.

* Fixed behavior after selecting a area with the selection tool

* Fixed a problem that caused error sounds to become louder


.. _id-changelog-1-2-7-en:

ver.1.2.7 - 2022-09-05 
####################################################

List of changes
=====================================

Added

* Added a function to display the folder path by clicking the current folder name display on the upper right of the screen.

Changed

* Changed not to display the file path of the open song folder in the title bar.

Fixed

* Fixed a bug that the app may crash when sound previewing with the key number changed in the chord pattern tool.


.. _id-changelog-1-2-6-en:

ver.1.2.6 - 2022-07-20 
####################################################

List of changes
=====================================

Added

* Added help function: F1 key to open the display screen instructions, F2 key to open the user guide
* Added a function to input continuous copy of notes in the selected range by pressing Ctrl + D
* Added function to display the name of the currently selected scale and its component notes in text (when mouse cursor is placed on the scale key operation button)
* App now remember the song that was open when the app was closed last time. (  When the app started, the song will open​.)
* Added function limitation processing, etc. for making the new trial version*

Changed

* Changed default location of song data, etc. to LovelyComposer folder under user document folder (to simplify version upgrade)
* When using the eraser tool, pressing the tone icon in the tone selection tool always switches to the pen tool.

Fixed

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

Added

* Added the system setting tool (Top right of the screen)
* Supports non-integer multiple enlargement display and linear interpolation display on the screen
* Added the song list window (Display by click the song number display)

Changed

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


ver.1.2.3 - 2022-02-21
#########################################################

In version 1.2.3, sound effect on / off settings, export function, keyboard input improvements, etc. have been made.

Added

* Added Sound Effects on / off setting
* Added an option to export an audio file for each part
* Added a JSONL file export function that adds rhythm pattern notes to the internal song data

Changed

* Enabled to play chords on the keyboard (or MIDI keyboard) when chord part is selected
* Changed the export screen UI to switch options depending on the selected output  type
* Changeed 1 file output to default selection on the export screen

Fixed

* Fixed an issue where Pan Law and Compatibility mode specifications were not enabled when exporting files
* Fixed an issue where pre-played sound effects could be played periodically and repeatedly when the page loop was turned on.
* Fixed a few noise tones that aren't currently available in the sample song (the sound doesn't change)


ver.1.2.2 - 2022-01-01
#########################################################

Only the following changes are made.

* Fixed an issue where if you edited a score during playback, the note volume and pan on that page would play incorrectly. (Until it plays again)
* Fixed the version number notation being still 1.2.0.



ver.1.2.1 - 2022-12-24
#########################################################

Fixed

* Fixed an issue where the first pitch might shift while dragging notes with the Pen tool


ver.1.2.0 - 2022-12-23
#########################################################

Changed

* The 4bit low resolution triangle wave has been slightly modified to be closer to the waveform of an 8bit game machine.

Fixed

* Fixed an issue where notes could be placed off the screen by transpose (dragging the selection area)
* Fixed an issue where putting a chord mute symbol at the end of a page and selecting a chord scale on the next page would freeze
* Fixed an issue where the mixer volume specification would be invalid if the chord extension line spans the next page

1.2.0 released!
==========================================================

This is the major update in about 3 months!

Volume and stereo support have been added, greatly improving expressiveness.

The volume is 16 levels, the stereo is Center / Left / Right selectable. ( the specifications are based on 8-bit game machines. )

With the addition in the form of Pro Mode, advanced composers will be able to provide richer expressiveness and functionality while maintaining the traditional simple screen for beginners.

Also, this time, we have added 10 new sample songs created by some users of Lovely Composer. These songs are samples with volume and stereo features of ver.1.2.

When using a sample song, it is strongly recommended to write the author's name somewhere, but other than that, you can use it freely. See the included readme for details. 

Thank you to the authors of the sample songs!


  ver.1.2.0 Sample music (LC_SAMPLE_1.2.0) ------------

    No. 0 ... Author: yktakaha4                 Title: Uchu-now

    No. 1 ... Author: チカンゴ                  Title: (Untitled)

    No. 2 ... Author: えなじ～                  Title: Execute

    No. 3 ... Author: tdhr                      Title: (Untitled)

    No. 4 ... Author: 荒巻那智 (Nachi Aramaki)  Title: まどろむ未確認

    No. 5 ... Author: f@ct                      Title: Fun days

    No. 6 ... Author: にしあぷ                  Title: (Original Song) The Other Day, I Met a Bear（Traditional American Song）

    No. 7 ... Author: hits                      Title: 風の足跡

    No. 8 ... Author: hits                      Title: Starry Drive

    No. 9 ... Author: えなじ～                  Title: 帰り道のアンダンテ

Demo
=======================================
`Youtube <https://youtu.be/9qsP4k_6AVM>`_



ver.1.2.0beta4 
#########################################################