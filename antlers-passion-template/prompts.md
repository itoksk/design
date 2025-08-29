# Antlers Passion Design Prompts

## 基本プロンプト

### 情熱的レイアウト生成
```
Create a passionate layout with:
- Antlers red (#B01224) as primary passion color
- Kashima navy (#001E62) as deep ocean color
- Wave-like transitions between sections
- Rose petal decorative elements
- Gradient flows from red to navy
- Curved and flowing compositions
- Warm-to-cool color transitions
- Dynamic movement and energy
- Balanced asymmetry with organic shapes
```

### ヒーローセクション
```
Design a hero section featuring:
- Gradient background from antlers red to sunset orange
- Wave divider transitioning to navy section
- Floating rose petals animation
- Bold Oswald or similar display typography
- Pulsing CTA button with ripple effect
- Parallax ocean waves in background
- Mobile-responsive wave adjustments
- Passion meter or counter display
```

### 波形分割レイアウト
```
Create wave-split layout with:
- SVG wave path between red and navy sections
- Animated wave motion (3s ease-in-out)
- 30px amplitude, 200px frequency
- Top section: gradient red background
- Bottom section: deep navy background
- Content floats above wave layer
- Responsive wave height adjustment
Format:
╔════════════════════════╗
║     ANTLERS RED        ║
║    ∿∿∿∿∿∿∿∿∿∿∿∿∿∿     ║
║     KASHIMA NAVY       ║
╚════════════════════════╝
```

### ローズカードグリッド
```
Design rose-themed cards with:
- White background, pink rose border
- Petal decoration in top-right corner
- Hover: border transitions to crimson
- Bloom animation on hover
- Gradient accents from red to pink
- Soft shadows with red glow
- Card content with elegant serif fonts
- Responsive grid layout
```

## ナビゲーション・ヘッダー

### オーシャンナビゲーション
```
Create ocean-themed navigation:
- Semi-transparent navy background (0.95 opacity)
- Backdrop blur effect (10px)
- White text with red hover state
- Wave underline animation on active
- Sticky positioning with transition
- Scroll: background becomes solid
- Mobile: slide-in from side with wave transition
- Logo with passion gradient
```

### 波形アンダーライン
```
Design wave underline for links:
- Start: scaleX(0) from left
- Hover: scaleX(1) with wave motion
- Color: antlers red (#B01224)
- Height: 3px with curved path
- Timing: cubic-bezier(0.4, 0, 0.2, 1)
- Transform origin: left center
```

## コンテンツセクション

### 情熱メーター表示
```
Create passion meter display:
- Gray background track (#F5F5F5)
- Gradient fill: red to orange
- Animated fill on scroll
- Pulse effect at leading edge
- Percentage or value display
- 12px height, rounded corners
- Optional glow effect
- Responsive sizing
```

### フローティングカード
```
Design floating glass cards:
- Semi-transparent white (0.95 opacity)
- Backdrop blur (10px)
- Thin red border (0.2 opacity)
- Soft navy shadow
- Hover: slight elevation
- Parallax movement option
- Content with mixed typography
```

### 花びらアニメーション
```
Create petal fall animation:
- Random starting positions
- Fall duration: 10s
- Rotation during fall (360deg)
- Gradient colors: crimson to pink
- Opacity fade at bottom
- Multiple petal shapes
- Pointer-events: none
- Z-index layering
```

## インタラクション要素

### パッションボタン
```
Design passion CTA buttons:

Primary (Red):
- Background: #B01224
- Hover: gradient to orange
- Text: white, uppercase, bold
- Border-radius: 50px
- Ripple effect on click
- Shadow with red glow

Wave Button:
- Transparent with red border
- Wave fill from left on hover
- Transform: skewX for wave effect
- Color transition to white

Ocean Button:
- Navy background
- Hover: lighter blue
- White text
- Subtle wave animation
```

