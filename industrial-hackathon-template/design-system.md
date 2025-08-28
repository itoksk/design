# Industrial Hackathon Design System

## デザインコンセプト

### 基本理念
**ブルータリズム × インダストリアル**
- AIらしさを徹底排除
- 工場現場の無骨さと力強さを表現
- 警告色とモノトーンの対比
- アシンメトリーと歪みによる動的表現

## カラーパレット

### Primary Colors
```yaml
black: #0a0a0a        # 背景のベースカラー
amber-400: #fbbf24    # 警告色・アクセント
gray-900: #1a1a1a     # セカンダリ背景
white: #ffffff        # テキスト
```

### Secondary Colors
```yaml
gray-700: #374151     # ボーダー
gray-600: #4b5556     # 補助テキスト  
gray-400: #9ca3af     # 説明テキスト
red-500: #ef4444      # エラー・警告
```

## タイポグラフィ

### フォントファミリー
```css
/* インダストリアル系フォント */
.bebas {
  font-family: 'Bebas Neue', cursive;  /* 見出し用 */
}

.oswald {
  font-family: 'Oswald', sans-serif;   /* サブ見出し用 */
}

/* 日本語 */
body {
  font-family: 'Noto Sans JP', sans-serif;
}
```

### フォントサイズ規則
- Hero Title: `text-9xl` (128px)
- Section Title: `text-6xl` ~ `text-7xl` 
- Subsection: `text-4xl`
- Body: `text-sm` ~ `text-base`

## 特徴的なビジュアル要素

### 1. ハザードストライプ（警告帯）
```css
.hazard-stripe {
  background: repeating-linear-gradient(
    45deg,
    #fbbf24,
    #fbbf24 10px,
    #1f2937 10px,
    #1f2937 20px
  );
}
```
**使用場所**: セクション区切り、重要な告知

### 2. グリッチエフェクト
```css
.glitch {
  text-shadow: 
    0.05em 0 0 rgba(255, 0, 0, .75),
    -0.025em -0.05em 0 rgba(0, 255, 0, .75),
    0.025em 0.05em 0 rgba(0, 0, 255, .75);
  animation: glitch 500ms infinite;
}
```
**使用場所**: キーワード、インパクトが必要な箇所

### 3. ブルータリストボックス
```css
.brutalist-box {
  background: #1a1a1a;
  border: 4px solid #fbbf24;
  box-shadow: 8px 8px 0 #000;
}
```
**使用場所**: コンテンツカード、重要情報

### 4. オフセットボックス
```css
.offset-box::after {
  content: '';
  position: absolute;
  top: 4px;
  left: 4px;
  right: -4px;
  bottom: -4px;
  background: #fbbf24;
  z-index: -1;
}
```
**使用場所**: 小さな情報ブロック、リスト

### 5. インダストリアルグリッド
```css
.industrial-grid {
  background-image: 
    linear-gradient(rgba(59, 130, 246, 0.1) 1px, transparent 1px),
    linear-gradient(90deg, rgba(59, 130, 246, 0.1) 1px, transparent 1px);
  background-size: 50px 50px;
}
```
**使用場所**: 背景パターン

### 6. 傾斜・歪み
```css
transform: rotate(1deg);   /* 微妙な傾き */
transform: rotate(-1deg);  /* 逆傾き */
transform: skewX(-2deg);   /* X軸歪み */
```
**使用場所**: コンテンツボックスに動きを与える

## レイアウト原則

### 1. アシンメトリー
- 完全な対称を避ける
- ボックスを交互に傾ける（1deg, -1deg）
- 不規則な配置で緊張感を演出

### 2. 大胆な余白
- セクション間: `py-20`
- コンテンツ間: `mb-16`
- 内部パディング: `p-8`

### 3. 強いコントラスト
- 黒背景 + 白文字
- アンバー色のアクセント
- 太いボーダー（4px）

## コンポーネントパターン

### タイムラインアイテム
```html
<div class="timeline-item bg-gray-900 p-8 mb-8">
  <div class="bebas text-5xl text-amber-400">00-10</div>
  <h4 class="text-2xl font-bold mt-2">タイトル</h4>
  <!-- コンテンツ -->
</div>
```

### ストーリーカード
```html
<div class="brutalist-box p-8 transform rotate-1">
  <div class="text-amber-400 bebas text-4xl">時刻</div>
  <h3 class="text-2xl font-bold">見出し</h3>
  <div class="text-gray-300">本文</div>
</div>
```

### 警告・注意喚起
```html
<div class="bg-red-900/20 border-2 border-red-500 p-8">
  <p class="text-red-400 font-bold">警告タイトル</p>
  <!-- 内容 -->
</div>
```

## アニメーション

### 使用する効果
1. **グリッチ**: キーワードの強調
2. **ホバー無し**: 意図的に静的
3. **スクロール連動無し**: シンプルさ重視

## 禁止事項（AIっぽさの排除）

### 使わないもの
- ❌ グラデーション背景（単色のみ）
- ❌ 角丸（border-radius）
- ❌ 影のぼかし（シャープな影のみ）
- ❌ パステルカラー
- ❌ 絵文字の多用
- ❌ カード型の整然としたグリッド
- ❌ スムーズなトランジション

### 代わりに使うもの
- ✅ ソリッドカラー
- ✅ 直角・鋭角
- ✅ ハードシャドウ
- ✅ 高コントラスト色
- ✅ テキストベース
- ✅ 不規則な配置
- ✅ 即座の状態変化

## レスポンシブ対応

### ブレークポイント
- Mobile: デフォルト
- Tablet: `md:` (768px~)
- Desktop: `lg:` (1024px~)

### モバイル優先
- 基本的に1カラム
- タブレット以上で2カラム、3カラム展開
- テキストサイズは相対指定

## 実装のポイント

1. **Tailwind CDN使用**
   ```html
   <script src="https://cdn.tailwindcss.com"></script>
   ```

2. **カスタムフォント読み込み**
   ```css
   @import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Oswald:wght@200;400;700&family=Noto+Sans+JP:wght@300;400;700;900&display=swap');
   ```

3. **ダークモード前提**
   - 常に黒背景
   - 明るい色は警告・注意喚起のみ

## 使用例

このデザインシステムは以下の場面で効果的：
- 工業・製造業関連のハッカソン
- 技術系イベント
- エンジニアリング教育
- 実践的なワークショップ

## メンテナンス

定期的に以下を確認：
1. フォントCDNの可用性
2. Tailwind CSSのバージョン
3. ブラウザ互換性（Chrome, Firefox, Safari）