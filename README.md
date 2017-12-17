# unitytest

unityでwindows mixed reality向けのアプリケーションを開発する際のいろいろな設定について記録するリポジトリです。

## 利用方法
### 初期設定
1. unityのプロジェクトを作成
1. MainCameraの座標を(0, 0, 0)に設定
1. [File] -> [Build Settings...] Build Settingsのウインドウを出す
1. Add Open Scenes で現在のシーンを追加
1. Platform で Universal Windows Platform を選択
1. Switch Platform ボタンをクリック
1. Build Settings ウインドウ右側の設定
    1. Target device: Any device
    1. Build Type: D3D
    1. SDK: Latest installed
    1. Build and Run on: Local Machine
1. 左下の Player Settings... ボタンをクリック
1. 右側のInspectorでの設定
    1. Other Settings を開く
        - Script Backend を .NET にする
    1. XR Settings を開く
        - Virtual Reality Supported にチェックを入れる

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
    1. 画面上方のリボンで設定
        1. ソリューション構成をReleaseにする
        1. ソリューションプラットフォームをx86にする
        1. ビルド先をローカル コンピューターにする
    1. [デバッグ] -> [デバッグなしで開始]
1. HMDを装着、実行を待つ

## 参考文献
- [Windows デベロッパー センター Windows Mixed Reality](https://developer.microsoft.com/ja-jp/windows/mixed-reality)
- [Windows Mixed Reality Headsetで自作コンテンツを動かす with Unity](http://tks-yoshinaga.hatenablog.com/entry/2017/08/23/171354)
- [Windows Mixed Reality 対応アプリ開発のための情報まとめ](https://blogs.msdn.microsoft.com/shintak/2017/09/07/winmrdev/)
