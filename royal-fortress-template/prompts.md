# Royal Fortress Design Prompts

## Core Design Generation Prompt

Create a blue flame fortress design with dual core power systems and citadel architecture:

### Visual Requirements
- Implement blue flame geometric patterns with triangular shards
- Create dual core grid systems with hexagonal and rectangular cells
- Use plasma stream animations connecting core elements
- Apply gold accent highlights on critical power nodes
- Build citadel structures with angular, fortress-like geometry

### Layout Patterns
1. **Fortress Wall Header**: Crenellated top edge with watchtowers
2. **Shield Grid**: Hexagonal and shield-shaped card arrangements
3. **Tower Sidebar**: Vertical tower structure for navigation
4. **Throne Room Hero**: Centered grandeur with radiating golden lines
5. **Castle Gate Footer**: Arched doorways and portcullis patterns

### Color Application
- Blue (#003DA5) and Black (#0D0D0D) as primary fortress colors
- Gold (#FFD700) and White (#FFFFFF) as power accent colors
- Blue flame spectrum (#4A90E2, #0066FF, #001E4D) for core energy
- Blue represents the flame core, black the fortress walls
- Gold traces the power pathways, white the energy peaks

### Animation Directives
- Plasma streams flowing through power channels
- Blue flame shards pulsing with energy
- Gold power indicators cycling intensity
- Dual core rotation in opposite directions
- Citadel gates sliding open on interaction

## Component-Specific Prompts

### Rampart Header
"Create a header with zigzag bottom edge resembling fortress ramparts. Navigation links use parallelogram clip-paths with gold slide-in on hover. Background is fortress black with 4px gold bottom border. Links overlap like defensive positions."

### Blue Flame Core Hero
"Design a hero with 20x10 grid of triangular flame shards in blue variations. Central dual core title with 3deg skew and gold stroke. Plasma streams connect shards. Power badge with polygon clip-path. Background is fortress black with blue glow."

### Dual Core Grid
"Create a 3-column, 4-row grid mixing hexagonal and rectangular cells. Cells span multiple positions creating asymmetric layout. Blue glow on active cells, gold trim on hover. Each cell contains code designation (A1, B2, etc.)."

### Power Gauge Sidebar
"Fixed left sidebar with vertical power level indicators. Blue plasma fills gauge on scroll. Gold markers at 25/50/75/100 levels. Pulse animation when reaching thresholds. Width transitions on hover."

### Plasma Gate CTA
"Call-to-action with sliding plasma beams. On hover, beams part horizontally revealing gold core. Blue electric arcs at edges. Transform scale and glow intensity increase on interaction."

### Citadel Foundation Footer
"Footer with angular fortress base design. Three-tier structure with blue plasma channels. Gold power nodes at intersections. Links use hexagonal clip-paths with designation codes."

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