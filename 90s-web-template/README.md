# 90s Web Design Template

## 概要
1990年代初期のWorld Wide Web黎明期を再現したデザインテンプレート。Under Construction、アニメーションGIF、MIDIファイル、フレームセット、そして原色の嵐。Webの無限の可能性を信じていた時代へのオマージュ。

## デザイン哲学

### コアコンセプト
- **Information Superhighway**: 情報高速道路への入り口
- **Under Construction Forever**: 永遠に工事中
- **GIF Paradise**: アニメーションGIFの楽園
- **HTML Tables Everything**: テーブルで全てを構築
- **Netscape Navigator Era**: ブラウザ戦争の時代

### 視覚的特徴
1. **原色の多用**: 青リンク、紫訪問済み、赤文字、黄色背景
2. **背景パターン**: タイル状の繰り返し背景画像
3. **アニメーションGIF**: 回転するロゴ、点滅するメール、工事中看板
4. **Times New Roman**: デフォルトフォントの美学
5. **3D効果**: ベベル、エンボス、影付き文字

## 使用シーン

### 最適な用途
- レトロゲームサイト
- 90年代カルチャー展示
- インターネット歴史博物館
- ノスタルジックプロジェクト
- アートインスタレーション

### 避けるべき用途
- 現代的な企業サイト
- モバイルファースト設計
- Eコマース
- SaaS製品
- 金融サービス

## カラーパレット

```
WEB SAFE BLUE:   #0000FF (標準リンク色)
VISITED PURPLE:  #551A8B (訪問済みリンク)
ACTIVE RED:      #FF0000 (アクティブリンク)
BLACK:           #000000 (標準テキスト)
WHITE:           #FFFFFF (背景)
YELLOW:          #FFFF00 (ハイライト)
LIME:            #00FF00 (NEW!表示)
CYAN:            #00FFFF (特別な強調)
MAGENTA:         #FF00FF (重要な告知)
GRAY:            #808080 (区切り線)
```

## タイポグラフィ

### フォントファミリー
```css
Default:  Times New Roman, Times, serif
Heading:  Arial, Helvetica, sans-serif
Code:     Courier New, Courier, monospace
Special:  Comic Sans MS, cursive (後期90年代)
```

## 主要コンポーネント

### Welcome Banner
```
╔════════════════════════════════════════╗
║  WELCOME TO MY HOMEPAGE ON THE WWW!   ║
║    Best viewed with Netscape 3.0      ║
║        Resolution: 800x600             ║
╚════════════════════════════════════════╝
```

### Under Construction
```
     /\
    /  \
   / ⚠  \  UNDER CONSTRUCTION
  /______\  Please come back soon!
  
[Animated GIF of construction worker]
```

### Navigation Table
```html
<TABLE BORDER="3" CELLPADDING="5" CELLSPACING="2">
  <TR>
    <TD BGCOLOR="#FF0000"><A HREF="home.html">HOME</A></TD>
    <TD BGCOLOR="#00FF00"><A HREF="about.html">ABOUT</A></TD>
    <TD BGCOLOR="#0000FF"><A HREF="links.html">LINKS</A></TD>
    <TD BGCOLOR="#FFFF00"><A HREF="guestbook.html">GUESTBOOK</A></TD>
  </TR>
</TABLE>
```

### Hit Counter
```
You are visitor number:
[0][0][0][4][2][1]
Since January 1, 1996
```

### Webring
```
<< PREV | RANDOM | NEXT >>
[___Geocities Neighborhood___]
This site is part of the CoolSites webring
```

### Email Link
```
[Animated Mail GIF]
Send me email: webmaster@geocities.com
(Please allow 48-72 hours for response)
```

## デコレーション要素

### 区切り線バリエーション
```html
<HR>
<HR SIZE="5" WIDTH="50%" COLOR="#FF0000">
<HR NOSHADE>
Rainbow divider: [animated rainbow bar.gif]
Under construction: [construction line.gif]
```

### Blinking Text
```html
<BLINK>NEW!</BLINK>
<BLINK>HOT!</BLINK>
<BLINK>UPDATED!</BLINK>
```

