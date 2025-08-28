# Liquid Gradient Design Template

## 概要
流体的グラデーションとモーフィングシェイプを特徴とする次世代デザインシステム。静的なレイアウトの概念を破壊し、常に変化し続ける有機的なビジュアル体験を提供します。

## デザイン哲学

### コアコンセプト
- **Fluid Morphing**: 形状が呼吸するように変化し続ける
- **Gradient Mesh**: 複数のグラデーションが干渉し合う
- **Organic Motion**: 自然界の流体力学を模倣した動き
- **Depth Layering**: Z軸を活用した多層的な奥行き表現
- **Color Breathing**: 色彩が脈動するように変化

### 視覚的特徴
1. **メタボール効果**: 要素同士が磁石のように引き合い融合
2. **ノイズグラデーション**: Perlinノイズによる有機的な色の流れ
3. **グラスモーフィズム**: 曇りガラス効果とぼかしの多用
4. **3D変形**: CSS 3D transformによる空間的な歪み
5. **パーティクルフロー**: 背景に流れる光の粒子

## 使用シーン

### 最適な用途
- クリエイティブエージェンシーのポートフォリオ
- 音楽フェスティバル・アートイベント
- ファッションブランドのキャンペーンサイト
- インタラクティブアート展示
- 実験的なWebエクスペリエンス

### 避けるべき用途
- コーポレートサイト
- Eコマースプラットフォーム
- ニュース・情報サイト
- アクセシビリティ重視のサービス

## ディレクトリ構成

```
liquid-gradient-template/
├── README.md              # このファイル
├── design-system.yaml     # デザインシステム仕様
├── prompts.md            # AI生成用プロンプト
├── components.json       # コンポーネントライブラリ
├── theme.json           # テーマ設定
└── examples/            # 実装サンプル
    └── showcase.html    # デモページ
```

## クイックスタート

### 基本的な実装

```html
<!DOCTYPE html>
<html>
<head>
    <style>
        .liquid-container {
            background: linear-gradient(45deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #feca57 75%, #48c9b0 100%);
            background-size: 400% 400%;
            animation: gradient-shift 15s ease infinite;
        }
        
        @keyframes gradient-shift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }
        
        .morphing-blob {
            border-radius: 40% 60% 70% 30% / 40% 50% 60% 50%;
            animation: morph 8s ease-in-out infinite;
        }
        
        @keyframes morph {
            0%, 100% { border-radius: 40% 60% 70% 30% / 40% 50% 60% 50%; }
            50% { border-radius: 70% 30% 50% 50% / 30% 30% 70% 70%; }
        }
    </style>
</head>
<body>
    <!-- Your content here -->
</body>
</html>
```

## 主要コンポーネント

### Liquid Navigation
流体のように変形するナビゲーションバー
- マウス追従エフェクト
- メタボール融合アニメーション
- グラデーションの波紋効果

### Morphing Cards
形状が常に変化し続けるカードコンポーネント
- ランダムな border-radius アニメーション
- ホバー時の液体化エフェクト
- 深度を感じる多層シャドウ

### Particle Background
インタラクティブなパーティクル背景
- マウスに反応する粒子群
- 重力シミュレーション
- カラーフィールドの干渉

### Glassmorphic Panels
ガラスモーフィズムを極限まで追求したパネル
- 多重ブラー効果
- 屈折シミュレーション
- 虹色の光の反射

## カラーシステム

### グラデーションパレット
```css
/* Aurora Dreams */
background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #feca57 75%, #48c9b0 100%);

/* Neon Ocean */
background: linear-gradient(45deg, #00f2fe 0%, #4facfe 25%, #00f2fe 50%, #4facfe 75%, #00f2fe 100%);

/* Sunset Plasma */
background: linear-gradient(90deg, #fc466b 0%, #3f5efb 25%, #fc466b 50%, #3f5efb 75%, #fc466b 100%);
```

## アニメーション原則

### Ease Functions
```css
/* Organic Ease */
cubic-bezier(0.4, 0.0, 0.2, 1)

/* Liquid Flow */
cubic-bezier(0.25, 0.46, 0.45, 0.94)

/* Elastic Bounce */
cubic-bezier(0.68, -0.55, 0.265, 1.55)
```

### タイミング
- 基本周期: 8-15秒（ゆったりとした呼吸のリズム）
- インタラクション: 0.3-0.6秒
- マイクロアニメーション: 0.15-0.3秒

## ベストプラクティス

### DO ✓
- GPU加速を活用（transform, opacity）
- will-changeプロパティの適切な使用
- requestAnimationFrameでのスムーズな描画
- パフォーマンスモニタリング

### DON'T ✗
- 過度なアニメーション要素（最大5-7個）
- 高頻度のリペイント/リフロー
- モバイルでの複雑なフィルター効果
- アクセシビリティの完全無視

## ブラウザサポート
- Chrome 90+ (推奨)
- Firefox 88+
- Safari 14+
- Edge 90+

※ backdrop-filter, CSS Grid, Custom Properties 必須

## パフォーマンス最適化

- CSS containmentの活用
- Intersection Observerでの遅延アニメーション
- GPUレイヤーの分離
- 60fps維持のための最適化

## ライセンス
MIT License - 自由に使用・改変可能

## インスピレーション
- Liquid Crystal Display
- Lava Lamp Physics
- Northern Lights
- Deep Sea Bioluminescence
- Plasma Globe Effects