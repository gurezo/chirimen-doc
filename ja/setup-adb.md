## adb のセットアップ
### android-tools-adbをインストールする  
- Ubuntu 12.10以降
  ```
  $ sudo apt-get install -y android-tools-adb
  ```
- Fedora 19以降
  ```
  $ sudo yum install android-tools -y
  ```
- Mac OSX以降（[Homebrew](https://brew.sh/index_ja.html) を使っている時）
  ```
  $ brew install android-platform-tools
  ```

### adb_usb.ini 編集する
```
$ mkdir ~/.android
$ cd ~/.android
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


### 引用
- [ADBをインストールして使用する](https://developer.mozilla.org/ja/docs/Archive/B2G_OS/Debugging/Installing_ADB)
- [ADBコマンド導入の方法](http://qiita.com/hikaru__m/items/15baae425b6fad25da05)
