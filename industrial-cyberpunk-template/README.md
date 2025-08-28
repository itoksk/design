# Industrial Cyberpunk Design Template

## 概要
工業的サイバーパンクデザインシステム。警告色と技術的要素を組み合わせた、緊急性と機能性を表現するWebデザインテンプレート。

## デザイン哲学

### コアコンセプト
- **Industrial Warning**: 工場の警告標識から着想
- **Technical Typography**: 技術文書のような正確性
- **Functional Chaos**: 機能的でありながら緊急性を演出
- **ASCII Engineering**: エンジニアリング図面のような装飾

### 視覚的特徴
1. **カラーパレット**: 黄黒の警告色 + 赤のアクセント
2. **タイポグラフィ**: モノスペースと極太フォントの組み合わせ
3. **レイアウト**: グリッドベースだが意図的な破壊
4. **装飾**: ASCIIボーダー、警告ストライプ、技術的記号

## 使用シーン

### 最適な用途
- ハッカソン・技術イベントサイト
- 工業系・製造業のプロジェクト
- セキュリティ・警告システムUI
- 技術ドキュメンテーション
- ゲームやSFコンテンツ

### 避けるべき用途
- 企業の公式サイト
- 医療・福祉関連
- 子供向けコンテンツ
- フォーマルな政府機関

## ディレクトリ構成

```
industrial-cyberpunk-template/
├── README.md           # このファイル
├── design-system.yaml  # デザイントークン定義
├── components.json     # 再利用可能コンポーネント
├── prompts.md         # AI生成用プロンプト
└── examples/          # 実装例
    ├── basic.html     # 基本実装
    └── advanced.html  # 高度な実装例
```

## クイックスタート

### 1. 基本HTML構造
```html
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <title>Industrial Cyberpunk Site</title>
    <link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Bebas+Neue&display=swap" rel="stylesheet">
</head>
<body style="background: #000; color: #FF0; cursor: crosshair;">
    <!-- コンテンツ -->
</body>
</html>
```

### 2. 必須スタイル
```css
/* ベーススタイル */
* { margin: 0; padding: 0; box-sizing: border-box; }
body {
    background: #000;
    color: #FFF;
    font-family: 'Space Mono', monospace;
    cursor: crosshair;
}

/* 警告ストライプ */
.warning-stripe {
    background: repeating-linear-gradient(
        45deg,
        #FF0,
        #FF0 10px,
        #000 10px,
        #000 20px
    );
    height: 10px;
}

/* ASCIIボーダー */
.ascii-border::before {
    content: '[===================================]';
    color: #FF0;
    font-family: monospace;
}
```

## 主要コンポーネント

### タイムラインブロック
90分のハッカソンなどの時間管理に使用
- 黄色の時間表示
- 赤い緊急マーカー
- モノスペースフォント

### ストーリーブロック
シナリオやケーススタディの表示
- ASCIIアート装飾
- 引用風デザイン
- タイプライター効果オプション

### データグリッド
評価基準やスコア表示
- 黄黒のストライプヘッダー
- ホバーでハイライト
- 警告色のアクセント

### サポートテーブル
リソースや支援情報の整理
- 技術的なモノスペース表示
- カテゴリー別色分け
- リンクは黄色でハイライト

## カスタマイズ

### カラーバリエーション
```yaml
# デフォルト（イエロー警告）
primary: #FFFF00
accent: #FF0000

# グリーンターミナル
primary: #00FF00
accent: #00FFFF

# レッドアラート
primary: #FF0000
accent: #FF00FF
```

### フォント変更
```css
/* オプション1: よりテクニカル */
font-family: 'Fira Code', 'Courier New', monospace;

/* オプション2: より工業的 */
font-family: 'Oswald', 'Arial Black', sans-serif;

/* オプション3: サイバーパンク */
font-family: 'Orbitron', 'Bebas Neue', sans-serif;
```

## ベストプラクティス

### DO ✓
- 警告色は重要な情報にのみ使用
- ASCIIアートは節度を持って配置
- モバイルでも読みやすさを確保
- アニメーションは目的を持って使用

### DON'T ✗
- 警告色の乱用（目が疲れる）
- 過度なグリッチエフェクト
- 読みにくいフォントサイズ
- アクセシビリティの無視

## ブラウザサポート
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## ライセンス
MIT License - 自由に使用・改変可能

## クレジット
Inspired by:
- 工業現場の安全標識
- サイバーパンク映画のUI
- ハッカーターミナル
- 90年代のハッキングカルチャー