# Ocean Flame Design Prompts

## Core Design Generation Prompt

Create a submarine depth exploration design with volcanic thermal vents and pressure systems:

### Visual Requirements
- Implement periscope navigation with rotating circular viewer and crosshairs
- Create submarine grid layouts with varied cell shapes (circles, curves, spans)
- Use depth pressure gauges with pulsing animations
- Apply thermal vent gradients rising from ocean floor
- Build multi-depth layer system with increasing blur at deeper levels

### Layout Patterns
1. **Submarine Grid**: 6x3 grid with cells spanning multiple positions
2. **Thermal Vent Section**: Vertical columns with rising gradient animations
3. **Pressure Chamber Hero**: Centered with radial depth gauges
4. **Periscope Navigation**: Fixed circular viewer with depth-level menu
5. **Depth Layers**: Surface, Twilight, Midnight, Abyss, Trench zones

### Color Application
- Deep navy (#003366) as ocean base
- Antlers red (#B01224) for passion points
- Seafoam (#E8F4F8) for wave crests
- Gradient transitions from ocean to flame

### Animation Directives
- Rising bubbles with wobble and size variation
- Thermal vent bubble streams at 8s intervals
- Depth gauge pulsing at 4s cycles
- Floating cards with 6s drift animation
- Periscope continuous rotation

## Component-Specific Prompts

### Pressure Chamber Hero
"Create a hero with radial gradient from ocean blue to midnight. Three depth gauges positioned absolutely, pulsing with depthPulse animation. Massive DEPTH/IGNITION text with 3px stroke and 40px glow. Background simulates underwater pressure chamber."

### Thermal Vents Section
"Generate 5 thermal vent columns with heights ranging 350-500px. Each vent has gradient from transparent through antlers red to rose red. Bubble animation rises through vents at 8s intervals. Columns positioned at 10%, 25%, 50%, 70%, 85% horizontally."

### Submarine Grid
"Design 6x3 grid with 200px cell height and 20px gaps. Cells have unique shapes: circles (border-radius 50%), curves (100px 0 0 100px), standard rectangles. Large cells span 2x2, wide cells span 3 columns. Each cell labeled with depth codes."

### Periscope Navigation
"Fixed header with 120px circular viewer. 8px antlers red border, crosshair overlay. Continuous rotation animation. Depth menu with levels: SURFACE, TWILIGHT, MIDNIGHT, ABYSS, TRENCH. Red underline slides under active level."

### Ocean Floor Footer
"Footer with seafoam text on midnight background. Rising bubble effects from bottom. Depth indicator shows current scroll depth. Links arranged in submarine grid pattern. Thermal glow effects at base."

## Typography Prompts

### Fluid Headers
"Use Saira Condensed for headers with variable font weight animation on scroll. Text appears to be affected by water current, with slight wave distortion."

### Body Text
"Source Sans Pro with increased letter-spacing for readability. Subtle color gradient from navy to charcoal on longer paragraphs."

### Accent Text
"Merriweather serif for quotes and highlights. Apply water drop shadow effect and slight blur as if seen through water."

## Animation Specifications

### Wave Animation
```
@keyframes waveMotion {
  0% { d: path("M0,100 Q50,80 100,100 T200,100"); }
  50% { d: path("M0,100 Q50,120 100,100 T200,100"); }
  100% { d: path("M0,100 Q50,80 100,100 T200,100"); }
}
Multiple layers with offset timing
```

### Bubble Rise
```
@keyframes bubbleRise {
  0% { transform: translateY(100vh) scale(0); }
  10% { transform: translateY(90vh) scale(1); }
  100% { transform: translateY(-10vh) scale(0.5); }
}
Random duration 10-20s, random X offset
```

### Flame Flicker
```
@keyframes flameFlicker {
  0%, 100% { transform: scaleY(1); opacity: 1; }
  25% { transform: scaleY(1.1); opacity: 0.9; }
  75% { transform: scaleY(0.95); opacity: 1; }
}
Duration: 0.5s, ease-in-out
```

### Ripple Effect
```
Expanding circles from click point
Multiple rings with decreasing opacity
Duration: 1s, ease-out
Scale from 0 to 400%
```

## Unique Layout Features

### Tidal Sections
- Content sections that expand/contract like tides
- Parallax scrolling with different speeds per layer
- Elements drift horizontally as user scrolls

### Depth Layers
- Background: Deep ocean (z-index: -2)
- Midwater: Floating elements (z-index: 0-50)
- Surface: Interactive content (z-index: 100+)
- Each layer with different blur and opacity

### Organic Shapes
- No straight edges on major containers
- Use border-radius variations: "50% 20% 50% 20%"
- Clip-path for irregular shapes
- SVG masks for complex forms

## Responsive Behavior

### Mobile (< 768px)
- Simplified wave animations
- Reduced particle count
- Static bubble positions
- Touch-optimized ripples

### Tablet (768px - 1024px)
- Moderate wave complexity
- Some floating animations
- 2-column maximum layouts

### Desktop (> 1024px)
- Full wave systems active
- All particles and effects
- Complex multi-layer parallax
- Whirlpool navigation enabled

## Anti-AI Patterns to Maintain
- Avoid perfect circles and rectangles
- No uniform spacing between elements
- Irregular wave patterns, not sine waves
- Asymmetric bubble distributions
- Organic, hand-drawn feel to shapes
- Unexpected color bleeds between sections
- Non-standard navigation patterns