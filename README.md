# 🔥 FLAMES Game - Relationship Calculator

A fun and interactive web-based game to calculate relationship compatibility between two people using the classic FLAMES algorithm.

## 📋 Table of Contents
- [About](#about)
- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Installation & Setup](#installation--setup)
- [How to Run](#how-to-run)
- [How to Play](#how-to-play)
- [How It Works](#how-it-works)
- [Project Structure](#project-structure)
- [Browser Compatibility](#browser-compatibility)
- [Contributing](#contributing)
- [License](#license)

## 🎯 About

FLAMES is a popular relationship calculator game that determines the relationship between two people based on their names. FLAMES stands for:
- **F** - Friends 🤝
- **L** - Love 💖
- **A** - Affection 💕
- **M** - Marriage 💍
- **E** - Enemy 😅
- **S** - Siblings 👫

## ✨ Features

- ✅ **Zero Dependencies** - Pure HTML, CSS, and JavaScript
- ✅ **No Backend Required** - Runs entirely in the browser
- ✅ **Responsive Design** - Works on mobile, tablet, and desktop
- ✅ **Beautiful UI** - Modern gradient design with smooth animations
- ✅ **Real-time Validation** - Input validation and error handling
- ✅ **Interactive Results** - Animated results with emojis and messages
- ✅ **Perfect Match Detection** - Special handling when all characters match
- ✅ **Try Again Feature** - Easy reset to play multiple times
- ✅ **Fast & Lightweight** - No loading time, instant calculations

## 🎬 Demo

Simply open the HTML file in any modern web browser to see the game in action!

## 🛠️ Technologies Used

- **HTML5** - Structure and content
- **CSS3** - Styling, animations, and responsive design
- **JavaScript (ES6)** - Game logic and interactivity

## 📥 Installation & Setup

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge, etc.)
- A text editor (optional, for viewing/editing code)

### Download

**Option 1: Direct Download**
1. Download the `flames-game.html` file
2. Save it to your desired location on your computer

**Option 2: Clone Repository**
```bash
git clone https://github.com/yourusername/flames-game.git
cd flames-game
```

**Option 3: Create from Scratch**
1. Create a new file named `flames-game.html`
2. Copy the entire HTML code into the file
3. Save the file

## 🚀 How to Run

### Method 1: Direct Opening (Recommended)
1. Locate the `flames-game.html` file on your computer
2. **Double-click** the file
3. The game will open in your default web browser
4. Start playing immediately! 🎉

### Method 2: Using File Explorer/Finder
**Windows:**
```
1. Right-click on flames-game.html
2. Select "Open with"
3. Choose your preferred browser (Chrome, Firefox, etc.)
```

**Mac:**
```
1. Right-click (or Control+click) on flames-game.html
2. Select "Open With"
3. Choose your preferred browser (Safari, Chrome, etc.)
```

**Linux:**
```bash
# Using default browser
xdg-open flames-game.html

# Using specific browser
firefox flames-game.html
# or
google-chrome flames-game.html
```

### Method 3: Drag and Drop
1. Open your web browser
2. Drag the `flames-game.html` file into the browser window
3. The game will load automatically

### Method 4: Using a Local Server (Optional)
If you want to run it through a local server:

**Python 3:**
```bash
python -m http.server 8000
```
Then open: `http://localhost:8000/flames-game.html`

**Node.js (with http-server):**
```bash
npx http-server
```
Then open: `http://localhost:8080/flames-game.html`

**VS Code Live Server:**
1. Install "Live Server" extension in VS Code
2. Right-click on `flames-game.html`
3. Select "Open with Live Server"

## 🎮 How to Play

1. **Enter First Name** - Type the first person's name in the "First Name" field
2. **Enter Second Name** - Type the second person's name in the "Second Name" field
3. **Click "Calculate FLAMES"** - Press the button to see the result
4. **View Result** - See your relationship compatibility with a fun message!
5. **Try Again** - Click the "Try Again" button to play with different names

### Example:
```
First Name: John
Second Name: Mary

Result: L - Love 💖
Message: "Love is in the air! 💖"
```

## 🧮 How It Works

### Algorithm Steps:

1. **Input**: Take two names as input
   ```
   Name 1: FLAMES
   Name 2: GAMES
   ```

2. **Remove Common Characters**: 
   ```
   F L A M E S
   G A M E S
   
   Common: A, M, E, S
   Remaining: F, L (from FLAMES) + G (from GAMES)
   Total Count: 3
   ```

3. **Apply FLAMES Algorithm**:
   - Start with: F, L, A, M, E, S
   - Count using the remaining character count (3)
   - Eliminate letters one by one
   - The last remaining letter is the result

4. **Display Result**: Show the relationship type with a fun message!

### Code Logic:

```javascript
// Remove common characters
function removeCommonChars(name1, name2) {
    // Remove spaces, convert to lowercase
    // Find and remove common characters
    // Return count of remaining characters
}

// Calculate FLAMES result
function calculateFlames(count) {
    // Start with ['F', 'L', 'A', 'M', 'E', 'S']
    // Eliminate letters based on count
    // Return the last remaining letter
}
```

## 📁 Project Structure

```
flames-game/
│
├── flames-game.html          # Main HTML file (single file project)
│   ├── HTML Structure        # Game layout and form
│   ├── CSS Styles           # Embedded styling and animations
│   └── JavaScript Logic     # Game logic and calculations
│
└── README.md                 # Project documentation (this file)
```

### File Organization:
- **HTML**: Contains the structure of the game interface
- **CSS**: Embedded in `<style>` tags with responsive design
- **JavaScript**: Embedded in `<script>` tags with game logic

## 🌐 Browser Compatibility

The game works on all modern browsers:

| Browser | Minimum Version | Status |
|---------|----------------|--------|
| Chrome  | 60+            | ✅ Fully Supported |
| Firefox | 60+            | ✅ Fully Supported |
| Safari  | 12+            | ✅ Fully Supported |
| Edge    | 79+            | ✅ Fully Supported |
| Opera   | 50+            | ✅ Fully Supported |

### Mobile Support:
- ✅ iOS Safari (iOS 12+)
- ✅ Chrome Mobile (Android 5+)
- ✅ Samsung Internet
- ✅ Firefox Mobile

## 🎨 Customization

You can easily customize the game by editing the HTML file:

### Change Colors:
```css
/* Find this in the <style> section */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Change to your preferred colors */
background: linear-gradient(135deg, #FF6B6B 0%, #4ECDC4 100%);
```

### Modify Messages:
```javascript
// Find the getMessage() function
const messages = {
    'F': "Your custom Friends message! 🤝",
    'L': "Your custom Love message! 💖",
    // ... customize other messages
};
```

### Add Sound Effects (Optional):
```javascript
// Add in the calculateFlames function
const audio = new Audio('result-sound.mp3');
audio.play();
```

## 🐛 Troubleshooting

### Common Issues:

**Issue 1: File doesn't open**
- **Solution**: Make sure the file has `.html` extension, not `.txt`

**Issue 2: Styles not showing**
- **Solution**: Ensure you copied the entire HTML code including `<style>` tags

**Issue 3: Buttons not working**
- **Solution**: Check that JavaScript is enabled in your browser

**Issue 4: Display looks broken**
- **Solution**: Try opening in a different browser or clear browser cache

## 📝 Notes

- This is a **fun game** and should not be taken seriously for real relationships! 😄
- The game runs **entirely offline** - no internet connection required
- **No data is stored** - all calculations happen in your browser
- The game is **completely free** and open for personal use

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

### Ideas for Contribution:
- Add sound effects
- Create different themes (dark mode, light mode)
- Add more animations
- Create a history of calculations
- Add sharing functionality
- Translate to other languages

## 📄 License

This project is open source and available under the MIT License.

```
MIT License

Copyright (c) 2024 FLAMES Game

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 👨‍💻 Author

Created with ❤️ for fun and learning

## 🙏 Acknowledgments

- Inspired by the classic FLAMES game
- Built with modern web technologies
- Thanks to all contributors and users!

## 📞 Support

If you encounter any issues or have questions:
1. Check the [Troubleshooting](#troubleshooting) section
2. Open an issue on GitHub
3. Contact the maintainer

## 🎉 Have Fun!

Enjoy playing the FLAMES game and discover your relationship compatibility! Remember, it's all in good fun! 😊

---

**⭐ If you like this project, please give it a star on GitHub! ⭐**

---

*Last Updated: December 2024*