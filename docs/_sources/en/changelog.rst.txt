Lovely Composer - Change Log
#####################################################


.. _id-changelog-1-2-6-en:

ver.1.2.6
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

Important Notices
===================================
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

ver.1.2.5
####################################################

List of changes
============================================================================
* Added the system setting tool (Top right of the screen)
* Supports non-integer multiple enlargement display and linear interpolation display on the screen
* The maximum number of songs for each folder has been increased up to 100 songs from 32 songs.
* Added the song list window (Display by click the song number display)

Demo
=======================================
`Youtube <https://youtu.be/Pvl7DNT6hLE>`_


変更内容
============================================================================

**追加**

* F1キーで表示画面の説明書、F2キーでユーザーガイドを開くヘルプ機能を追加
* 選択範囲の音符をCtrl + Dで連続コピー入力する機能の追加
* 選択中のスケール名とその構成音をテキスト表示する機能の追加（スケールキー操作ボタンにマウスカーソルを置いたとき）
* 体験版のための機能制限処理等の追加

**変更**

* 曲データ等のデフォルト配置場所を、ユーザドキュメントフォルダ以下のLovelyComposerフォルダに変更（バージョンアップの簡易化のため）
* 消しゴムツール使用時、音色選択ツールで音色アイコンを押したときは常にペンツールに切り替わるようにした

**修正**

* フォルダ選択画面のフォルダの最大数がコードパターンの数になっていた問題を修正
* USER_SFXフォルダの32番以降が効果音向けの初期設定になっていなかったのを修正


※ 重要なお知らせ
============================================================================
今回のアップデートでは、ユーザがプログラムのバージョンアップをしやすくするため、曲データ等のデフォルト配置場所を、プログラムフォルダの直下からユーザドキュメントフォルダ以下のLovelyComposerフォルダ内に変えました。

今まではプログラムのバージョンアップ時に毎回曲データの移行作業をする必要がありましたが、このバージョン以後は新しいプログラムをダウンロードするだけで済むようになるはずです。

ただしver.1.2.5以前から曲データを移行するのには、初回だけ移行作業が必要となります。作業は以下の手順で行ってください。**（事前に曲ファイルのバックアップを作成してください。）**

#. はじめに新しいバージョンのLovely Composerを起動してください。自動的にユーザーのドキュメントフォルダ以下にLovelyComposerフォルダが作成されます。（例\: C\:/Users/ユーザ名/Documents/ ） （※Linuxの場合、 /home/ユーザ名/Documents/ または /home/ユーザ名/ ）。
#. 起動が完了したらそのままLovely Composerを閉じてください。
#. ユーザードキュメントの下のLovelyComposerフォルダ内にある"music"フォルダと"app_settings.json"ファイルへ、あなたのデータファイル（以前のバージョンのプログラムフォルダ以下にあるmusicフォルダとapp_settings.jsonファイル）を上書きしてください。

※今まで通り、プログラムフォルダ以下にデータを配置したい場合は、設定で可能です。（説明の準備中）


**デモ動画**

`Youtube <https://youtu.be/kw5izF6dYk4>`_

