# Stadium Classic Design Prompts

## 基本プロンプト

### スタジアムレイアウト生成
```
Create a stadium-inspired layout with:
- Pure white (#FFFFFF) background as the base
- Stadium black (#0A0A0A) for strong contrast elements
- Crimson red (#DC143C) as accent color for CTAs and highlights
- Diagonal compositions creating dynamic movement
- Sharp geometric patterns suggesting tactical formations
- Bold typography with uppercase letters
- High contrast between elements
- Minimal color palette (only white, black, red)
- Strong grid system with asymmetric balance
```

### ヒーローセクション
```
Design a hero section featuring:
- Full-width diagonal split background at 135deg angle
- Rotated -15deg for dynamic effect
- Pure white (#FFFFFF) and stadium black (#0A0A0A) split at 49%/51%
- Bold display typography (Bebas Neue or similar)
- Title split across white/black with mix-blend-mode: difference
- Crimson red (#DC143C) accent text with pulse animation
- Score counter in top-right with polygon clip-path
- Mobile-responsive diagonal adjustment
```

### スコアボードコンポーネント
```
Create a scoreboard display with:
- Black background panel
- White text for team names
- Crimson red for current score
- Teko or condensed font for numbers
- Live pulse animation for active game
- Timer/clock display
- Statistics grid below scores
- Responsive scaling for mobile
Format:
┌────────────────────────┐
│   HOME  3 : 2  AWAY    │
│      FULL TIME         │
└────────────────────────┘
```

### チームカードグリッド
```
Design team/player cards with:
- White background with clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%)
- Hover: clip-path transitions to full rectangle
- Player number in Teko font, 8rem size, #0A0A0A color
- Hover: number transitions to crimson red (#DC143C)
- Transform: translateY(-10px) on hover
- Name in 1.5rem bold uppercase
- Position in silver (#C0C0C0) uppercase
- Grid layout with auto-fit, minmax(300px, 1fr)
```

## ナビゲーション・ヘッダー

### 固定ナビゲーション
```
Create a fixed navigation header:
- White background with black bottom border
- Logo in black on left
- Menu items in uppercase, black text
- Active item: crimson red underline (3px)
- Hover: text transitions to crimson
- Hamburger menu: three black lines
- Scroll: background switches to black, text to white
- Sticky positioning with shadow on scroll
```

### モバイルメニュー
```
Design mobile navigation menu:
- Full screen overlay (95% black opacity)
- White text on black background
- Crimson red accent for active page
- Slide-in from right animation
- X close button in top right
- Menu items stacked vertically
- Social icons at bottom
```

## コンテンツセクション

### パワーグリッド
```
Create asymmetric power grid:
- Grid template: 2fr 1fr 1fr columns
- 2px gap with black (#0A0A0A) background
- Transform: skewY(-2deg) for dynamic angle
- White (#FFFFFF) grid items with 40px padding
- First item spans 2 rows, fourth spans 2 columns
- Hover: background to crimson, scale(1.02)
- Grid numbers in top-right, 5rem Teko font
- Opacity 0.3, transitions to 0.2 on hover
```

### ニュースカード
```
Design news/blog cards:
- White card with black border
- Category tag in crimson red
- Black headline text
- Hover: slight scale and shadow
- Date in gray (#808080)
- Read more arrow in red
- Image with diagonal overlay option
```

### CTAセクション
```
Create call-to-action section with moving stripes:
- Background: repeating-linear-gradient(45deg, transparent 0, transparent 50px, #F5F5F5 50px, #F5F5F5 100px)
- Animation: translateX movement over 20s linear infinite
- Crimson red (#DC143C) button, 20px 60px padding
- Button with ::before pseudo-element slide effect
- Black background slides in from left on hover
- Transform: scale(1.05) on hover
- Bold Bebas Neue heading, 4rem size
- Centered content, max-width 800px
```

## インタラクション要素

