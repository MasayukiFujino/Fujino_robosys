# Fujino_robosys

# ライセンス概要

This repository is licensed under the GPLv3 license, see LICENSE.

# 課題概要

このデバイスドライバはGPLのもとアップロードされています。
このデバイスドライバは、入力した数字に応じて、LEDを点灯させることができます。
ただし、4よりも大きい数字を入力してもLEDは点灯しません。

# ファイルの位置

Fujino_robosys/myled/myled.c

# 操作方法

$ make
$ sudo insmod myled.ko
$ sudo mknod /dev/myled0 c 240 0
$ sudo chmod 666 /dev/myled0
$ echo 1 > /dev/myled0
$ echo 2 > /dev/myled0
$ echo 3 > /dev/myled0
$ echo 4 > /dev/myled0

# 動画URL

https://twitter.com/i/status/1205149596164296704

