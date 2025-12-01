# SBCM-MAP-JAPAN
# SBCM Japan Visualizer 🇯🇵
**Visualization of Budget Distortion Index ( $D_{index}$ ) based on Meso-Economics**

このリポジトリは、**「標準ブロック比較法 (SBCM)」** に基づき、日本の基礎自治体における財政構造の歪みを可視化するプロジェクトです。

## 🌐 Live Demo
[地図を見る (View Map)](https://SBCM-Alliance.github.io/sbcm-map/)

## 📊 What is SBCM?
**標準ブロック比較法 (Standard Block Comparison Method)** は、人口規模の異なる自治体を「標準ブロック（人口約7.2万人）」という共通単位で正規化し、比較可能にするフレームワークです。

### 歪み指数 ($D_{index}$) の定義
本マップでは、以下の計算式に基づいて算出された **歪み指数 ($D_{index}$)** をヒートマップとして表示しています。

$$ D_{index} = \frac{I_{budget}}{I_{coverage}} $$

- **$D_{index} \approx 1.0$**: 適正 (標準的な財政規模)
- **$D_{index} > 10.0$**: **歪みあり (Distortion)** - 人口規模に対して過大な予算が投入されている状態

## 🗂 Data Sources (出典)

本プロジェクトでは、以下のオープンデータおよび統計情報を使用しています。

### 1. 地図データ (Map Data)
- **提供**: [スマートニュース メディア研究所 (SmartNews Media Research Institute)](https://github.com/smartnews-smri/japan-topography)
- **原典**: 国土交通省 国土数値情報（行政区域データ）
- **ライセンス**: 本地図データの加工・著作権はスマートニュース社および国土交通省に帰属します。

### 2. 統計データ (Statistics)
マップ上の数値（$D_{index}$）は、以下の公的統計をもとに算出・推計しています。
- **人口データ**: 総務省「住民基本台帳に基づく人口、人口動態及び世帯数」
- **財政データ**: 総務省「地方財政状況調査関係資料（決算カード）」
- **寄附金データ**: 総務省「ふるさと納税に関する現況調査」

## 🚀 Usage (使い方)

### 環境 (Requirements)
- Python 3.x
- Folium
- Geopandas

### 実行方法
Google Colab等のNotebook環境で `map_generator.py` (または該当するスクリプト) を実行することで、最新の地図データ (`index.html`) を生成できます。

## 👤 Author
**Melnus**
- [Standard-Block-Comparison-Method (Theory)](https://github.com/Melnus/Standard-Block-Comparison-Method)

---
*This project is an implementation of Meso-Economics theory.*
