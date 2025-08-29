# Royal Fortress Design Prompts

## Core Design Generation Prompt

Create a design with fortress-like structures, castle battlements, and royal grandeur:

### Visual Requirements
- Implement castle battlement patterns as section dividers
- Create shield-shaped cards and containers
- Use metallic gold shimmer effects on important elements
- Apply stone texture overlays for depth
- Build tower-like vertical navigation structures

### Layout Patterns
1. **Fortress Wall Header**: Crenellated top edge with watchtowers
2. **Shield Grid**: Hexagonal and shield-shaped card arrangements
3. **Tower Sidebar**: Vertical tower structure for navigation
4. **Throne Room Hero**: Centered grandeur with radiating golden lines
5. **Castle Gate Footer**: Arched doorways and portcullis patterns

### Color Application
- Royal blue (#003DA5) as primary nobility
- Fortress black (#0D0D0D) for structure
- Champion gold (#FFD700) for accents and glory
- Pure white (#FFFFFF) for clarity
- Metallic gradients for premium feel

### Animation Directives
- Gold shimmer moving across surfaces
- Drawbridge lowering on scroll
- Banner flags waving in the wind
- Torch flames flickering
- Shield rotation on hover

## Component-Specific Prompts

### Fortress Header
"Create a header with castle battlement silhouette along the top edge. Include corner watchtowers with flag animations. Background uses fortress black with gold trim. Navigation items appear as carved stone blocks with gold inlay on hover."

### Throne Room Hero
"Design a hero section with central throne-like focal point. Radiating golden lines emanate from center like sun rays. Large serif typography with gold foil effect. Background has subtle stone texture with inner shadow for depth."

### Shield Grid
"Arrange content cards in hexagonal honeycomb pattern or shield shapes using clip-path. Each shield has a different heraldic-inspired background pattern. Gold borders appear on hover with slight rotation. Drop shadows create layered castle wall effect."

### Tower Navigation
"Fixed vertical navigation styled as a castle tower. Circular tower top with rotating banner. Menu items stack vertically like tower windows. Gold highlight travels up the tower on scroll position."

### Drawbridge CTA
"Call-to-action styled as castle drawbridge. On hover, chains animate and bridge lowers (transform: rotateX). Gold trim highlights the entrance. Shadow beneath creates moat effect."

### Castle Gate Footer
"Footer with large arched gateway design. Multiple archways of decreasing size create depth. Portcullis pattern overlay using CSS grid. Links arranged in heraldic shield formations."

## Typography Prompts

### Royal Headers
"Use Cinzel or similar Roman-inspired serif. Large size with wide letter-spacing. Gold gradient text with subtle shadow. Text appears carved in stone."

### Body Text
"Montserrat for modern readability. High contrast between headers and body. Generous line-height for luxury feel."

### Heraldic Numbers
"Bebas Neue for strong numerical display. Metallic gold effect with inner shadow. Numbers appear embossed on shields."

## Animation Specifications

### Gold Shimmer
```
@keyframes goldShimmer {
  0% { background-position: -200% center; }
  100% { background-position: 200% center; }
}
Linear gradient with gold highlights
Duration: 3s, infinite
```

### Banner Wave
```
@keyframes bannerWave {
  0%, 100% { transform: rotate(-2deg); }
  50% { transform: rotate(2deg); }
}
Transform-origin: top left
Duration: 4s, ease-in-out
```

### Drawbridge Lower
```
@keyframes drawbridgeLower {
  from { transform: rotateX(-90deg); }
  to { transform: rotateX(0); }
}
Transform-origin: bottom
Duration: 0.8s, ease-out
```

### Torch Flicker
```
@keyframes torchFlicker {
  0%, 100% { opacity: 1; filter: brightness(1); }
  50% { opacity: 0.8; filter: brightness(1.2); }
}
Random delay per torch
Duration: 0.5-1s
```

## Unique Layout Features

### Fortress Architecture
- Thick borders (4-8px) suggesting stone walls
- Beveled edges using box-shadow insets
- Layered sections like castle terraces
- Vertical emphasis suggesting tower height

### Heraldic Patterns
- Diagonal stripes (supporter pattern)
- Checkered backgrounds (chess pattern)
- Quatrefoil and trefoil decorations
- Lion and crown watermarks

### Defensive Structures
- Moat-like gaps between sections
- Arrow slit shaped dividers
- Portcullis grid overlays
- Watchtower corner elements

### Royal Elements
- Crown-shaped badges
- Scepter divider lines
- Throne-like focal points
- Banner/flag decorations

## Responsive Behavior

### Mobile (< 768px)
- Simplified battlement patterns
- Single tower navigation
- Stacked shield cards
- Reduced gold effects

### Tablet (768px - 1024px)
- Moderate fortress complexity
- Two-column shield grid
- Side tower navigation

### Desktop (> 1024px)
- Full castle architecture
- Complex heraldic patterns
- Multiple tower elements
- All gold animations active

### Luxury (> 1920px)
- Extra wide fortress walls
- Enhanced gold effects
- Additional decorative elements
- Parallax castle layers

## Anti-AI Patterns to Maintain
- Avoid perfect symmetry (real castles are asymmetric)
- Use rough stone textures, not smooth gradients
- Irregular battlement spacing
- Hand-drawn heraldic elements
- Unexpected defensive angles
- Non-uniform brick/stone patterns
- Medieval imperfections in design