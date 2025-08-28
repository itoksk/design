# AI Prompts for Technology Editorial Template

This document contains specialized AI prompts for generating content using the Technology Magazine Style template.

## Core Implementation Prompt

### Japanese Version

```
以下の要件で、テクノロジー雑誌風のエディトリアルデザインのWebページを作成してください：

【デザインスタイル】
Technology Magazine Style（テクノロジー誌スタイル）を採用

【カラースキーム】
- プライマリ: Tech Blue (#0066CC), Tech Cyan (#00A8CC), Tech Dark (#001F3F)
- セカンダリ: Tech Gray (#2C3E50), Tech Light (#ECF0F1), Tech Accent (#FF6B35)
- 背景: Paper White (#F8F9FA)

【タイポグラフィ】
- メインフォント: 'Zen Kaku Gothic New', sans-serif（日本語）
- ディスプレイ: 'Bebas Neue', sans-serif（英語見出し）
- アクセント: 'Montserrat', sans-serif（サブタイトル）

【必須コンポーネント】
1. ヘッダー: グラデーション文字、クリップパス付きタグ
2. テックカード: アニメーショングラデーションバー、右スライドホバー
3. データパネル: 左上固定ラベル、大文字スタイル
4. プログレス: 六角形インジケーター、グラデーション接続線
5. スキルマトリックス: グリッド配置、ホバー時色反転&スケール

【特殊効果】
- ホバー効果: translateX(8px), scale(1.05), 色反転
- アニメーション: グラデーションスライド（3秒無限ループ）
- 背景パターン: 50pxグリッド、tech_blue 0.03透明度

【デザイン要素】
- サーキット基板風グリッドパターン
- 幾何学的クリップパス（多角形）
- データパネルスタイルカード
- 六角形プログレスインジケーター
- 斜めクリップパスの番号表示

【重要な注意点】
- 絵文字は最小限に抑える（AIっぽさを避ける）
- 番号は01, 02, 03形式を使用
- レスポンシブ対応必須（768px, 1024pxブレークポイント）
- アクセシビリティに配慮（十分なコントラスト比）
- テクノロジー感を演出する幾何学的要素を多用
```

### English Version

```
Create a technology magazine-style editorial webpage with the following requirements:

[Design Style]
Adopt Technology Magazine Style with circuit board and digital elements

[Color Scheme]
- Primary: Tech Blue (#0066CC), Tech Cyan (#00A8CC), Tech Dark (#001F3F)
- Secondary: Tech Gray (#2C3E50), Tech Light (#ECF0F1), Tech Accent (#FF6B35)
- Background: Paper White (#F8F9FA)

[Typography]
- Main Font: 'Zen Kaku Gothic New', sans-serif (Japanese text)
- Display: 'Bebas Neue', sans-serif (English headers)
- Accent: 'Montserrat', sans-serif (Subtitles)

[Required Components]
1. Header: Gradient text, clipped polygon tags
2. Tech Cards: Animated gradient top bar, right-slide hover
3. Data Panels: Fixed top-left labels, uppercase styling
4. Progress: Hexagonal indicators, gradient connection lines
5. Skill Matrix: Grid layout, hover color inversion & scale

[Special Effects]
- Hover effects: translateX(8px), scale(1.05), color inversion
- Animations: Gradient slide (3s infinite loop)
- Background pattern: 50px grid, tech_blue 0.03 opacity

[Design Elements]
- Circuit board-style grid patterns
- Geometric clip-paths (polygonal shapes)
- Data panel-style cards
- Hexagonal progress indicators
- Diagonal clip-path numbering

[Important Notes]
- Minimize emoji usage (avoid AI-like patterns)
- Use 01, 02, 03 numbering format
- Responsive design required (768px, 1024px breakpoints)
- Consider accessibility (sufficient contrast ratios)
- Emphasize technological feel with geometric elements
```

## Content Generation Prompts

### Tech Product/Service Content

```
Generate content for a tech product or startup using the tech editorial template. Include:

1. Product name with compelling tagline
2. 4-6 key features with:
   - Numbered cards (01, 02, 03...)
   - Feature highlight chips
   - Performance badges
   - Brief descriptions focusing on user benefits

3. Technology stack section with:
   - 6-9 technologies used in development
   - Modern frameworks (React, Node.js, Python, etc.)
   - Cloud platforms (AWS, Google Cloud, Azure, etc.)

4. Product benefits in data panel format
5. Target market and use case information

Content should be innovative, cutting-edge, and engaging for tech professionals and enthusiasts.
```

### Tech Event/Conference Content

```
Create a technology conference or event page with:

1. Event header with:
   - Event category tag
   - Main title in English (uppercase, tech style)
   - Subtitle with location/date
   - Brief engaging description

2. Event features as tech cards:
   - Keynote speakers
   - Innovation showcases
   - Networking opportunities
   - Demo sessions

3. Event information in overview cards:
   - Target attendees
   - Registration details
   - Venue capacity
   - Schedule duration

4. Technology focus areas in skill matrix
5. Event timeline with hexagonal indicators

Focus on innovation, networking, and knowledge sharing experiences.
```

### Product/Service Documentation

```
Design a technical product page featuring:

1. Product name with technology category tag
2. Key features as numbered tech cards
3. Technical specifications in data panels
4. Implementation timeline with progress indicators
5. Compatibility matrix showing supported platforms

Emphasize precision, reliability, and technical sophistication.
```

## Style-Specific Instructions

### Visual Hierarchy

- Use large section numbers (01, 02, 03) with low opacity
- Implement gradient text for main headlines
- Apply clip-path styling to badges and numbers
- Maintain consistent 24px spacing in grid layouts

### Interaction Design

- Cards should slide 8px right on hover
- Skill matrix cells invert colors and scale to 1.05x
- Progress indicators connect with animated gradient lines
- Subtle shadow effects enhance depth

### Responsive Behavior

- Single column layout below 768px
- Hexagonal progress becomes vertical stack on mobile
- Font sizes scale using clamp() functions
- Grid gaps reduce on smaller screens

### Content Tone

- Professional but approachable
- Technical accuracy without overwhelming jargon
- Focus on practical applications and real-world relevance
- Emphasize hands-on learning and experimentation

## Customization Prompts

### Color Variation

```
Adapt the tech editorial template for [SPECIFIC DOMAIN] with:
- Primary color adjusted to: [HEX COLOR]
- Accent color modified to: [HEX COLOR]
- Maintain tech aesthetic while reflecting [DOMAIN] characteristics
```

### Content Domain Adaptation

```
Modify the technology template for [SPECIFIC SUBJECT]:
- Adjust terminology for [SUBJECT] field
- Include relevant tools and platforms
- Adapt skill matrix to [SUBJECT] competencies
- Maintain geometric, technical visual language
```

These prompts ensure consistent application of the technology editorial style while allowing for content flexibility and domain-specific adaptations.