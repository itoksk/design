# ASCII Terminal Design Prompts

## 基本プロンプト

### ターミナルウィンドウ生成
```
Create a retro terminal window interface with:
- Classic phosphor green or amber text on black background
- CRT screen effects including scanlines and slight curvature
- Terminal window chrome with minimize/maximize/close buttons
- Command prompt showing user@machine:~$ format
- Blinking block cursor
- Monospace font rendering
- Optional screen flicker and glow effects
```

### ASCIIアート生成
```
Generate ASCII art that:
- Uses only standard ASCII characters (32-126)
- Maintains proper spacing for monospace display
- Creates recognizable shapes and patterns
- Includes shading using characters: █▓▒░
- Features clean edges with box-drawing characters: ┌─┐│└┘
- Supports both simple line art and complex illustrations
- Works at different zoom levels
```

### マトリックスレイン効果
```
Create a Matrix-style digital rain effect with:
- Vertical streams of characters falling at different speeds
- Japanese katakana mixed with numbers and symbols
- Gradual fade from bright green to dark green
- Random character changes as they fall
- Variable stream lengths and speeds
- Characters leaving trails
- Occasional bright "lead" characters
```

### CRTエフェクト
```
Apply authentic CRT monitor effects including:
- Horizontal scanlines moving slowly down the screen
- Subtle RGB color separation (chromatic aberration)
- Screen curvature at edges
- Phosphor glow around bright text
- Occasional flicker or interference
- Slight static noise overlay
- Bloom effect on bright areas
- Vignette darkening at corners
```

## コンポーネント別プロンプト

### コマンドラインインターフェース
```
Design a functional command-line interface with:
- Input field with command history
- Auto-completion suggestions
- Syntax highlighting for commands
- Error messages in red
- Success messages in green
- Directory navigation visualization
- Command output formatting
- Scrollable history buffer
```

### ASCIIメニュー
```
Create an ASCII-based menu system featuring:
- Box-drawn borders around menu items
- Keyboard navigation indicators
- Selected item highlighting (inverted colors)
- Numbered options or arrow key selection
- Nested submenus with tree structure
- Status bar at bottom
- Help text in corner
Format:
┌─────────────────────┐
│  1. New Game        │
│ >2. Load Game       │
│  3. Options         │
│  4. Exit            │
└─────────────────────┘
```

### ASCIIテーブル
```
Generate ASCII tables with:
- Clean borders using box-drawing characters
- Column headers with separator lines
- Aligned data in columns
- Optional row numbers
- Footer with totals/summary
Example format:
╔════╦══════════╦═════════╗
║ ID ║   Name   ║  Score  ║
╠════╬══════════╬═════════╣
║ 01 ║ Player1  ║  9,999  ║
║ 02 ║ Player2  ║  8,765  ║
╚════╩══════════╩═════════╝
```

### ローディングアニメーション
```
Create ASCII loading animations including:
- Progress bar: [████████░░░░░░░░] 50%
- Spinning indicators: ⠋ ⠙ ⠹ ⠸ ⠼ ⠴ ⠦ ⠧ ⠇ ⠏
- Dot animation: Loading... / Loading.. / Loading.
- ASCII art spinner:
  /-\|/-\|
- Percentage counter with bar fill
- Matrix-style streaming characters
- Typewriter effect for messages
```

### ダイアログボックス
```
Design ASCII dialog boxes with:
- Double or single line borders
- Title bar with centered text
- Content area with word wrapping
- Button options at bottom
- Shadow effect using darker characters
Format:
╔══════════════════════════╗
║     Confirmation         ║
╟──────────────────────────╢
║ Are you sure you want    ║
║ to delete this file?     ║
╟──────────────────────────╢
║  [YES]     [NO]          ║
╚══════════════════════════╝
```

## アニメーション・エフェクトプロンプト

### タイピング効果
```
Implement realistic typing animation:
- Characters appear one by one
- Variable speed for human-like typing
- Occasional backspace and correction
- Cursor blinking at end of text
- Sound effect per keystroke (optional)
- Pause at punctuation
- Speed variations for different text types
- Multi-line typing with carriage returns
```

### グリッチテキスト
```
Create glitch text effects:
- Random character substitution
- Position offset jittering
- Color channel separation
- Temporary scrambling
- Binary/hex number insertions
- Static noise characters: ▓▒░
- Corruption patterns
- Recovery animation
```