### フォーム要素
```
Style ocean-themed inputs:
- White background
- Bottom border only (2px)
- Focus: red border appears
- Wave animation on focus
- Labels: navy, uppercase
- Placeholder: light gray
- Error: orange border
- Success: teal accent
```

### リップルエフェクト
```
Implement ripple interactions:
- Click origin: cursor position
- Expand from 0 to 400% scale
- Fade opacity during expansion
- Duration: 0.6s ease-out
- Color: white at 0.5 opacity
- Multiple ripples allowed
```

## 特殊効果・パターン

### 波形パターン
```
Create wave patterns:
- SVG path: M0,50 Q25,30 50,50 T100,50
- Stroke: antlers red
- Fill: none or gradient
- Animation: translateX movement
- Multiple wave layers
- Varying amplitudes
- Use as dividers or backgrounds
```

### グラデーションフロー
```
Design gradient flows:
- Start: antlers red (#B01224)
- Mid: sunset orange (#FF4500)
- End: kashima navy (#001E62)
- Angle: 135deg or 90deg
- Animated: background-position shift
- Size: 200% for animation
- Blend modes for depth
```

### ローズブルーム
```
Create rose bloom effect:
- Radial gradient from center
- Start: crimson (#DC143C)
- End: sakura pink (#FFB7C5)
- Scale animation on trigger
- Opacity pulse
- Multiple bloom points
- Soft blur edges
```

## レイアウトパターン

### 情熱と海の対比
```
Create passion-ocean contrast:
- Top half: warm reds and oranges
- Bottom half: cool blues and navy
- Transition: wave or gradient
- Content: white for contrast
- Accents: opposite color hints
- Balance: 60/40 or 50/50
```

### 流動的グリッド
```
Design fluid grid system:
- 12 columns with 24px gutters
- Wave-like section breaks
- Cards with varying heights
- Stagger animation on scroll
- Red accents on hover
- Navy shadows for depth
```

### 花びら配置
```
Implement petal layout:
     ●
   ●   ●
  ●  ●  ●
   ●   ●
     ●
- Center focus point
- Radial arrangement
- Each petal: interactive
- Hover: bloom outward
- Click: navigation or modal
```

## モバイル最適化

### レスポンシブ波形
```
Adapt waves for mobile:
- Reduce amplitude to 15px
- Simplify SVG paths
- Static waves option
- Vertical wave orientation
- Touch-friendly interactions
- Faster animations (1.5s)
```

### タッチインタラクション
```
Optimize for touch devices:
- Tap targets: 44px minimum
- Remove hover states
- Add touch feedback
- Swipe for navigation
- Pull-to-refresh with wave
- Bottom sheet modals
```

## パフォーマンス最適化

### グラデーント最適化
```
Optimize gradient rendering:
- CSS gradients over images
- Limit gradient stops
- Use GPU acceleration
- Cache gradient backgrounds
- Reduce animation complexity
- Static fallbacks available
```

### アニメーション効率化
```
Optimize animations:
- Transform and opacity only
- Will-change on animated elements
- RequestAnimationFrame usage
- Intersection Observer triggers
- Reduce motion settings
- 60fps target
```

## アクセシビリティ

### カラーコントラスト
```
Ensure contrast compliance:
- Red on white: 7.5:1 (AAA)
- Navy on white: 15:1 (AAA)
- White on red: 7.5:1 (AAA)
- White on navy: 15:1 (AAA)
- Avoid red on navy directly
```

### フォーカス表示
```
Implement focus indicators:
- Orange outline (#FF4500)
- 3px width, 2px offset
- Visible on all backgrounds
- Custom for each component
- Keyboard navigation paths
```

## 使用上の注意

このデザインシステムは強い色彩対比と
動的な要素が特徴です。
情熱的なブランドメッセージに最適ですが、
静的なコンテンツには不向きな場合があります。
赤と紺の使用バランスに注意してください。