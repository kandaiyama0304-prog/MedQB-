MedQB v1.2 更新内容

1. Android上部の時刻とMedQBの重なりを修正
   - Android 15 / targetSdk 35でもstatus bar insetを取得してWebViewを下げる方式へ変更

2. 各単元の学習状況バーを3色化
   - 青：最後の解答が正解
   - 赤：最後の解答が誤答
   - 灰：未回答
   - 各色の問題数もバー下に表示

GitHubでは index.html / MainActivity.java / build.gradle の3ファイルを上書きし、Commit changesしてください。
その後 Build MedQB APK が自動実行されます。

3. 今後の上書き更新用に固定debug署名を追加
   - medqb-debug.keystore をGitHubリポジトリ直下に置きます。
   - v1.2を一度入れ直した後は、この鍵を使い続ける限りv1.3以降を上書き更新できます。
   - この鍵は個人用/開発用です。Play Store公開用の本番署名には使わないでください。

今回はv1.1と署名が異なるため、v1.2導入時だけ旧アプリのアンインストールが必要になる可能性があります。先に学習データを書き出してください。

GitHubへアップロードするファイル：
- index.html
- MainActivity.java
- build.gradle
- medqb-debug.keystore
