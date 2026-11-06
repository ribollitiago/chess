# Chess

A fully functional console-based chess game built in Java, featuring object-oriented design with board abstraction, piece hierarchy, and core chess rule enforcement including check detection.

---

## Highlights

- Full 8×8 board representation with coordinate mapping (`ChessPosition` ↔ `Position`)
- Piece hierarchy: abstract `Piece` → `ChessPiece` → concrete pieces (King, Rook, …)
- Check detection and legal-move filtering
- Custom `BoardException` / `ChessException` for domain-level error handling
- Interactive console UI with colored output via `UI.java`

---

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Java 17+ |
| IDE | Eclipse |
| Architecture | OOP — Inheritance & Encapsulation |
| UI | Console (ANSI color) |

---

## Project Structure

```
src/
├── boardgame/
│   ├── Board.java          # Board state and piece placement
│   ├── BoardException.java
│   ├── Piece.java          # Abstract piece base
│   └── Position.java       # Matrix coordinate
├── chess/
│   ├── ChessMatch.java     # Game loop & rule engine
│   ├── ChessPiece.java     # Chess-specific piece base
│   ├── ChessPosition.java  # Algebraic notation (a1–h8)
│   ├── Color.java
│   └── pieces/
│       ├── King.java
│       └── Rook.java
└── application/
    ├── Program.java        # Entry point
    └── UI.java             # Console rendering
```

---

## Getting Started

### Prerequisites

- Java 17 or higher
- Eclipse IDE (or any Java IDE / `javac` CLI)

### Run via Eclipse

1. Clone the repository and import as an existing Eclipse project.
2. Run `application/Program.java` as a Java Application.

### Run via CLI

```bash
# From the project root (after compiling)
javac -d bin src/**/*.java
java -cp bin application.Program
```

---

## Author

**Tiago Ribolli Blasquez**  
[linkedin.com/in/tiagoribolli](https://linkedin.com/in/tiago-ribolli-blasquez-060810244) · [github.com/ribollitiago](https://github.com/ribollitiago)
