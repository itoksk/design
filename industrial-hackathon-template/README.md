# 🏭 Industrial Hackathon Website Template

クリエイティブ・コレクティブ向けの**ブルータリズム×インダストリアル**デザインテンプレート

## 概要

このテンプレートは、AIが生成しがちな「ありきたりなデザイン」を徹底的に排除し、アンダーグラウンド・カルチャーのエッジの効いた美しさを表現した独創的なWebサイトを作成するためのものです。

### 特徴
- ❌ AIっぽさゼロ（グラデーション、角丸、パステルカラー禁止）
- ✅ ブルータリズムデザイン（ハードシャドウ、直角、高コントラスト）
- 🏭 インダストリアルテーマ（警告色、ハザードストライプ、グリッチエフェクト）

## クイックスタート

### 方法1: AIに生成させる

1. `prompts.md`を開く
2. マスタープロンプトをコピー
3. ChatGPT/Claude等に貼り付け
4. 生成されたHTMLを保存

```bash
# 例
cat prompts.md
# マスタープロンプトをコピーしてAIに投げる
```

### 方法2: テンプレートから構築

1. `theme.json`の設定を確認
2. `config.yaml`でコンテンツを定義
3. `design-system.md`のルールに従って実装

## ファイル構成

```
industrial-hackathon-template/
├── README.md                # このファイル
├── design-system.md         # デザインシステム仕様書
├── prompts.md              # AI生成用プロンプト集
├── config.yaml             # サイト設定ファイル
├── theme.json              # テーマ設定（詳細）
└── examples/               # 実装例（オプション）
```

## 各ファイルの役割

### 📐 design-system.md
デザインの完全仕様書。カラーパレット、タイポグラフィ、コンポーネント、禁止事項などを詳細に記載。

### 💬 prompts.md
AIにWebサイトを生成させるための詳細なプロンプト集。セクション別、コンポーネント別に整理。

### ⚙️ config.yaml
サイトの構成情報を構造化。色、フォント、レイアウト、コンテンツを定義。

### 🎨 theme.json
より詳細なテーマ設定。JSONフォーマットでプログラマティックに利用可能。

## 使用方法

### 1. AI生成の場合

```markdown
# prompts.mdからマスタープロンプトをコピー
# 以下を追加してカスタマイズ

「ストーリーは全文載せてください」
「もっとブルータリズムを強調して」
「警告色をもっと目立たせて」
```

### 2. 手動実装の場合

```html
<!DOCTYPE html>
<html lang="ja">
<head>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* design-system.mdのカスタムCSSを貼り付け */
        .brutalist-box {
            background: #1a1a1a;
            border: 4px solid #fbbf24;
            box-shadow: 8px 8px 0 #000;
        }
    </style>
</head>
<body>
    <!-- config.yamlの構成に従って実装 -->
</body>
</html>
```

## デザインルール

### ✅ 必須要素
- 黒背景（#0a0a0a）
- アンバー色のアクセント（#fbbf24）
- Bebas Neue / Oswaldフォント
- ハードシャドウ
- 直角・鋭角のみ

### ❌ 禁止事項
- グラデーション
- 角丸（border-radius）
- ソフトシャドウ
- パステルカラー
- 絵文字の多用
- スムーズなアニメーション

## カスタマイズ

### カラー変更
`theme.json`の`colors.palette`を編集：
```json
"primary": {
    "black": "#0a0a0a",    // ベース背景
    "amber-400": "#fbbf24", // アクセント色（変更可）
    "white": "#ffffff"
}
```

### セクション追加
`config.yaml`の`sections`に追加：
```yaml
sections:
  custom_section:
    title: "新しいセクション"
    style: "brutalist_box"
```

## トラブルシューティング

### Q: AIが角丸やグラデーションを生成してしまう
A: プロンプトに以下を追加：
```
「角丸は絶対に使わないで」
「グラデーションは禁止、単色のみ」
「もっと無骨に、工業的に」
```

### Q: デザインが整いすぎている
A: ボックスの傾きを追加：
```css
transform: rotate(1deg);  /* 微妙に傾ける */
transform: rotate(-1deg); /* 逆方向 */
```

### Q: 文字が読みにくい
A: コントラストを確認：
- 黒背景には白文字
- アンバー色は太字で使用
- 文字サイズは最小でも`text-sm`

## 実装例

完成例は親ディレクトリの`index.html`を参照：
```bash
open ../index.html
```

## 応用例

このテンプレートは以下の用途に最適：
- 🏭 工業系ハッカソン
- ⚙️ エンジニアリングイベント
- 🔧 技術ワークショップ
- 🎯 実践的教育プログラム

## ライセンス

MIT License - 自由に使用・改変可能

## コントリビューション

改善案やバグ報告は大歓迎です。
特に以下の点での貢献を求めています：
- より「非AI的」なデザイン要素
- 工業テーマの強化
- アクセシビリティの向上

## 参考資料

- [Brutalist Web Design](https://brutalistwebsites.com/)
- [Industrial Design Principles](https://www.industrialdesign.com/)
- [Tailwind CSS Documentation](https://tailwindcss.com/)

---

**Remember**: AIっぽさを徹底排除。限界を超えた独創性を追求。