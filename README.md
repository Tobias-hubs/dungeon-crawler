## Summary
This PR completes the implementation of the **Exercise 2 – Dungeon Crawler** game according to the assignment requirements.  
The project is a turn‑based CLI game built in Java, featuring a randomly generated dungeon, multiple enemy types, items, and a player inventory system.

## Key Features

### 🧩 OOP Principles
- **Encapsulation**: Private/protected fields with getters/setters; inventory managed via dedicated methods.
- **Inheritance**: `Player` and `Enemy` extend `Character`; multiple enemy subclasses (`Goblin`, `Ghost`, `Troll`, `Dragon`).
- **Polymorphism**: Abstract methods (`getAttackDamage`, `takeTurn`) overridden in subclasses; `Combat` works with `Character` references.

### 🗺 Dungeon Map
- `DungeonGrid` with walls, floor tiles, and printed map view.

### 🎲 Random Generation
- `RandomGeneration` ensures valid placement of enemies and items.

### ⚔ Game Mechanics
- Movement with collision detection.
- Combat system with both interactive (`start`) and test‑friendly (`doAttack`) modes.
- Inventory management and item usage (`HealthPotion`).

### 🧪 Testing (JUnit 5)
1. **Movement logic** – verifies player cannot move through walls.  
2. **Combat calculations** – verifies enemy HP decreases after attack.  
3. **Item effects** – verifies potion use increases player HP.  
4. **Map generation** – verifies random positions are in‑bounds and not walls.

---

## Additional Notes
- Removed unused classes and commented out debug prints for a clean submission.
- All four unit tests pass successfully. 
- School assignment Issue
[Exercise 2 - Dungeon Crawler](https://github.com/fungover/exercise2025/issues/6)
