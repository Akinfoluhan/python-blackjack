# 🃏 Blackjack Game (Python)

## Overview

This project is a Python implementation of Blackjack, a classic card game where players aim to achieve a hand value as close to 21 as possible without exceeding it.

The game simulates a standard round of Blackjack with one player and a dealer. The player chooses whether to hit (draw another card) or stand (end their turn), while the dealer follows a fixed rule set. Final outcomes are determined by comparing the player’s hand against the dealer’s hand.

The project emphasizes modular design, clear game logic, and testable components.

## Game Rules

### Dealing

- The player is dealt two cards at the start of the game.
- The player may hit as many times as desired.
- If the player’s hand value exceeds 21, they bust and automatically lose.

### Dealer Rules

- The dealer plays after the player’s turn is complete.
- The dealer must stand if their hand value is 17 or higher.
- The dealer must hit if their hand value is less than 17.
- The dealer continues hitting until they reach 17 or bust.

---

## Scoring Rules

- Face cards (Jack, Queen, King) are worth 10.
- Aces are worth 11.
- Number cards (2–10) are worth their face value.

---

## Game Outcomes

At the end of the round, the player receives one of the following outcomes:

- Win: the player does not bust and has a higher hand value than the dealer.
- Lose: the player busts or has a lower hand value than the dealer.
- Push: the player does not bust and ties with the dealer.

---

## Features

- Modular game architecture with separate components for player logic, dealer behavior, card values, and outcome evaluation
- Turn-based gameplay with user input
- Automatic dealer logic based on standard Blackjack rules
- Unit and integration tests validating core game behavior

---

## Project Structure

`````md
src/
├── blackjack.py
├── blackjack_helper.py
├── dealer.py
├── user.py
├── value.py
├── name.py
├── end_status.py

tests/
├── unit_test_helper.py
├── unit_test_blackjack_helper.py
├── integration_test_helper.py
├── integration_test_blackjack.py

---

````md
## Tech Stack

- Language: Python
- Concepts:
  - Object-oriented programming
  - Modular design
  - Control flow and game state management
  - Unit and integration testing

---

## Running the Game

```bash
python src/blackjack.py
```

---

## Testing

Unit and integration tests are included to verify game logic and outcomes.

```bash
pytest
```

---

## Future Improvements

- Dynamic Ace handling (1 or 11)
- Support for multiple players
- Betting system and chip tracking
- Graphical user interface
- Improved input validation
````
`````
