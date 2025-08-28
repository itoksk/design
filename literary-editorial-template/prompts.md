# Literary Editorial Style AI Prompts
# 文芸誌スタイル AI生成プロンプト集

## 基本構造生成プロンプト

### 初期HTML生成
```
文芸誌スタイルのエディトリアルデザインWebページを作成してください。

デザイン要件：
- カラーパレット: インク色 (#0A0E27), 紙色 (#FEFEF8), 電気的な水色 (#00F0FF)
- フォント: 'Zen Kaku Gothic New' (メイン), 'Space Grotesk' (アクセント), 'Bebas Neue' (見出し)
- レイアウト: 創作ポートフォリオ向けの洗練されたデザイン
- 紙の質感を演出する背景パターン

必須コンポーネント：
1. 固定ナビゲーション（半透明白背景、下線アニメーション）
2. ヒーローセクション（巨大タイトル、回転ラベル）
3. 番号付きカード（01, 02, 03...、白黒反転ホバー）
4. セクション区切り（大きな薄い番号）
5. 紙質感の背景エフェクト

出力：
- 完全に動作するHTML（インラインCSS含む）
- レスポンシブ対応
- アクセシビリティ配慮
```

### レイアウトパターン生成

#### 文芸誌風ナビゲーション
```
文芸誌スタイルの固定ナビゲーションを作成してください。

仕様：
- 背景: rgba(254, 254, 248, 0.95) 半透明白
- ブラー効果: backdrop-filter: blur(10px)
- 下線アニメーション: ホバー時に電気的な水色で表示
- フォント: 'Zen Kaku Gothic New' メイン、'Space Grotesk' アクセント
- レスポンシブ: 768px以下でメニュー非表示

実装例：
<nav class="literary-nav">
  <div class="nav-title">Digital Arts Magazine</div>
  <div class="nav-menu">
    <a href="#">Features</a>
    <a href="#">Portfolio</a>
    <a href="#">About</a>
  </div>
</nav>
```

#### 番号付きカードシステム
```
文芸誌スタイルの番号付きカードを作成してください。

カード仕様：
- 背景: 白 (#FEFEF8)
- 枠線: 2px solid 黒 (#0A0E27)
- 影: ::before疑似要素で黒い影（4px offset）
- 番号: 40x40px 正方形、電気的な水色背景 (#00F0FF)
- ホバー効果: 白黒反転 + 左上移動 (-4px, -4px)

番号スタイル：
- フォント: 'Space Grotesk' monospace
- 形式: 01, 02, 03, 04...
- 太さ: font-weight: 700

HTML構造：
<div class="literary-card">
  <div class="card-number">01</div>
  <h3 class="card-title">タイトル</h3>
  <p class="card-description">説明文</p>
</div>
```

### コンテンツパターン生成

#### ヒーローセクション
```
クリエイティブ・ポートフォリオ向けのヒーローセクションを作成してください。

レイアウト仕様：
- 高さ: min-height: 100vh
- 配置: 縦積み中央揃え
- 背景: 紙質感パターン付き

要素構成：
1. 回転ラベル（transform: rotate(-1deg)）
   - 背景: 黒 (#0A0E27)
   - 文字: 白
   - 内容: "CREATIVE SHOWCASE"

2. メインタイトル
   - サイズ: clamp(3rem, 8vw, 6rem)
   - フォント: 'Zen Kaku Gothic New'
   - 行間: line-height: 0.9

3. サブタイトル（span要素）
   - 色: 電気的な水色 (#00F0FF)
   - サイズ: 0.7em

4. 説明文
   - サイズ: 1.25rem
   - 最大幅: 800px
   - 行間: 1.8
```

#### フェーズカードシステム
```
プロジェクトフェーズを示すカードシステムを作成してください。

デザイン仕様：
- 区切り線: 点線の下線（repeating background-image使用）
- 番号: 巨大な薄い数字（5rem, opacity: 0.2）
- 色: 紫 (#7C3AED)
- レイアウト: フレックス（番号＋タイトル）

実装例：
<div class="phase-card">
  <div class="phase-header">
    <div class="phase-number">01</div>
    <div class="phase-title">Concept Phase</div>
  </div>
  <p class="phase-description">Creative ideation and visual exploration</p>
</div>

CSS実装：
- 番号フォント: 'Space Grotesk'
- タイトルフォント: 'Zen Kaku Gothic New'
- 下線パターン: 20px間隔の点線
```

### インタラクション生成

#### ホバーエフェクト
```
文芸誌スタイルのホバーエフェクトを実装してください。

カードホバー：
- 背景: 白 → 黒に反転
- 文字色: 黒 → 白に反転
- 移動: transform: translate(-4px, -4px)
- 影の拡大: top: 4px → 8px, left: 4px → 8px
- 番号背景: 水色 → 白に反転、文字は黒に

ナビゲーションホバー：
- 下線: width: 0 → 100%
- 色: 電気的な水色 (#00F0FF)
- アニメーション: 0.3s ease

テーブル行ホバー：
- 背景: rgba(0, 240, 255, 0.05) 薄い水色
```

