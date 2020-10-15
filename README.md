# 概要

RPGツクールMZ用のプラグイン。

プレイヤーの前方移動方向に対して円形の光表現を描画する。

# プロジェクトへのインポート方法

1. プラグインをダウンロードする。以下のリンクをクリックすると最新のバイナリを落とせる。
    * [FlashLight-1.0.3](https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/FlashLight-1.0.3.zip)

3. ダウンロードしたZIPファイルを展開する。

2. FlashLight.jsをRPGツクールMZのプロジェクトのプラグインフォルダにコピーする。

3. エディタのプラグイン管理からFlashLightを読み込んでONにする。


# コマンド

## 懐中電灯タイプ

前方移動方向を照らす。

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/command_example_light.png?raw=true">

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/flashlight_light.gif?raw=true">

## 松明タイプ

プレイヤーを中心に照らす。

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/command_example_torch.png?raw=true">

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/flashlight_torch.gif?raw=true">

## 光を消す

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/command_example_off.png?raw=true">

# 開発

## 必要条件

| アプリケーション | バージョン               |
| :--------------- | :----------------------- |
| node.js          | `>=8.11.4`               |
| npm              | `>=5.6.0`                |
| gulp             | `>=2.3.0`                |
| parcel           | `>=1.12.4`               |

[Gulp](https://gulpjs.com/)を以下のコマンドでインストールする。
```
npm install -g gulp
```

[Parcel](https://ja.parceljs.org/)を以下のコマンドでインストールする。
```
npm install -g parcel-bundler
```


## スタートガイド

リポジトリをクローンする。
```
git clone https://github.com/sevenspice/FlashLight.git
```

ディレクトリを移動する。
```
cd FlashLight
```

設定ファイルを編集する。
```
copy mv.origin.json mv.json
```
* mv.jsonの`dest`に、インポートしたいRPGツクールMZプロジェクトのプラグインフォルダを指定すること。

モジュールをインストールする。
```
npm install
```

コンパイルとプロジェクトへのコピーを実行する。
```
gulp
```

以上で、ゲームプロジェクトにプラグインがインポートされる。
