# 企業ランダム抽出プログラム

## プロジェクト概要

このノートブックは、指定されたEDINETコードリストを基に、特定の条件（決算日、上場区分、連結の有無）で企業をフィルタリングし、各業種から重複なしでランダムに企業を抽出することを目的としています。
抽出された企業リストはCSVファイルとして出力されます。

## ディレクトリ構成

```
company_random_sampler/
├── README.md
├── 企業ランダム抽出プログラム.ipynb
├──output.csv
└── data/
    └── EdinetcodeDlInfo.csv
```

## 使用環境

本プロジェクトは **Google Colab** 上での実行を想定しています。

Colab では以下の主要ライブラリがあらかじめ利用可能です：
- Python 3.10
- Jupyter Notebook（Colab環境）
- pandas
- numpy
- matplotlib
- seaborn

追加で必要なライブラリがある場合は、Notebook の冒頭で次のようにインストールしてください：
```python
!pip install ライブラリ名
```

## データについて
企業データについてはEDINETコードリストからダウンロードできます。(2025/11/11時点)

```data```フォルダの直下に配置してください。
- https://disclosure2.edinet-fsa.go.jp/weee0010.aspx

## 結果・出力
Notebookを実行すると、抽出された企業データの結果が```output.csv```が保存されます。