#### 紙質感エフェクト
```
印刷物の紙質感を演出する背景エフェクトを追加してください。

実装方法：
body::before疑似要素を使用して全画面にオーバーレイ

背景パターン：
repeating-linear-gradient(
  90deg,
  transparent,
  transparent 2px,
  rgba(10, 14, 39, 0.01) 2px,
  rgba(10, 14, 39, 0.01) 4px
)

設定：
- position: fixed
- z-index: 1
- pointer-events: none
- width/height: 100%
```

### テーブル・リストパターン

#### スケジュールテーブル
```
文芸誌スタイルのプロジェクト・タイムラインテーブルを作成してください。

仕様：
- ヘッダー: 黒背景 (#0A0E27) + 白文字
- セル: 1.25rem 1rem パディング
- ホバー: 薄い水色背景 rgba(0,240,255,0.05)
- セッション番号: 'Space Grotesk' フォント、水色 (#00F0FF)
- border-collapse: separate
- border-spacing: 0

HTML構造：
<table class="schedule-table">
  <thead>
    <tr>
      <th>Phase</th>
      <th>Focus</th>
      <th>Output</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="schedule-session">01</td>
      <td>Discovery</td>
      <td>Visual research and mood boards</td>
    </tr>
  </tbody>
</table>
```

### レスポンシブ対応プロンプト

#### モバイル最適化
```
文芸誌スタイルのモバイル対応を実装してください。

ブレークポイント: 768px以下

調整内容：
1. ナビゲーション
   - メニュー非表示: .nav-menu { display: none; }

2. グリッドレイアウト
   - 多列 → 単列: grid-template-columns: 1fr

3. タイポグラフィ
   - ヒーロータイトル: 最小サイズ制限
   - clamp(2rem, 8vw, 4rem)

4. フェーズカード
   - フレックス方向: column
   - 番号サイズ: 5rem → 3rem

5. カード
   - パディング: 2rem → 1.5rem

Media Query実装：
@media (max-width: 768px) {
  /* モバイル調整 */
}
```

## 完全なページ生成プロンプト

### クリエイティブ・ポートフォリオページ
```
以下の要素を含む文芸誌スタイルのクリエイティブ・ポートフォリオページを作成してください：

構造：
1. 固定ナビゲーション（半透明、下線アニメーション）
2. ヒーローセクション（巨大タイトル、回転ラベル、説明文）
3. 作品概要（3列グリッド、番号付きカード）
4. プロジェクト構成（フェーズカード、巨大薄い番号）
5. タイムラインテーブル（黒ヘッダー、ホバー効果）

デザインスタイル：
- カラー: インク (#0A0E27), 紙 (#FEFEF8), 水色 (#00F0FF)
- フォント: 'Zen Kaku Gothic New', 'Space Grotesk', 'Bebas Neue'
- 紙質感の背景パターン
- 番号システム: 01, 02, 03...

インタラクション：
- カードの白黒反転ホバー
- ナビゲーション下線アニメーション
- テーブル行のホバー効果
- 滑らかなトランジション (0.3s ease)

レスポンシブ：
- モバイル: 768px以下で単列レイアウト
- タブレット: 1024px以下で調整
- デスクトップ: 1400px最大幅

注意事項：
- 絵文字の使用は最小限
- 読みやすさ最優先
- アクセシビリティ配慮
- SEO対応のセマンティックHTML
```

### アートプロジェクトショーケースページ
```
文芸誌スタイルのアートプロジェクトショーケースページを作成してください：

必須セクション：
1. プロジェクトタイトル（巨大テキスト、サブタイトル付き）
2. コンセプト概要（番号付きカード3-4枚）
3. 制作プロセス（フェーズカード形式）
4. 成果物・ギャラリー（テーブルまたはグリッド）
5. インスピレーション・参考（リスト形式）

特殊要素：
- 回転した「CREATIVE PROJECT」ラベル
- 作品ビジュアル用のプレースホルダー
- インスピレーション引用ブロック（特別なスタイリング）
- 技法・素材説明システム

クリエイティブ要素：
- セクション番号システム (1., 1.1, 1.2...)
- 作品キャプション
- インスピレーションリンク
- コンセプトステートメント表示

同じデザインシステムを維持：
- 紙とインクの質感
- 番号付きカードシステム
- ホバー時の白黒反転
- 統一されたタイポグラフィ
```

## カスタマイズ用プロンプト

### カラー変更
```
文芸誌スタイルのカラーパレットをカスタマイズ：

代替カラーパレット：
1. 暖色系: インク(#2D1810), 紙(#FFF8F0), アクセント(#FF7A00)
2. 寒色系: インク(#0F1419), 紙(#F8FAFC), アクセント(#0EA5E9)  
3. モノトーン: インク(#1F2937), 紙(#F9FAFB), アクセント(#6B7280)

変更箇所：
- CSS変数の更新
- ホバー効果の色調整
- アクセント要素の色変更
```

### フォント変更
```
代替フォントの組み合わせ：

クラシック：
- メイン: 'Noto Serif JP'
- アクセント: 'JetBrains Mono'
- 見出し: 'Playfair Display'

モダン：
- メイン: 'Inter'
- アクセント: 'Fira Code'  
- 見出し: 'Poppins'

和風：
- メイン: 'Noto Sans JP'
- アクセント: 'Source Code Pro'
- 見出し: 'M PLUS Rounded 1c'
```