### Marquee Messages
```html
<MARQUEE>Welcome to the World Wide Web!</MARQUEE>
<MARQUEE DIRECTION="RIGHT">This site is Netscape Enhanced!</MARQUEE>
<MARQUEE BEHAVIOR="ALTERNATE">Sign my guestbook!</MARQUEE>
```

### アニメーションGIFギャラリー
```
- rotating_email.gif (回転する封筒)
- under_construction.gif (工事中看板)
- flame.gif (炎文字)
- spinning_globe.gif (回転する地球)
- new_blink.gif (点滅NEW)
- welcome.gif (虹色Welcome)
- counter.gif (デジタルカウンター)
- netscape_now.gif (Netscapeボタン)
```

## レイアウトパターン

### フレームセット
```
┌─────────────────────────────────┐
│         Banner Frame            │
├──────┬──────────────────────────┤
│ Menu │                          │
│Frame │     Content Frame        │
│      │                          │
│      │                          │
└──────┴──────────────────────────┘
```

### テーブルレイアウト
```
TABLE WIDTH="100%" BORDER="1"
  TR
    TD COLSPAN="2" - Header
  TR
    TD WIDTH="150" - Navigation
    TD - Main Content
  TR
    TD COLSPAN="2" - Footer
```

## インタラクション

### JavaScript Alert
```javascript
alert("Welcome to my homepage!");
window.status = "Welcome to the coolest site on the web!";
```

### Image Maps
```
[Image with clickable areas]
Click on different parts to navigate!
```

### Java Applets
```
[Java Applet: Scrolling Text]
[Java Applet: Lake Effect]
[Java Applet: Clock]
Your browser doesn't support Java!
```

### MIDI Background Music
```
♪ Playing: canyon.mid
[Stop] [Play] [Loop]
```

## ブラウザ対応

### Best Viewed With
```
This page is best viewed with:
- Netscape Navigator 3.0 or higher
- Internet Explorer 3.0 or higher
- Resolution: 800x600
- 256 Colors
```

### Browser Detection
```javascript
if (navigator.appName == "Netscape") {
    document.write("Netscape users click here!");
} else {
    document.write("IE users click here!");
}
```

## 特別な機能

### Guestbook
```
┌─────────────────────────────────┐
│        SIGN MY GUESTBOOK        │
├─────────────────────────────────┤
│ Name: [___________]             │
│ Email: [___________]            │
│ Homepage: [___________]         │
│ Comments:                       │
│ [                             ] │
│ [                             ] │
│ [Submit] [Reset]               │
└─────────────────────────────────┘
```

### Awards & Badges
```
[Cool Site Award]  [Top 5% of Web]
[Netscape Now!]    [Made with Mac]
[Best Viewed IE3]  [HTML 3.2 Valid]
```

### Download Section
```
FREE DOWNLOADS!!!
- Winamp Skins
- Desktop Wallpapers (800x600)
- Screen Savers
- MIDI Files
- Animated Cursors
(Right-click and Save As...)
```

## アクセシビリティ

### 90年代スタイル
- ALT属性は気が向いたら
- テーブルレイアウトで構造無視
- 固定幅デザイン
- フォントサイズ固定
- フレーム使用で混乱必至

## パフォーマンス

### 特徴
- 画像の最適化なし
- インラインスタイル多用
- JavaScriptでdocument.write
- 同期的な読み込み
- プリローダーなし

## 懐かしの要素

### リンク集
```
MY FAVORITE LINKS:
- Yahoo!
- AltaVista
- GeoCities
- Angelfire
- Tripod
- HotMail
```

### 免責事項
```
DISCLAIMER: This page is for entertainment
purposes only. The webmaster is not responsible
for any damage to your computer. This site is
Y2K compliant!
```

### Copyright Notice
```
© 1996-1999 [Your Name Here]
All Rights Reserved
This page was last updated on: 01/01/1999
Made with Notepad!
```

## 使用上の注意

このテンプレートは1990年代のWeb黎明期を忠実に再現したもので、
現代のWeb標準、アクセシビリティ、ユーザビリティとは相容れません。
純粋にノスタルジックな目的、またはアート作品としてのみ使用してください。