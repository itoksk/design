# 90s Web Design Prompts

## 基本プロンプト

### 90年代ホームページレイアウト
```
Create a 1990s personal homepage with:
- Fixed width table layout (640px or 800px)
- Tiled background pattern (stars.gif or clouds.gif)
- Centered content using <CENTER> tags
- Welcome banner with animated GIF text
- Navigation using HTML table with colored cells
- "Under Construction" animated GIF
- Hit counter at the bottom
- "Best viewed with Netscape" badge
- Multiple <HR> horizontal rules as dividers
- Times New Roman as default font
```

### フレームセットレイアウト
```
Design a frameset-based layout:
- Top frame: Banner with site title (height: 100px)
- Left frame: Navigation menu (width: 150px)
- Main frame: Content area
- Optional bottom frame: Copyright info
- Frame borders visible (5px, gray)
- No frameborder for clean look option
- NOFRAMES fallback content
- Each frame loads separate HTML file
Structure:
<FRAMESET ROWS="100,*,50">
  <FRAME SRC="banner.html">
  <FRAMESET COLS="150,*">
    <FRAME SRC="menu.html">
    <FRAME SRC="main.html">
  </FRAMESET>
  <FRAME SRC="footer.html">
</FRAMESET>
```

### Under Construction ページ
```
Create an "Under Construction" page featuring:
- Large construction worker animated GIF
- Blinking "UNDER CONSTRUCTION" text
- Yellow and black striped borders
- "Coming Soon!" message
- Expected completion date
- "Sign up for updates" email form
- Animated construction barriers
- Hard hat icons
- "Please bookmark and come back" text
- Alternative "Site Map" link
```

### ゲストブック
```
Design a 90s-style guestbook with:
- TABLE-based form layout
- Text input fields with SIZE attribute
- TEXTAREA for comments (ROWS=10 COLS=50)
- "Sign My Guestbook!" header with rainbow text
- View previous entries below form
- Each entry in a table cell
- Visitor counter integration
- "Thanks for signing!" JavaScript alert
- Email notification option
- Anti-spam question (simple math)
```

## コンポーネント別プロンプト

### Welcome Banner
```
Create a welcome banner with:
- Animated "WELCOME" GIF (flame text or rainbow)
- Site title in <H1> with <CENTER>
- "You are visitor number [counter]"
- Current date/time display
- "Best viewed at 800x600" notice
- Browser detection message
- "Please sign my guestbook!" link
- Scrolling marquee with news
Format:
╔════════════════════════════════╗
║  WELCOME TO [NAME]'S HOMEPAGE  ║
║   ON THE WORLD WIDE WEB!       ║
╚════════════════════════════════╝
```

### ナビゲーションテーブル
```
Design navigation using HTML tables:
<TABLE BORDER="3" CELLPADDING="10" BGCOLOR="#C0C0C0">
  <TR>
    <TD BGCOLOR="#FF0000">
      <A HREF="index.html">
        <FONT COLOR="#FFFFFF"><B>HOME</B></FONT>
      </A>
    </TD>
    <TD BGCOLOR="#00FF00">
      <A HREF="about.html">
        <FONT COLOR="#000000"><B>ABOUT ME</B></FONT>
      </A>
    </TD>
    <TD BGCOLOR="#0000FF">
      <A HREF="photos.html">
        <FONT COLOR="#FFFFFF"><B>PHOTOS</B></FONT>
      </A>
    </TD>
  </TR>
</TABLE>
Each cell different color, 3D border effect
```

### Email Contact
```
Create email contact section:
- Animated spinning envelope GIF
- "Send me email!" text
- mailto: link with subject
- "Please allow 48 hours for response"
- ASCII art email address (spam prevention)
- "NO SPAM PLEASE!" warning
- Alternative contact form
- ICQ number display
- "Email me at: webmaster AT geocities DOT com"
```

### リンク集ページ
```
Design a links page featuring:
- "MY FAVORITE LINKS" title with HR
- Categories in separate tables
- Each link with description
- "COOL!" or "HOT!" animated GIFs
- Reciprocal link requests
- Link exchange banner section
- "Add your link" form
- Dead link report option
Categories:
- Search Engines (Yahoo!, AltaVista, Excite)
- Cool Sites
- Friend's Pages
- Web Resources
```

