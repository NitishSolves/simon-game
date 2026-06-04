# 🎮 Simon Says Game

A classic Simon Says memory game built with **vanilla HTML, CSS, and JavaScript**. Test your memory and beat your high score!

## 🎯 How to Play

1. **Start the Game**: Press any key on your keyboard to begin
2. **Watch the Pattern**: Simon will flash a random button in a sequence
3. **Repeat the Sequence**: Click the buttons in the same order Simon showed
4. **Level Up**: Each correct sequence adds one more button to remember
5. **Game Over**: If you click the wrong button, it's game over!
6. **Beat Your Score**: Try to reach a higher level and beat your personal high score

### Game Rules
- The sequence gets longer with each level
- You must click the exact buttons in the exact order
- If you make a mistake, the game ends and shows your score
- Press any key to try again and beat your high score
- The high score is tracked throughout your session

## 🎮 Game Interface

The game has 4 colored buttons:
- **Red** (Button 1)
- **Yellow** (Button 2)
- **Green** (Button 3)
- **Purple** (Button 4)

Watch for them to flash, then click in the correct sequence!

## ✨ Features

✅ Responsive button design  
✅ Sound-free gameplay (visual feedback only)  
✅ Real-time level counter  
✅ High score tracking per session  
✅ Color-coded buttons for visual clarity  
✅ Game-over detection with score display  
✅ Smooth animations and visual feedback  

## 🛠️ Tech Stack

- **HTML5** — Semantic structure
- **CSS3** — Flexbox layout, animations, and styling
- **JavaScript (ES6+)** — Game logic, event handling, DOM manipulation

## 📁 Project Structure

```
simon-game/
├── index.html      # Game markup
├── style.css       # Styling and animations
├── app.js          # Game logic
└── README.md       # This file
```

## 🚀 Getting Started

### Play Online
Visit the live demo: [https://nitishsolves.github.io/simon-game/]

### Play Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/NitishSolves/simon-game.git
   cd simon-game
   ```

2. Open in your browser:
   - Double-click `index.html`, OR
   - Use a local server (recommended):
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Python 2
     python -m SimpleHTTPServer 8000
     
     # Using Node.js (with http-server package)
     npx http-server
     ```
   - Then visit `http://localhost:8000`
   - 

## 📊 How the Game Works

### Game Flow
1. Player presses any key → `levelUp()` is called
2. A random button is selected and added to `gameSeq[]`
3. Button flashes (visual feedback)
4. Player clicks buttons → `btnPress()` is called
5. Each click is added to `userSeq[]` and checked via `checkAns()`
6. If correct, game waits 1 second then calls `levelUp()` again
7. If incorrect, game ends and resets

### Sequence Tracking
- `gameSeq[]` — Stores the pattern Simon generates
- `userSeq[]` — Stores the buttons you click in the current level
- `highScore` — Persists throughout your session

## 📝 License

This project is open source and free to use. Feel free to fork, modify, and redistribute!

## 👨‍💻 Author

Made with ❤️ by **Nitish** | [GitHub](https://github.com/NitishSolves)

---


**Have fun playing!🎯** ❤️
