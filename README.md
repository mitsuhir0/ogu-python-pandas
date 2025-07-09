# Python Pandas データ分析

![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/pandas-latest-green.svg)
![Quarto](https://img.shields.io/badge/quarto-1.4+-orange.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

Pythonのpandasライブラリを使用した実践的なデータ分析手法を学習するためのインタラクティブなブックです。実際のデータを使用して、段階的にデータ分析を進めていきます。

## 📚 オンライン版

このブックはQuarto Pubでオンライン版を公開しています：
- **オンライン版**: https://your-username.quarto.pub/ogu-python-pandas/


## 概要

このプロジェクトでは、以下のデータ分析手法を実践的に学習できます：

- **データの読み込み・探索**: CSVファイルからのデータ読み込み、基本統計量の算出
- **データ可視化**: matplotlib/pandasを用いたグラフ作成とカスタマイズ
- **統計分析**: 回帰分析、相関分析などの基本的な統計手法
- **結果の解釈**: 分析結果の適切な解釈と表現方法

## 学習内容

### 第1章：景気動向指数分析
日本の景気動向指数（CI）データを使用した経済動向の分析
- 時系列データの扱い方
- 基本統計量の算出
- 時系列グラフの作成と解釈

### 第2章：年収と修学年数データ分析
年収と修学年数の関係を分析し、統計的な関係性を探る
- 散布図による可視化
- 相関分析
- 線形回帰分析（通常・対数変換）
- 回帰結果の解釈

## 使用技術

- **Python 3.8+**: データ分析の主要言語
- **pandas**: データ操作・分析ライブラリ
- **matplotlib**: データ可視化ライブラリ
- **statsmodels**: 統計モデリングライブラリ
- **Quarto**: 動的ドキュメント生成システム

## プロジェクト構造

```
├── _quarto.yml          # Quartoプロジェクト設定
├── index.qmd            # メインページ
├── pages/
│   ├── keiki.qmd        # 景気動向指数分析
│   ├── income.qmd       # 年収と修学年数分析
│   └── csv/
│       ├── keiki_ci.csv     # 景気動向指数データ
│       └── 2_income.csv     # 年収・修学年数データ
├── docs/                # 生成されたHTMLファイル
└── styles.css           # カスタムスタイル
```

## セットアップ

### 1. リポジトリのクローン
```bash
git clone https://github.com/mitsuhir0/ogu-python-pandas.git
cd ogu-python-pandas
```

### 2. 仮想環境の作成（推奨）
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. 必要なライブラリのインストール
```bash
pip install pandas matplotlib matplotlib-fontja statsmodels quarto
```

### 4. Quartoの実行
```bash
quarto render
```

## サンプルデータ

プロジェクトに含まれるサンプルデータ：

- **景気動向指数データ** (`pages/csv/keiki_ci.csv`)
  - 日本の景気動向指数（先行・一致・遅行指数）
  - 時系列データ形式

- **年収・修学年数データ** (`pages/csv/2_income.csv`)
  - 年収（income）と修学年数（yeduc）の関係データ
  - 田中隆一／著『計量経済学の第一歩――実証分析のススメ』（有斐閣，2015年）のウェブサポートページから出版社の許諾を得て転載
  - 出典: https://www.yuhikaku.co.jp/static/studia_ws/index.html#isbn_9784641150287

## 学習の進め方

1. **基礎編**: `pages/keiki.qmd`から始めて、pandas の基本操作を学習
2. **応用編**: `pages/income.qmd`で統計分析と回帰分析を実践
3. **発展編**: 独自のデータで分析手法を応用

## 実行結果の例

### 景気動向指数の推移
時系列グラフによる経済動向の可視化と分析

### 年収と修学年数の関係
- 散布図による関係性の可視化
- 回帰分析による統計的関係の定量化
- 教育の経済的収益率の算出

## 貢献

改善提案やバグ報告は、以下の方法で歓迎します：

1. Issue を作成
2. Pull Request を提出
3. 新しい分析手法の追加提案

## ライセンス

このプロジェクトは MIT ライセンスの下で公開されています。詳細は [LICENSE](LICENSE) ファイルを参照してください。

## 連絡先

- **著者**: Mitsuhiro Okano
- **プロジェクト**: [GitHub Repository](https://github.com/your-username/ogu-python-pandas)

---

**学習のヒント**: 各章のコードを実際に実行しながら進めることで、pandasの機能を効果的に習得できます。質問やフィードバックは Issue でお気軽にお寄せください。