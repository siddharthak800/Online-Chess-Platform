# ChessConnect - Real-time Chess Game 👑

A web-based chess application that enables real-time gameplay between two players using different browsers. Built with JavaScript, HTML, and CSS, featuring live game updates, move validation, and interactive UI.


## Features ✨

- **Real-time Gameplay**
  - Live game updates across browsers
  - WebSocket connection for instant moves
  - No refresh needed
  - Player status indicators

- **Chess Logic**
  - Complete chess rule implementation
  - Valid move highlighting
  - Check and checkmate detection
  - Pawn promotion
  - En passant and castling
  - Move history tracking

- **Game Features**
  - Player matchmaking
  - Game clock/timer
  - Move notation
  - Piece capture display
  - Game state saving
  - Rematch options

- **User Interface**
  - Responsive chess board
  - Drag and drop pieces
  - Move highlighting
  - Legal move indicators
  - Game chat system

## Tech Stack 🛠️

- **Frontend**
  - HTML5
  - CSS3 (with Flexbox/Grid)
  - JavaScript (ES6+)
  - WebSocket API

- **Real-time Communication**
  - Socket.io/WebSocket
  - JSON for data transfer

- **Game Assets**
  - SVG chess pieces
  - Custom sound effects
  - Responsive board design

## Live Demo 🎮
Try it live: [ChessConnect Demo](https://your-demo-link.com)

## Installation 🚀

1. Clone the repository:
https://github.com/siddharthak800/Online-Chess-Platform.git

2. Install dependencies:
   ```bash
   npm install (install from imports)
   ```

3. Set up WebSocket server:
   ```bash
   npm install socket.io
   ```

4. Start the server:
   ```bash
   npm start
   ```

5. Open in browser:
   - Navigate to `http://localhost:3000`
   - Open another browser window for the second player


## Gameplay Instructions 🎯

1. **Starting a Game**
   - Visit the website
   - Click "New Game" or "Join Game"

2. **Making Moves**
   - Drag and drop pieces or click to select and move
   - Valid moves are highlighted in blue
   - Captured pieces show in the sidebar

3. **Game Features**
   - Use chat to communicate with opponent
   - View move history in algebraic notation
   - Clock shows remaining time for each player
   - "Resign" or "Offer Draw" buttons available

## Screenshots 📸

![chessplay](https://github.com/user-attachments/assets/10f69402-b8cf-4753-939c-a74d9e2e4d44)

## Game State Management 🎮

```javascript
class GameState {
    constructor() {
        this.board = this.initializeBoard();
        this.currentPlayer = 'white';
        this.moveHistory = [];
        this.capturedPieces = {
            white: [],
            black: []
        };
    }
    // ... additional methods
}
```

## Browser Support 🌐

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Optimizations ⚡

- Piece movement animations use CSS transforms
- WebSocket data compression
- Lazy loading of sound effects
- Efficient board state updates
- Minimal DOM manipulation

## Contributing 🤝

1. Fork the repository
2. Create a feature branch
   ```bash
   git checkout -b feature/NewFeature
   ```
3. Commit your changes
4. Push to the branch
5. Open a pull request

## Known Issues 🐛

- [ ] Safari mobile drag-and-drop occasionally unresponsive
- [ ] Rare WebSocket reconnection issues
- [ ] Clock sync delays on slow connections

## Future Enhancements 🚀

- AI opponent option
- Tournament system
- ELO rating system
- Game analysis tools
- Opening book integration
- Social features

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support 💬

For support and queries:
- Create a GitHub issue
- Email: support@chessconnect.com
- Discord: [Join our server](discord-link)

## Acknowledgments 🙏

- Chess.com for inspiration
- Socket.io team
- Chess piece SVG creators
- Open-source contributors

## Version History 📝

- v1.0.0
  - Initial release
  - Basic gameplay
  - Real-time functionality
- v1.1.0
  - Added game chat
  - Improved move validation
  - Mobile responsiveness
