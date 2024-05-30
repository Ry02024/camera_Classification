# Camera Classification
このリポジトリは、吾妻先生のスクリプトを基に作成されたカメラ分類プロジェクトです。機械学習技術を利用して、異なる種類のカメラで撮影された画像を分類します。

謝辞
このプロジェクトの基盤となるスクリプトを提供していただいた吾妻先生に感謝します。また、Yukinagaの画像分類リポジトリからも多くのインスピレーションとガイダンスをいただきました。

概要
このプロジェクトは、撮影カメラの種類に基づいて画像を分類することを目的としています。高精度な分類を実現するために、ディープラーニングモデルを活用しています。

リポジトリ構成
data/: データセットを保存するディレクトリ
models/: 訓練済みモデルを保存するディレクトリ
notebooks/: 実験や開発用のJupyterノートブック
scripts/: データ処理、訓練、評価のためのPythonスクリプト
README.md: このファイル
セットアップ
プロジェクト環境をセットアップするための手順は以下の通りです：

リポジトリをクローン:

bash
コードをコピーする
git clone https://github.com/Ry02024/camera_Classification.git
cd camera_Classification
依存関係をインストール:

bash
コードをコピーする
pip install -r requirements.txt
データセットを準備:

データセットをdata/ディレクトリに配置します。
データセットが画像分類に適した形式で整理されていることを確認します。
使用方法
訓練
モデルを訓練するには、以下のコマンドを実行します：

bash
コードをコピーする
python scripts/train.py --config config/train_config.yaml
評価
訓練済みモデルを評価するには、以下を使用します：

bash
コードをコピーする
python scripts/evaluate.py --model models/best_model.pth --data data/test
推論
新しい画像に対して予測を行うには：

bash
コードをコピーする
python scripts/inference.py --model models/best_model.pth --image path/to/image.jpg
設定
このプロジェクトでは、訓練パラメータやその他の設定を指定するためにYAML構成ファイルを使用しています。config/ディレクトリにサンプル構成ファイルが含まれています。

参考文献
Yukinagaの画像分類リポジトリ
ライセンス
このプロジェクトはMITライセンスの下でライセンスされています。詳細については、LICENSEファイルを参照してください。
