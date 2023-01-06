# ROS2

## リポジトリの説明

このリポジトリはROS2を用いて作成したコマンドを含み，ROS2をインストールした環境で実行する．

[![test](https://github.com/RRRCCCIII/ROS2/actions/workflows/test.yml/badge.svg)](https://github.com/RRRCCCIII/ROS2/actions/workflows/test.yml)

## ノード
ノードはリポジトリのROS2/ros2_ws/src/mypkg にあり，talker.pyとlistener.pyをもつ．

- talker.py
0.5秒ごとに数字をカウントし，"countup"トピックを送信する．

- listener.py
talker.pyから送信されるトピックを受信し表示する．

## インストール方法
1. リポジトリをクローン

```bash  
$ git clone https://github.com/RRRCCCIII/ROS2.git
```

2. ディレクトリをクローンしたリポジトリに移動
```bash
$ cd ./ROS2/ros2_ws
```

3. コマンドを実行  
ROS2を使って実行
二つのノードを同時に実行させるために launchファイルを用いる．
```bash
ros2 launch mypkg talk_listen.launch.py
```

## 使用ソフトウェア
- Python 3.7〜3.10

## テスト環境
- Ubuntu 20.04

## ライセンス
このソフトウェアパッケージは，3条項BSDライセンスの下，再頒布および使用が許可されます．

© 2023 Ryuji Hirano
