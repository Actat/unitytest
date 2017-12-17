# unitytest

unityでwindows mixed reality向けのアプリケーションを開発する際のいろいろな設定について記録するリポジトリです。

このリポジトリのunitytestディレクトリをコピペすると初期設定が終了している状態を**目指しています**。

## 利用方法
### unityでプレビュー
1. unityでプログラムを書いて保存
1. HMDを接続
1. 画面中央上の再生ボタンを押す
1. HMDを装着、実行を待つ

### ビルドしてインストール、実行
1. unityでプログラムを書いて保存
1. HMDを接続
1. unityでの操作
    1. [File] -> [Build Settings...] Build Settingsのウインドウを出す
    1. 右下のBuildボタンをクリック
    1. appというディレクトリを選択する（ない場合は作る）
    1. ビルドが始まるので終わるまで待つ
1. visual studioでの操作
    1. unitytest/app/New Unity Project.sln を開く
    1. 画面情報のリボンで設定
        1. ソリューション構成をReleaseにする
        1. ソリューションプラットフォームをx86にする
        1. ビルド先をローカル コンピューターにする
    1. [デバッグ] -> [デバッグなしで開始]
1. HMDを装着、実行を待つ

## 参考文献
- [Windows デベロッパー センター Windows Mixed Reality](https://developer.microsoft.com/ja-jp/windows/mixed-reality)
- [Windows Mixed Reality Headsetで自作コンテンツを動かす with Unity](http://tks-yoshinaga.hatenablog.com/entry/2017/08/23/171354)
- [Windows Mixed Reality 対応アプリ開発のための情報まとめ](https://blogs.msdn.microsoft.com/shintak/2017/09/07/winmrdev/)
