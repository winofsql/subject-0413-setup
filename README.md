# subject-220413-setup

- ## [Google Drive for Desktop](https://support.google.com/a/answer/7491144?hl=ja) のインストール
  - R101・R202 教室用アカウントで、共有ドライブを二つアサイン\
  ![image](https://user-images.githubusercontent.com/1501327/163701537-45e12313-1013-464a-80af-b83c3ba7dcde.png)
  - R101・R202 グループをその 共有ドライブに追加して、その共有ドライブを教室ベースのファイル置き場とする
  - Google Drive for Desktop は常に教室用アカウントでログインしておく

- ## 教室PC はリモートアクセス可にしておく
  ![image](https://github.com/winofsql/subject-220413-setup/assets/1501327/3621496f-9800-4ccb-bebc-b14355e66631)

- ## Visual Studio Code のインストール
  - folder.bat を実行して c:\app と **c:\app2** を作成しておく
  - "G:\共有ドライブ\SE-WORK-DOWNLOAD\microsoft\.vscode.zip" をダウンロード
  - 解凍して C:\Users\ユーザ名\\.vscode に内容を全てコピーして、VScode を起動して拡張の確認
  ![image](https://user-images.githubusercontent.com/1501327/163191863-be277ebe-134b-4bbe-914c-39558b1ae86f.png)
```bat
REM folder.bat
mkdir c:\app
mkdir C:\app\web22
mkdir c:\app2
mkdir c:\user
mkdir c:\TEMP
mkdir c:\TMP
```


- ## xampp.zip( インストール直後 ) c:\xampp に置くことを前提
  - Google ドライブ等より取得( "G:\共有ドライブ\SE-WORK-DOWNLOAD\software\xampp.zip" )
  - 最悪隣の PC の Cドライブからコピー
  - 解答は 7zip で行う事( 他のソフトは使わないように )


- ## Google Chrome の設定
  - 開発用ブックマーク( テンプレート / bookmarks_2022_04_06.html )
  - セキュリティ設定( chrome.reg )
```reg
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome]
"ShowHomeButton"=dword:00000001
"PasswordManagerEnabled"=dword:00000000
"AutofillCreditCardEnabled"=dword:00000000
"AutofillAddressEnabled"=dword:00000000
```

### 上記レジストリを開く処理
```bat
wscript open_reg.vbs HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome
```