### ボタンスタイル
```
Design button variations:

Primary (Crimson):
- Background: #DC143C
- Text: white, uppercase, bold
- Hover: darken to #CC1100
- Padding: 12px 32px
- No border

Secondary (White):
- Background: white
- Text: black
- Border: 2px solid black
- Hover: invert colors

Ghost (Transparent):
- Background: transparent
- Border: 2px solid current
- Hover: fill with color
```

### フォーム要素
```
Style form inputs and controls:
- White background
- 2px black border
- Focus: crimson red border
- Error state: blood orange (#CC1100)
- Labels in bold black
- Placeholder in gray
- Checkbox: black border, red check
- Radio: black circle, red dot
```

### ホバーエフェクト
```
Implement hover interactions:
- Color inversion (black ↔ white)
- Crimson red glow/highlight
- Scale up 1.05
- Diagonal slide reveal
- Shadow appearance
- Border color change to red
- Image colorization
- Text underline slide-in
```

## 特殊効果・パターン

### 対角線パターン
```
Create diagonal stripe patterns:
- 45-degree angle
- Black and white alternating
- 10-20px stripe width
- Optional red accent stripe
- Use as background or mask
- CSS gradient or SVG pattern
- Animated sliding option
```

### ノイズテクスチャ
```
Add subtle texture overlays:
- Light grain/noise at 2% opacity
- Multiply blend mode
- Stadium atmosphere feel
- Paper-like texture option
- Consistent across sections
```

### カウンターアニメーション
```
Implement number animations:
- Count up from 0 to target
- Duration based on value
- Ease-out timing
- Thousand separators
- Optional + or % suffix
- Trigger on scroll into view
- Crimson red for increases
```

## レイアウトパターン

### 対角線分割
```
Create diagonal split layouts:
- 45-degree angle division
- White and black sections
- Content aligned to angle
- Text remains horizontal
- Mobile: switch to horizontal
- Smooth edge or sharp
- Parallax offset option
```

### グリッドシステム
```
Implement 12-column grid:
- 24px gutters
- Max width 1440px
- Flexible breakpoints
- Asymmetric layouts allowed
- Black borders for structure
- White space emphasis
```

### カードグリッド
```
Design card-based layouts:
- 3 columns desktop
- 2 columns tablet  
- 1 column mobile
- Equal height cards
- Black borders
- White backgrounds
- Red accent elements
```

## モバイル最適化

### レスポンシブ調整
```
Adapt for mobile devices:
- Stack diagonal sections
- Reduce font sizes (0.9x)
- Increase tap targets (44px min)
- Simplify animations
- Hide decorative elements
- Vertical navigation
- Full-width buttons
```

### タッチインタラクション
```
Optimize for touch:
- Remove hover effects
- Add touch feedback
- Swipe gestures for galleries
- Larger click areas
- Bottom sheet modals
- Thumb-friendly navigation
```

## パフォーマンス最適化

### 画像処理
```
Optimize visual assets:
- Monochrome images where possible
- WebP format with fallbacks
- Lazy loading implementation
- Responsive image sizes
- CSS shapes over images
- SVG for icons and logos
```

### アニメーション
```
Optimize animations:
- CSS transforms only
- Will-change property
- 60fps target
- Reduce on mobile
- Respect prefers-reduced-motion
- GPU acceleration
```

## アクセシビリティ

### コントラスト確保
```
Ensure WCAG AAA compliance:
- Black on white: 21:1 ratio
- White on black: 21:1 ratio
- White on crimson: 8.5:1 ratio
- Never red on black
- Test all combinations
```

### フォーカス表示
```
Implement focus indicators:
- 3px crimson red outline
- 2px offset from element
- Visible on all backgrounds
- Custom for each component
- Keyboard navigation friendly
```

## 使用上の注意

このデザインシステムは極めて限定的な色使いと
強いコントラストが特徴です。
ブランドの力強さと伝統を表現する際に最適ですが、
すべてのコンテキストに適しているわけではありません。