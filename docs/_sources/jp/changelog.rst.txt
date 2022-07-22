Lovely Composer - 更新履歴
#####################################################


.. _id-changelog-1-2-6-jp:

ver.1.2.6 - 2022-07-20
####################################################

.. raw:: html
    <iframe width="560" height="315" src="https://www.youtube.com/embed/kw5izF6dYk4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

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


**デモ**

`Youtube <https://youtu.be/kw5izF6dYk4>`_


ver.1.2.5 - 2022-05-18
####################################################

追加

* システム設定画面追加
* 画面の非整数倍拡大表示、線形補間表示に対応
* フォルダ内の曲一覧表示追加

変更

* フォルダごとに上限32曲だったのを100曲まで扱えるように増量

デモ
=======================================
`Youtube <https://youtu.be/Pvl7DNT6hLE>`_




ver.1.2.4 - 2022-04-11
####################################################

* Windowsに加えてLinuxを正式サポート
* 非公式ベータ版としてMac用とラズベリーパイ用を追加（動作保証なし）
* オーディオバッファサイズのデフォルトを2048から1024に変更


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
####################################################

追加

* 効果音のオン/オフ設定を追加
* オーディオファイルをパートごとにエクスポートするオプションを追加しました
* 内部曲データのJSONLファイルにリズムパターンの音符を追加出力するエクスポート機能を追加しました

変更

* コードパートを選択すると、キーボード（またはMIDIキーボード）でコードを演奏できるようになります
* 選択した出力タイプに応じてオプションを切り替えるようにエクスポート画面のUIを変更しました
* 1ファイル出力をエクスポート画面のデフォルトに変更しました

修正

* ファイルのエクスポート時にパンロウ設定と互換モードの指定が有効にならなかった問題を修正しました
* 効果音が定期的かつ繰り返し再生される可能性がある問題を修正しました。
* サンプル曲で現在利用できないノイズ音色が使用されていたのを修正しました（音は変更されません）



ver.1.2.2 - 2022-01-01
#########################################################

修正

* 再生中に楽譜を編集すると、（再生し直すまで）そのページの音符の音量とパンが正しく再生されなくなる問題を修正しました。
* バージョン番号表記が1.2.0から変わってなかったのを修正しました。


ver.1.2.1 - 2022-12-24
#########################################################

修正

* ペンツールでノートをドラッグ入力するときに、最初の音程がずれる場合がある問題を修正しました


ver.1.2.0 - 2022-12-23
#########################################################

変更

* 4ビットローレゾ三角波を、8bitゲーム機の波形により近くなるようにわずかに変更しました

修正

* トランスポーズ（選択領域のドラッグ）によってノートが画面の外に配置できてしまう問題を修正しました
* コードミュート状態でコードスケールを選択するとフリーズする問題を修正しました
* コード延長線が次のページにまたがる場合、次ページ再生時にミキサーのボリューム指定が無効になる問題を修正しました


1.2.0 公開!
=============================================

約3か月ぶりのメジャーアップデートです！

音量の指定やステレオ対応を追加し、表現力が大きく向上しました。

音量は16段階、ステレオは中央/左/右の選択式と、8bitゲーム機を踏まえた仕様となっています。

Proモードという形で追加したことで、作曲初心者のために従来のシンプルな画面を維持したまま、作曲上級者にはより豊かな表現力や機能を提供します。

また今回は新しく、LovelyComposerの一部のユーザー達が制作したサンプル曲を10曲追加しています。これらの曲は、ver.1.2の音量やステレオ機能を使用したサンプルとなっています。

サンプル曲を使用する場合は、作者名をどこかに表記することを強く推奨していますが、それ以外は自由に使うことができます。詳しくは同梱のreadmeをご覧ください。

サンプル曲の作者の皆様、ありがとうございました!


ver.1.2.0 サンプル曲 (LC_SAMPLE_1.2.0) ------------

     0番 ... 作者名: yktakaha4      曲名: うちゅうなう

     1番 ... 作者名: チカンゴ       曲名: （なし）

     2番 ... 作者名: えなじ～       曲名: Execute

     3番 ... 作者名: tdhr           曲名: （特にありません）

     4番 ... 作者名: 荒巻那智       曲名: まどろむ未確認

     5番 ... 作者名: f@ct           曲名: Fun days

     6番 ... 作者名: にしあぷ       曲名: (原曲) The Other Day, I Met a Bear（アメリカ民謡）

     7番 ... 作者名: hits           曲名: 風の足跡

     8番 ... 作者名: hits           曲名: Starry Drive

     9番 ... 作者名: えなじ～       曲名: 帰り道のアンダンテ

デモ
=======================================
`Youtube <https://youtu.be/9qsP4k_6AVM>`_


ver.1.2.0beta4
#########################################################