### Hit Counter
```
Implement various hit counter styles:
1. Odometer style:
   Black background, green LED digits
   [0][0][1][2][3][4]
   
2. Animated GIF counter:
   Each digit as separate GIF
   
3. Text-based:
   "You are visitor number 12,345"
   "Counter started: January 1, 1996"
   
4. CGI counter:
   <IMG SRC="/cgi-bin/counter.cgi">
```

## アニメーション・エフェクトプロンプト

### Animated GIFs Collection
```
Include these classic animated GIFs:
- Rotating @ symbol for email
- Under construction signs
- Flaming text
- Spinning globe
- Dancing baby
- Rotating "NEW!" star
- Mailbox with flag
- Yellow smiley face
- Torch flames
- Police/emergency lights
- Fireworks
- American flag waving
- Computer with typing animation
- Book with turning pages
```

### マーキーテキスト
```
Implement scrolling text variations:
<MARQUEE>Welcome to my homepage!</MARQUEE>
<MARQUEE DIRECTION="RIGHT">This site is Netscape enhanced!</MARQUEE>
<MARQUEE BEHAVIOR="ALTERNATE">Sign my guestbook!</MARQUEE>
<MARQUEE SCROLLAMOUNT="10">Fast scrolling news!</MARQUEE>
<MARQUEE HEIGHT="50" BGCOLOR="#FFFF00">Important announcement!</MARQUEE>
```

### ブリンクテキスト
```
Create blinking elements:
<BLINK>NEW!</BLINK>
<BLINK><FONT COLOR="#FF0000">HOT!</FONT></BLINK>
<BLINK>UPDATED TODAY!</BLINK>
Note: Only works in Netscape Navigator
Alternative: Use animated GIF for cross-browser
```

### JavaScript Effects
```
Add 90s JavaScript interactions:
1. Welcome alert:
   alert("Welcome to my homepage!");
   
2. Status bar scroll:
   Scrolling text in browser status bar
   
3. Mouse trail:
   Text or images following cursor
   
4. Image rollover:
   onMouseOver="this.src='image2.gif'"
   
5. Popup windows:
   window.open('popup.html','','width=400,height=300')
   
6. Right-click disable:
   "No right click allowed!"
```

## スタイル生成プロンプト

### 背景パターン
```
Create tiled background patterns:
1. Starfield:
   Black background with white dots
   
2. Clouds:
   Repeating cloud pattern
   
3. Paper texture:
   Crumpled paper effect
   
4. Water/marble:
   Blue marble texture
   
5. Wood grain:
   Brown wood pattern
   
Implementation:
<BODY BACKGROUND="stars.gif">
or
<BODY BGCOLOR="#000000" TEXT="#FFFFFF">
```

### カラースキーム
```
Apply 90s color combinations:

1. Default:
   Background: White (#FFFFFF)
   Text: Black (#000000)
   Links: Blue (#0000FF)
   Visited: Purple (#551A8B)
   
2. Inverse:
   Background: Black (#000000)
   Text: White (#FFFFFF)
   Links: Cyan (#00FFFF)
   
3. Neon:
   Background: Black
   Text: Lime (#00FF00)
   Links: Yellow (#FFFF00)
   
4. Pastel:
   Background: Light Blue (#ADD8E6)
   Text: Dark Blue (#000080)
```

### テーブルデザイン
```
Style tables with 90s aesthetics:
<TABLE BORDER="5" CELLPADDING="10" CELLSPACING="5"
       BGCOLOR="#C0C0C0" BORDERCOLOR="#000000">
  <TR>
    <TD BGCOLOR="#FF0000" ALIGN="CENTER">
      <FONT SIZE="+2" COLOR="#FFFFFF"><B>HEADER</B></FONT>
    </TD>
  </TR>
  <TR>
    <TD BGCOLOR="#FFFFFF">
      Content with &nbsp;&nbsp;&nbsp; for spacing
    </TD>
  </TR>
</TABLE>
```

