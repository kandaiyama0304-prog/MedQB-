# MedQB Smartphone Kit

スマホへ入れるための完成パッケージです。

## Android
このリポジトリをGitHubへ置くと、GitHub Actionsが `app-debug.apk` を自動作成します。

1. GitHubで新しいリポジトリを作成
2. このフォルダの中身をリポジトリへアップロード
3. GitHubの Actions → `Build Android APK` を開く
4. `Run workflow` を押す
5. 完了後、Artifacts の `MedQB-Android-APK` をダウンロード
6. ZIP内の `app-debug.apk` をAndroidスマホへ送り、開いてインストール

Android側で「この提供元のアプリを許可」が必要になる場合があります。

## iPhone / iPad
iPhoneではAppleの署名なしでIPAを直接インストールできないため、PWAとしてホーム画面へ入れる方式を用意しています。

1. このフォルダをGitHubへアップロード
2. Repository Settings → Pages → Source を `GitHub Actions` に設定
3. Actions → `Deploy MedQB PWA` を実行
4. 発行されたHTTPS URLをiPhoneのSafariで開く
5. Safariの共有ボタン → `ホーム画面に追加`

これでMedQBがホーム画面にアイコン付きで入り、アプリのように起動します。オフライン対応です。

## 学習データ
学習履歴・お気に入り・メモは端末内に保存されます。
以前のHTML版のデータは、旧版で「学習データ書き出し」→新アプリで「読み込み」を使って移行してください。

## 収録
- 1,829問
- 基礎医学・臨床医学
- 症例問題
- 高度5連問
- 検査値・計算・心電図・画像模式図
- 検索
- 重要度
- 問題別正答率
- 選択肢別解説
- 弱点分析
- 誤答復習
- お気に入り
- 模試
