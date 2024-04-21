# subject-220413-setup

- ## [Google Drive for Desktop](https://support.google.com/a/answer/7491144?hl=ja) のインストール
  - R101・R202 教室用アカウントで、共有ドライブを二つアサイン\
  ![image](https://user-images.githubusercontent.com/1501327/163701537-45e12313-1013-464a-80af-b83c3ba7dcde.png)
  - R101・R202 グループをその 共有ドライブに追加して、その共有ドライブを教室ベースのファイル置き場とする
  - Google Drive for Desktop は常に教室用アカウントでログインしておく

- ## 教室PC はリモートアクセス可にしておく
  ![image](https://github.com/winofsql/subject-220413-setup/assets/1501327/3621496f-9800-4ccb-bebc-b14355e66631)

- ## Visual Studio Code のインストール
  - c:\app と **c:\app2** を作成しておく
  - c:\app2 の中に "C:\app2\Microsoft VS Code\Code.exe" となるようにインストール
  - 拡張は https://github.com/winofsql/subject の code-install-ext.bat を実行

- ### Chrome のポリシー設定レジストリを開く処理
  ```bat
  wscript open_reg.vbs HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome
  ```
