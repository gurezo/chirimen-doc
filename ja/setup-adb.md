### adb のセットアップ
#### android-tools-adbをインストールする  
- Ubuntu 12.10以降
  ```
  $ sudo apt-get install -y android-tools-adb
  ```
- Fedora 19以降
  ```
  $ sudo yum install android-tools -y
  ```
- Mac OSX以降（Homebrew を使っている時）
  ```
  $ brew install android-platform-tools
  ```

#### adb_usb.ini 編集する
```
$ vi ~/.android/adb_usb.ini
```
- 下記の内容を追記する  
~~~~
# 例：Fx0, Open Web Board  
# 他のデバイスも同様に記述する事
# 1 USB VENDOR ID PER LINE.
0x2207
# 2 USB VENDOR ID PER LINE.
0x1004
~~~~

#### ルールを設定する
  ```
  $ sudo vi /etc/udev/rules.d/51-android.rules
  ```

- 下記の内容を追記する
~~~~
# 例：Fx0, Open Web Board  
# 他のデバイスも同様に記述する事
SUBSYSTEM=="usb", ATTR{idVendor}=="2207", MODE="0666", GROUP="plugdev"
SUBSYSTEM=="usb", ATTR{idVendor}=="1004", MODE="0666", GROUP="plugdev"
~~~~

#### 設定を反映をする。
```
$ sudo udevadm control --reload
```

#### 引用
- [ADBをインストールして使用する](https://developer.mozilla.org/ja/docs/Archive/B2G_OS/Debugging/Installing_ADB)
- [ADBコマンド導入の方法](http://qiita.com/hikaru__m/items/15baae425b6fad25da05)
