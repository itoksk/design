# Ocean Flame Design Prompts

## Core Design Generation Prompt

Create a design where ocean waves meet burning passion with fluid, organic layouts:

### Visual Requirements
- Implement wave-shaped section dividers using SVG paths
- Create floating bubble particles that rise through sections
- Use flame-like flickering effects on text and borders
- Apply water ripple animations on interactions
- Blend navy gradients with red flame accents seamlessly

### Layout Patterns
1. **Wave Sections**: Curved section boundaries that flow like ocean waves
2. **Tidal Grid**: Cards that float at different depths with parallax
3. **Whirlpool Navigation**: Circular menu with spiral animation
4. **Coral Reef Footer**: Organic, branching layout structure

### Color Application
- Deep navy (#003366) as ocean base
- Antlers red (#B01224) for passion points
- Seafoam (#E8F4F8) for wave crests
- Gradient transitions from ocean to flame

### Animation Directives
- Continuous wave motion on section dividers
- Floating bubbles with random sizes and speeds
- Flame flicker on hover states
- Water ripple effect on click
- Tidal push-pull on scroll

## Component-Specific Prompts

### Hero Section
"Create a hero with animated ocean waves at the bottom using SVG paths. Overlay large text that appears to float on water with subtle bobbing animation. Add rising bubble particles and a gradient from deep navy to passionate red at focal points."

### Wave Dividers
"Generate SVG wave patterns with multiple layers moving at different speeds. Front wave: 3s duration, middle: 5s, back: 7s. Each wave slightly different amplitude and color opacity."

### Floating Grid
"Design cards that float at different z-index levels, creating depth. Apply subtle rotation and floating animation with different phases for each card. On hover, create ripple effect expanding from cursor position."

### Whirlpool Navigation
"Circular navigation menu that spirals open on hover/click. Items arranged in circle, rotating into view with staggered timing. Center logo pulses like a heartbeat."

### Coral Footer
"Footer with organic, branching structure. Links grow like coral formations. Background has subtle water caustic light effects. Elements sway gently as if underwater."

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