# Tic Tac Toe - React Learning Project

A simple yet interactive Tic Tac Toe game built with React. This project serves as an excellent introduction to React fundamentals, including components, state management, event handling, and conditional rendering.

## 🎮 Project Overview

This is a beginner-friendly React project that implements the classic Tic Tac Toe game. It demonstrates core React concepts in a practical, engaging way, making it ideal for developers who are just starting their React journey.

### Key Features

- **Interactive Gameplay**: Play Tic Tac Toe against another player (two-player mode)
- **Game State Management**: Learn how React manages component state and updates the UI
- **Winner Detection**: Automatic detection of winning combinations
- **Game Reset**: Ability to restart the game and play again
- **Responsive Design**: Clean, user-friendly interface that works on different screen sizes
- **Move History**: Track game moves and understand React's data flow

## 🚀 Getting Started

### Prerequisites

- **Node.js** (version 14.0 or higher)
- **npm** (Node Package Manager) or **yarn**
- Basic knowledge of JavaScript and React concepts

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Wira-Kusuma/tic-tac-tue.git
   cd tic-tac-tue
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```
   or
   ```bash
   yarn install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```
   or
   ```bash
   yarn start
   ```

4. **Open your browser**
   - Navigate to `http://localhost:3000` to play the game

## 📚 Learning Concepts

This project helps you understand and practice the following React concepts:

### 1. **Components**
   - Functional components
   - Component composition
   - Props passing

### 2. **State Management**
   - Using the `useState` hook
   - Updating state based on user interactions
   - Managing game board state

### 3. **Event Handling**
   - Click event handlers
   - Event propagation
   - Function binding in React

### 4. **Conditional Rendering**
   - Displaying different content based on game state
   - Showing winner announcements
   - Displaying current player turn

### 5. **Data Flow**
   - One-way data binding in React
   - Passing state and callbacks to child components
   - Lifting state up to parent components

### 6. **Array Methods**
   - Using `.map()` to render lists
   - Using `.slice()` to create copies of arrays
   - Array manipulation for game logic

## 🎯 How to Play

1. **Start the Game**: The game board will appear with an empty 3x3 grid
2. **Take Turns**: Player X goes first, followed by Player O
3. **Win the Game**: Get three of your marks in a row (horizontally, vertically, or diagonally)
4. **Draw**: If all squares are filled with no winner, the game ends in a draw
5. **Play Again**: Click the reset button to start a new game

## 📁 Project Structure

```
tic-tac-tue/
├── src/
│   ├── App.jsx
│   ├── App.css
│   ├── index.js
│   └── index.css
├── public/
│   ├── index.html
│   └── favicon.ico
├── package.json
└── README.md
```

## 💡 Key Concepts Explained

### State Hook (useState)
```javascript
const [board, setBoard] = useState(Array(9).fill(null));
const [isXNext, setIsXNext] = useState(true);
```

### Event Handling
```javascript
const handleClick = (index) => {
  if (board[index] || calculateWinner(board)) {
    return;
  }
  const newBoard = [...board];
  newBoard[index] = isXNext ? 'X' : 'O';
  setBoard(newBoard);
  setIsXNext(!isXNext);
};
```

### Conditional Rendering
```javascript
const winner = calculateWinner(board);
const status = winner 
  ? `Winner: ${winner}` 
  : `Next Player: ${isXNext ? 'X' : 'O'}`;
```

## 🔧 Technologies Used

- **React**: JavaScript library for building user interfaces
- **JavaScript (ES6+)**: Modern JavaScript features
- **CSS**: Styling the game interface
- **Create React App**: Project setup and build tool

## 📖 Resources for Learning

- [React Official Documentation](https://react.dev)
- [React Hooks Guide](https://react.dev/reference/react/hooks)
- [JavaScript ES6 Features](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)
- [React Tutorial - Tic Tac Toe](https://react.dev/learn/tutorial-tic-tac-toe)

## 🚀 Next Steps & Enhancements

After completing this basic project, consider implementing these features:

- **Single Player Mode**: Add AI opponent (difficulty levels)
- **Score Tracking**: Keep track of wins across multiple games
- **Move History**: Display previous moves and allow going back
- **Animations**: Add smooth transitions and game state animations
- **Sound Effects**: Include sound for clicks and game events
- **Difficulty Levels**: Implement different AI strategies
- **Game Statistics**: Track win/loss/draw statistics
- **Local Storage**: Save game data persistently

## 🤝 Contributing

This is a learning project! Feel free to:
- Fork the repository
- Create feature branches for new enhancements
- Submit pull requests with improvements
- Share your learning experience

## 📝 License

This project is open source and available under the MIT License. Feel free to use it for learning purposes.

## 👨‍💻 Author

**Wira-Kusuma** - Learning React with practical projects

---

## 🎓 Conclusion

This Tic Tac Toe project is a fantastic starting point for learning React. It covers essential concepts in a fun, interactive way. As you progress, you'll understand how to build more complex React applications by mastering these fundamentals.

Happy coding and enjoy your React learning journey! 🚀

---

**Last Updated**: December 18, 2025