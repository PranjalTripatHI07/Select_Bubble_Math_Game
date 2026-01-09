# 🫧 Bubble Math Game - Cognitive Assessment

A web-based Bubble Math Game that replicates the **Cognitive Assessment – Bubble Math Game (2026 pattern)**. Built with vanilla HTML, CSS, and JavaScript.

![Bubble Math Game](https://img.shields.io/badge/Version-1.0-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![Platform](https://img.shields.io/badge/Platform-Web-orange)

---

## 🎯 Objective

Mentally solve arithmetic expressions displayed inside floating bubbles and select them in the correct numerical order (**lowest to highest**) within a strict **15-second time limit** per question.

---

## ✨ Features

### 🧠 Game Structure
- **25 Questions** - Complete all rounds to finish the assessment
- **3 Floating Bubbles** - Each question displays 3 bubbles with arithmetic expressions
- **Triangle Layout** - Bubbles arranged in pyramid formation (1 top, 2 bottom)
- **Auto-Transition** - Questions transition immediately upon completion or timeout

### 🔢 Expression Types
| Type | Example |
|------|---------|
| Integers | `8 + 5`, `12 × 3` |
| Decimals | `3.5 + 2.1`, `4.25 ÷ 1.5` |
| Fractions | `1/2 + 3/4`, `2/3 × 5/6` |
| Mixed | `2.5 × 1/2`, `3.75 + 2/5` |

### ➕ Supported Operations
- Addition (+)
- Subtraction (−)
- Multiplication (×)
- Division (÷)

*No other operations (powers, roots, modulus, etc.) are permitted.*

---

## 📈 Adaptive Difficulty

The game silently adapts difficulty based on your performance:

### Adaptivity Signals
| Signal | Description |
|--------|-------------|
| Selection Accuracy | Tracks correct vs incorrect bubble selections |
| Completion Speed | Monitors average response time per question |
| Error Rate | Counts number of incorrect selections |

### Adaptive Controls
| Control | Easy → Hard |
|---------|-------------|
| Number Range | 15 → 50 |
| Decimal Precision | 0 → 1 → 2 decimal places |
| Fractions | Disabled → Enabled (Q8+) |
| Mixed Expressions | Disabled → Enabled (Q12+) |
| Operator Mixing | Simple → Complex combinations |

*Difficulty adjusts automatically with no visible indicator.*

---

## 🔁 No-Repetition Rule

- No arithmetic expression repeats across all 25 questions
- Uniqueness considers operands, operator, and structure
- Commutative expressions are treated as duplicates (e.g., `6 + 4` = `4 + 6`)
- Global expression history ensures uniqueness

---

## ⏱ Timing Rules

| Rule | Value |
|------|-------|
| Time Limit | 15 seconds per question |
| Timer Display | Live circular countdown |
| Warning State | Red timer when ≤5 seconds remain |
| Transition | Immediate (no pause between questions) |

---

## ✅ Visual Feedback

| Selection | Visual |
|-----------|--------|
| Correct | 🟢 Bubble turns green with pulse animation |
| Incorrect | 🔴 Bubble turns red with shake animation |
| Selected Order | Badge shows selection number (1, 2, 3) |

---

## 📊 Performance Tracking

### During Game
- Question progress (1-25)
- Correct selections count
- Incorrect selections count
- Accuracy percentage
- Perfect questions count
- Wrong questions count

### Final Results
- Final Score (weighted by accuracy + speed)
- Overall Accuracy %
- Correct/Incorrect Selections
- Average Response Time
- Questions Completed
- Perfect Questions
- Wrong Questions

---

## 🎨 UI/UX Features

- Clean, professional assessment-style interface
- Smooth floating bubble animations
- High-contrast, readable equations
- Circular progress timer
- Progress bar showing game completion
- Desktop-first responsive layout
- Mobile-friendly (140px bubbles on smaller screens)

---

## 🚀 Getting Started

### Play Online
Simply open `index.html` in any modern web browser.

### Local Development
```bash
# Clone the repository
git clone https://github.com/PranjalTripatHI07/Bubble-Game-.git

# Navigate to the directory
cd Bubble-Game-

# Open in browser
open index.html
# or
start index.html  # Windows
```

---

## 🛠 Technical Details

### Technologies
- **HTML5** - Structure
- **CSS3** - Styling, animations, responsive design
- **Vanilla JavaScript** - Game logic, no external libraries

### Key Implementation
- No external math evaluation libraries
- Accurate decimal and fraction handling
- Reliable timer with interval management
- Set-based expression uniqueness tracking
- Fisher-Yates shuffle for bubble randomization

### Browser Support
- Chrome (recommended)
- Firefox
- Safari
- Edge

---

## 📁 Project Structure

```
Bubble-Game-/
├── index.html    # Complete game (HTML + CSS + JS)
├── README.md     # Documentation
└── LICENSE       # MIT License
```

---

## 🎮 How to Play

1. **Start** - Click "Start Game" on the welcome screen
2. **Calculate** - Mentally solve each expression in the bubbles
3. **Select** - Click bubbles from **lowest to highest** value
4. **Repeat** - Complete all 25 questions
5. **Results** - View your final score and performance stats

### Tips
- Start calculating as soon as bubbles appear
- Watch the timer - you have exactly 15 seconds
- Wrong selections still count, so be careful!
- The game adapts - perform well and it gets harder

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Pranjal Tripathi**

- GitHub: [@PranjalTripatHI07](https://github.com/PranjalTripatHI07)

---

## 🙏 Acknowledgments

- Inspired by Accenture Cognitive Assessment (2026 Pattern)
- Built for practice and educational purposes

---



