# 概要

RPGツクールMZ用のプラグイン。

プレイヤーの前方移動方向に対して円形の光表現を描画する。

# コマンド

## 懐中電灯タイプ

前方移動方向を照らす。

![command_example_light](https://github.com/user-attachments/assets/95e92f23-6b20-41b5-879d-3c5723615f3e)

![flashlight_light](https://github.com/user-attachments/assets/6c82dea9-7589-4fd0-ab13-916f9cb3642f)

## 松明タイプ

プレイヤーを中心に照らす。

![command_example_torch](https://github.com/user-attachments/assets/3df4a305-d5e6-41d7-bbf3-54579599fbeb)

![flashlight_torch](https://github.com/user-attachments/assets/84d645bc-ec71-41b8-9524-8d3a71dbaabf)


## 光を消す

![command_example_off](https://github.com/user-attachments/assets/944dfb31-ef9f-470a-8136-695525c68104)

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
copy mz.origin.json mz.json
```
* mz.jsonの`dest`に、インポートしたいRPGツクールMZプロジェクトのプラグインフォルダを指定すること。

モジュールをインストールする。
```
npm install
```

コンパイルとプロジェクトへのコピーを実行する。
```
gulp
```

以上で、ゲームプロジェクトにプラグインがインポートされる。
