# 概要

RPGツクールMZ用のプラグイン。

プレイヤーの前方移動方向に対して円形の光表現を描画する。

# プロジェクトへのインポート方法

1. プラグインをダウンロードする。以下のリンクをクリックすると最新のバイナリを落とせる。
    * [FlashLight-1.0.0](https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/FlashLight-1.0.0.zip)

2. RPGツクールMZのプロジェクトのプラグインフォルダにコピーする。

3. エディタのプラグイン管理からFlashLightを読み込んでONにする。


# コマンド

## 懐中電灯タイプ

前方移動方向を照らす。

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89%E4%BE%8B_LIGHT.png?raw=true" width="408px">

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/%E6%87%90%E4%B8%AD%E9%9B%BB%E7%81%AF_LIGHT.gif?raw=true" width="408px">

## 松明タイプ

プレイヤーを中心に照らす。

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89%E4%BE%8B_TORCH.png?raw=true" width="408px">

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/%E6%87%90%E4%B8%AD%E9%9B%BB%E7%81%AF_TORCH.gif?raw=true" width="408px">

## 光を消す

<img src="https://storage.googleapis.com/aurelia-github/rpgmaker-mz/flashlight/%E3%82%B3%E3%83%9E%E3%83%B3%E3%83%89%E4%BE%8B_OFF.png?raw=true" width="408px">

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
copy mv.origin.json mv.sjon
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
