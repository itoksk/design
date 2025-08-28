# Brutalist Web Design Template

## 概要
このテンプレートは、ブルータリズムデザインの原則に基づいた、大胆で実験的なWebデザインシステムです。

## デザイン哲学

### コアコンセプト
- **非対称性**: 予測不可能なレイアウト配置
- **生々しさ**: 装飾を排除した素材感
- **機能美**: 構造そのものがデザイン
- **大胆さ**: 極端なサイズとコントラスト

## 主要な特徴

### 1. レイアウトパターン
- 斜めセクション（skewY変換）
- 壊れたグリッド（不規則な列幅）
- 浮遊要素（絶対配置）
- 分割スクリーン（非対称分割）
- 回転要素（rotate変換）

### 2. タイポグラフィ
- 巨大テキスト（15vw〜12rem）
- 縦書きテキスト
- アウトラインテキスト
- 斜体配置
- モノスペースフォント多用

### 3. カラースキーム
```
Primary: #000000 (Pure Black)
Accent: #FFFF00 (Electric Yellow)
Text: #FFFFFF (Pure White)
Muted: #666666 (Dark Gray)
```

### 4. インタラクション
- カーソル: crosshair
- ホバー: 文字間隔変化
- アニメーション: 浮遊、回転、グリッチ

## ファイル構成
```
brutalist-design-template/
├── README.md
├── design-system.yaml
├── prompts.md
├── components.json
└── examples/
    └── sample.html
```

## 使用方法

1. `design-system.yaml`でカラーとフォントを調整
2. `prompts.md`のプロンプトをAIに投げて基本構造を生成
3. `components.json`から必要なコンポーネントを選択
4. カスタマイズして実装

## 注意事項
- アクセシビリティへの配慮が必要
- モバイル対応は個別に調整必要
- 読みやすさより芸術性を優先したデザイン