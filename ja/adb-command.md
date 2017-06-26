## adb のコマンドの使い方
### デバイス確認
- CHIRIMENボードがハードウェア的に接続されているかを確認します。
```
$ adb deveices
```

### adb 起動
- adb プロセスを起動します。
```
$ adb start-server
```

### adb 停止
- adb プロセスを停止します。
```
$ adb kill-server
```

### adb 再起動
- adb プロセスを再起動します。
```
$ adb reboot
```

### adb シェル
- CHIRIMEN内で、Linuxコマンド操作をする時に遣います。
```
$ adb shell
```

### 引用
- [Android Debug Bridge](https://developer.android.com/studio/command-line/adb.html)
