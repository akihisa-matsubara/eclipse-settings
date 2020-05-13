# eclipse-settings
Eclipseの設定  

## 利用バージョン
2019.03(V4.11)  
Pleiades All in One Java  
Full edition  
64bit  

http://mergedoc.osdn.jp/

## 利用プラグイン
1.  ~~YEdit~~
1.  ~~Spring Tools 4 - for Spring Boot~~
1.  IBM WebSphere Application Server Developer Tools  
    IBM WebSphere Application Server V9.x Developer Tools  
    IBM WebSphere Application Server Liberty Developer Tools Beta  
    https://developer.ibm.com/wasdev/docs/websphere-developer-tools-releases/  
1.  sonarlint 4.1
1.  ~~jshint~~
1.  Darkest Dark Theme with DevStyle
1.  Properties Editor
1.  ERMaster
1.  ~~markdown editor~~  
    https://nodeclipse.github.io/updates/markdown/

### eclipse.ini
```
-vm
C:/IBM/WebSphere/AppServer/java/8.0/bin/javaw.exe
-Xms3g
-Xmx3g
-Dfile.encoding=utf-8
```

### Settings
- 一般>エディター>テキストエディター  
  空白文字を表示>可視性の構成 空白すべてチェック 透明度20  
  印刷マージン 160  

- 一般>エディター>テキストエディター>注釈  
  Check Style警告 濃い黄色  

- 一般>エディター>ファイルの関連付け  
  *.html             HTMLエディター  
  *.properties       プロパティエディター  
  *.yml, *.yaml      YEdit  

- 一般>外観>色とフォント  
  Ricty Diminished  

- Checkstyle>新規  
  my_checks  
  my_checks 構成>フィルター>抑制フィルター>開く `my_checks__resources_suppressions.xml` を指定  

- EGradle>エディター>構文の色の指定  
  通常の文字列               薄紫  

- ERMaster>JDBCドライバー  
  DB2 編集

- Java>インストール済みのJRE  
  WebSphere Application Server  

- Java>インストール済みのJRE>実行環境  
  Java1.8 -> WebSphere Application Server  

- Java>コード・スタイル>インポートの編成  
  インポート  

- Java>コード・スタイル>フォーマッター  
  インポート  

- Java>コンパイラー>エラー/警告  
  潜在的なプログラミングの問題>serialVersionUID なしのシリアライズ可能クラス    警告  

- Java 永続化>JPA>エラー/警告  
  型>解決できないマッピング・ファイル    警告  

- JavaScript>コード・スタイル>フォーマッター  
  インポート  

- Maven>ユーザー設定  
  グローバル設定  
  設定の更新  
  索引再作成  

- XML>XMLファイル>エディター  
  行の幅             160  
  スペースを使用したインデント  
  インデント・サイズ 4  

- Web>HTMLファイル>エディター  
  行の幅             160  
  スペースを使用したインデント  
  インデント・サイズ 2  

- チーム>Git  
  デフォルト・リポジトリー・フォルダー  
  接続タイムアウト   60  

- チーム>Git>構成  
  core.autocrlf      false  

- データ管理>SQL開発>SQLエディター>構文の色の指定  
  シングル・クォート文字列   薄紫  
  型                       薄青  
  識別子                   薄ピンク  


# 番外編：vscode-settings
Visual Studio Codeの設定  

## 利用プラグイン
1.  Table Formatter
1.  Auto-Open Markdown Preview
1.  Material Icon Theme
1.  EsLint (Style: AirBnB)
1.  code-eol

## 等倍フォントの設定
メニュー>ファイル>基本設定>設定  
```
{
    "editor.fontFamily": "Ricty Diminished",
    // フォントサイズ
    "editor.fontSize": 14,
    // ホワイトスペースの表示
    "editor.renderWhitespace": "all",
}
```
