# Design Templates Collection

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

独創的でAIっぽくないデザインテンプレートのコレクションです。各テンプレートは特定の用途に最適化され、詳細な設計仕様と実装ガイドを含んでいます。

## 📁 テンプレート一覧

### 1. [Brutalist Design Template](./brutalist-design-template/)
**ブルータリズムWebデザインテンプレート**
- 🎨 大胆で実験的なデザインシステム
- 📐 非対称レイアウト、生々しい素材感
- ⚡ 極端なサイズとコントラスト
- 🎯 芸術性重視のプロジェクト向け

### 2. [Literary Editorial Template](./literary-editorial-template/)
**文芸誌風エディトリアルデザイン**
- 📚 紙の質感とインクの温かみ
- 📖 独立系出版・アートマガジン向け
- 🔢 番号付きカード（01, 02, 03...）
- 🎭 ホバー時の白黒反転効果

### 3. [Tech Editorial Template](./tech-editorial-template/)
**テクノロジー誌風デザイン**
- 💻 サーキット基板パターン
- 🔷 六角形プログレスインジケーター
- 📊 データパネル風カード
- ⚡ アニメーショングラデーション

### 4. [Industrial Cyberpunk Template](./industrial-cyberpunk-template/)
**サイバーパンク×インダストリアルデザイン**
- ⚠️ 警告色とターミナルグリーン
- 💀 グリッチエフェクトとASCIIアート
- 🔌 サーキット基板風の装飾
- 🎮 アンダーグラウンドな雰囲気

### 5. [Industrial Hackathon Template](./industrial-hackathon-template/)
**クリエイティブコレクティブ向けデザイン**
- 🏭 ブルータリズム×インダストリアル
- ⚠️ 警告色、ハザードストライプ、グリッチエフェクト
- 🔧 工場現場の無骨さと力強さを表現
- ❌ AIっぽさを徹底排除

## 🚀 クイックスタート

### 基本的な使用方法

1. 使用したいテンプレートのディレクトリを選択
2. 各テンプレートのREADME.mdで詳細を確認
3. 設定ファイル（.yaml/.json）でカスタマイズ
4. プロンプトファイル（.md）を使用してAI生成、または手動実装

```bash
# テンプレートをクローン
git clone https://github.com/[your-username]/design-templates.git
cd design-templates

# 特定のテンプレートに移動
cd brutalist-design-template/
# または
cd literary-editorial-template/
# または
cd tech-editorial-template/
# または
cd industrial-cyberpunk-template/
# または
cd industrial-hackathon-template/

# 詳細を確認
cat README.md
```

## 📋 各テンプレートの構成

すべてのテンプレートには以下が含まれています：

- **README.md** - テンプレートの概要と使用方法
- **Design System** - デザイン仕様書（.yaml/.md形式）
- **Prompts** - AI生成用のプロンプト集
- **Components** - 再利用可能なコンポーネント定義
- **Examples** - 実装サンプル（一部テンプレート）

## 🎨 デザイン哲学

このコレクションは以下の原則に基づいています：

1. **独創性** - AIが生成しがちな一般的なデザインを避ける
2. **実用性** - 実際のプロジェクトで使用可能
3. **カスタマイズ性** - 簡単に調整・拡張可能
4. **完全性** - 実装に必要なすべての情報を含む

## 🛠️ カスタマイズ

各テンプレートは以下の方法でカスタマイズできます：

### カラーパレット変更
各テンプレートの設定ファイルで色を調整：
```yaml
colors:
  primary: "#your-color"
  secondary: "#your-color"
```

### フォント変更
```css
font-family: 'Your Font', fallback-font, sans-serif;
```

### レイアウト調整
各テンプレートのグリッドシステムとブレークポイントを活用

## 📱 レスポンシブ対応

すべてのテンプレートは以下のブレークポイントに対応：
- Mobile: < 768px
- Tablet: 768px - 1024px
- Desktop: > 1024px

## ⚠️ 注意事項

### 推奨事項
- ✅ デザインの一貫性を保つ
- ✅ アクセシビリティへの配慮
- ✅ パフォーマンスを意識した実装
- ✅ 各テンプレートの設計思想を理解して使用

### 避けるべきこと
- ❌ テンプレートの混在使用（統一感が失われる）
- ❌ 過度な装飾の追加
- ❌ デザインシステムを無視した変更
- ❌ AIっぽい一般的なデザインへの改変

## 🤝 コントリビューション

新しいテンプレートの追加や既存テンプレートの改善を歓迎します：

1. このリポジトリをフォーク
2. フィーチャーブランチを作成 (`git checkout -b feature/NewTemplate`)
3. 変更をコミット (`git commit -m 'Add new template'`)
4. ブランチをプッシュ (`git push origin feature/NewTemplate`)
5. プルリクエストを作成

### コントリビューションガイドライン

- 各テンプレートは独自のディレクトリに配置
- README.md、デザインシステム、プロンプトファイルを必ず含める
- AIっぽくない独創的なデザインを心がける
- 実装可能で実用的なものにする

## 📄 ライセンス

MIT License - 詳細は[LICENSE](./LICENSE)ファイルを参照してください。

商用利用も可能ですが、適切なクレジット表記をお願いします。

## 📞 サポート

質問や問題がある場合：
- 各テンプレートのREADMEを確認
- [Issues](https://github.com/[your-username]/design-templates/issues)で報告
- プルリクエストで改善提案

## 🌟 謝辞

これらのテンプレートは、様々なデザイントレンドと実践的なニーズから生まれました。
すべてのコントリビューターに感謝します。

---

**Made with ❤️ for unique and creative web design**