### 3D Text Effects
```
Create 3D text without CSS:
1. Use images for headers
2. Multiple font tags for shadow:
   <FONT COLOR="#808080">Shadow</FONT>
   <FONT COLOR="#000000">Text</FONT>
3. ASCII art headers:
   ╔══════════════╗
   ║   WELCOME    ║
   ╚══════════════╝
```

## 特殊機能プロンプト

### Webring Integration
```
Add webring navigation:
<TABLE BORDER="2" BGCOLOR="#C0C0C0">
  <TR>
    <TD COLSPAN="5" ALIGN="CENTER">
      <B>GeoCities Neighborhood Ring</B>
    </TD>
  </TR>
  <TR>
    <TD><A HREF="prev.html">&lt;&lt; PREV</A></TD>
    <TD><A HREF="next.html">NEXT &gt;&gt;</A></TD>
    <TD><A HREF="random.html">RANDOM</A></TD>
    <TD><A HREF="list.html">LIST</A></TD>
    <TD><A HREF="join.html">JOIN</A></TD>
  </TR>
</TABLE>
```

### Awards Section
```
Display website awards:
- "Cool Site of the Day" badge
- "Top 5% of the Web" award  
- "HTML 3.2 Compliant" button
- "Netscape Now!" button
- "Made with Macintosh" badge
- Custom award GIFs
- Award ceremony dates
- Links to award sites
```

### Download Area
```
Create downloads section:
- Desktop wallpapers (640x480, 800x600)
- Winamp skins
- Screen savers (.scr files)
- MIDI collection
- Animated cursors (.ani)
- "Right-click to Save As" instruction
- File sizes in KB
- "Get WinZip!" link
- Download counter per file
```

### Java Applet Effects
```
Include Java applets:
<APPLET CODE="Lake.class" WIDTH="300" HEIGHT="200">
  <PARAM NAME="image" VALUE="photo.jpg">
  Your browser doesn't support Java!
</APPLET>

Common applets:
- Lake reflection effect
- Scrolling text ticker
- Ripple effect on images
- Analog clock
- Eyes following mouse
```

## フォーム要素プロンプト

### 基本フォーム
```
Create 90s-style forms:
<FORM ACTION="/cgi-bin/formmail.cgi" METHOD="POST">
  <TABLE>
    <TR>
      <TD>Name:</TD>
      <TD><INPUT TYPE="TEXT" NAME="name" SIZE="30"></TD>
    </TR>
    <TR>
      <TD>Email:</TD>
      <TD><INPUT TYPE="TEXT" NAME="email" SIZE="30"></TD>
    </TR>
    <TR>
      <TD>Comments:</TD>
      <TD><TEXTAREA NAME="comments" ROWS="5" COLS="30"></TEXTAREA></TD>
    </TR>
    <TR>
      <TD COLSPAN="2" ALIGN="CENTER">
        <INPUT TYPE="SUBMIT" VALUE="Send!">
        <INPUT TYPE="RESET" VALUE="Clear">
      </TD>
    </TR>
  </TABLE>
</FORM>
```

### サーチボックス
```
Add search functionality:
- Yahoo! search box
- AltaVista search
- Site search (if available)
- "Search the Web" heading
- Submit button with "GO!" text
- "Powered by [Search Engine]" text
```

## モバイル非対応プロンプト

### Fixed Width Design
```
Enforce fixed width layout:
- 640px width (VGA)
- 800px width (SVGA)  
- Horizontal scrollbar expected
- "Best viewed at 800x600" notice
- No responsive design
- Absolute positioning with pixels
- Fixed font sizes
```

### Browser-Specific Messages
```
Show browser-specific content:
"This site is optimized for Netscape Navigator 3.0"
"Internet Explorer users click here"
"WebTV users may experience problems"
"Upgrade your browser!"
"Get Netscape!" button
"Get Internet Explorer!" button
```

## 使用上の注意

これらのプロンプトは1990年代のWeb標準（またはその欠如）を反映しており、
現代のベストプラクティスとは正反対です。
純粋にレトロな美学やノスタルジーのためにのみ使用してください。
アクセシビリティ、SEO、パフォーマンスは完全に度外視されています。