## WebIDE の使い方
### WebIDE の出し方
- メニューバー => ツール => ウェブ開発 => WebIDE
![img/01.Menu-WebIDE.png](img/01.Menu-WebIDE.png)
- WebIDE が表示されました。
![img/02.WebIDE.png](img/02.WebIDE.png)

### CHIRIMENの接続確認のやり方
- 下図のように「chirimen」と表示されていれば、接続OKです。<br>
![img/03.device.png](img/03.device.png)
- 表示されていない場合は、[adb コマンド](04.adb-command.md) を用いて確認します。<br>
  ※接続又は認識されていない表示例<br>
![img/No-Device.png](img/No-Device.png)

### アドオンインストールの確認のやり方
- 「シュミレータをインストール」をクリックします。<br>
![img/04.add-on.png](img/04.add-on.png)
- 下記コンポーネントがインストールされている事を確認します。
  - **ADB Helper アドオン（必須）**
  - **ツールアダプタアドオン（必須）**
  - Firefox OS x.x シミュレータ (任意)
  ![img/05.add-on.png](img/05.add-on.png)