### ブートシーケンス
```
Design system boot sequence:
- BIOS/UEFI style messages
- Memory test counter
- Hardware detection messages
- Service startup notifications
- ASCII art logo display
- Progress indicators
- System information display
- Login prompt appearance
Example:
BIOS v2.31 - Checking RAM... OK
Loading kernel... [OK]
Starting services...
  * Network Manager [OK]
  * Display Manager [OK]
Welcome to Terminal OS v1.0
Login: _
```

## インタラクションプロンプト

### キーボードショートカット
```
Implement keyboard controls:
- Vim-style navigation (h,j,k,l)
- Tab completion for commands
- Ctrl+C to cancel operations
- Ctrl+L to clear screen
- Arrow keys for history
- PageUp/PageDown for scrolling
- Function keys for quick actions
- ESC for menu/cancel
```

### テキスト選択
```
Create text selection interface:
- Click and drag to select
- Double-click for word selection
- Triple-click for line selection
- Highlighted selection with inverse colors
- Copy to clipboard support
- Visual feedback during selection
- Block selection mode (Alt+drag)
```

### コマンド実行
```
Design command execution system:
- Parse user input
- Execute predefined commands
- Show command output
- Handle errors gracefully
- Support piping and redirection
- Command history with up/down arrows
- Tab completion for commands/files
- Help system with 'man' pages
```

## スタイル生成プロンプト

### レトロターミナルテーマ
```
Create authentic retro terminal themes:

1. IBM 3270 (Green Screen):
   - Bright green (#00FF00) on black
   - Block cursor
   - Heavy scanlines
   
2. DEC VT100 (Amber):
   - Amber (#FFAA00) on black
   - Underline cursor
   - Slight screen curve
   
3. Apple II:
   - Apple green (#33FF00) on black
   - 40/80 column modes
   - Blocky character rendering
   
4. Commodore 64:
   - Light blue on dark blue
   - PETSCII characters
   - Border color
```

### ASCIIアートスタイル
```
Generate different ASCII art styles:

1. Line Art:
   Using: - | / \ _ 
   Simple geometric shapes

2. Shaded Art:
   Using: █▓▒░ for gradients
   3D depth effects

3. Block Art:
   Using: ▀▄█▌▐░▒▓
   Pixel-art style

4. Text Art:
   Using letters to form images
   Typography as illustration
```

### フレームデコレーション
```
Create decorative ASCII frames:

Simple:
+--------+
|        |
+--------+

Ornate:
╔══════════╗
║ ◊ TITLE ◊║
╠══════════╣
║          ║
╚══════════╝

Tech:
◢█████████◣
█ SYSTEM  █
█▄▄▄▄▄▄▄▄▄█

Minimal:
─────────
 CONTENT
─────────
```

## 特殊効果プロンプト

### ハッカー画面
```
Create Hollywood-style hacker interface:
- Rapidly scrolling text
- Multiple terminal windows
- Network traffic visualization
- ASCII art skull or logo
- Progress bars for "hacking"
- Flashing warnings
- Matrix rain background
- Hexadecimal data streams
- "Access Granted" animations
```

### システムモニター
```
Design system monitoring display:
- CPU usage bar graph
- Memory usage visualization
- Network traffic indicators
- Process list table
- Disk usage charts
- Temperature readings
- All in ASCII characters
Example:
CPU: [████████░░] 80%
MEM: [██████░░░░] 60%
NET: ↓128KB/s ↑64KB/s
```

### ゲーム要素
```
Create ASCII game interfaces:
- Roguelike dungeon maps
- Text adventure prompts
- ASCII sprite animations
- Score displays
- Health/mana bars
- Inventory systems
- Mini-maps
Example dungeon:
#########
#.....@.#
#.......#
#...M...#
#########
@ = Player, M = Monster, . = Floor, # = Wall
```

## パフォーマンス最適化プロンプト

### 軽量版
```
Create performance-optimized version:
- Disable complex animations
- Reduce particle effects
- Simplify scanline rendering
- Use CSS instead of JS where possible
- Lazy load ASCII art
- Minimize redraws
- Cache rendered text
```

### アクセシビリティ版
```
Design accessible terminal interface:
- High contrast mode
- Screen reader friendly
- Keyboard-only navigation
- Skip ASCII art option
- Clear focus indicators
- Descriptive ARIA labels
- Alternative text for art
- Adjustable font size
```

## 使用上の注意

これらのプロンプトはレトロな美学を重視しており、
現代的なUIの慣習とは異なる場合があります。
ユーザビリティとノスタルジアのバランスを考慮して使用してください。