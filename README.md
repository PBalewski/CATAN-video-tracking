# CATAN Elements Detection & Tracking

## Project Overview
This project focuses on detecting and tracking game elements in video recordings of the board game **Catan**. The goal is to analyze different phases of the game by recognizing in-game objects, tracking their movement, and handling various video conditions.

## In-Game Elements Tracked
### **Counters/Markers**
- **Robber token** (1 piece)
- **Number tokens** (18 circular tokens, marked 2–12 excluding 7)

### **Dice**
- **Standard dice** (2 six-sided dice, used to determine resource production)

### **Cards**
- **Resource cards** (95 total: Brick, Lumber, Grain, Ore, Wool)
- **Development cards** (25 total: Knight, Victory Point, Monopoly, Year of Plenty, Road Building)

### **Boards**
- **Hexagonal terrain tiles** (19 hexes: 5 resource types + 1 desert tile)
- **Frame (Border pieces)** (6 interlocking border pieces)

### **Figures (Player Pieces)**
- **Settlements** (20 small house-shaped pieces, 5 per player)
- **Cities** (16 larger building-shaped pieces, 4 per player)
- **Roads** (60 long rectangular pieces, 15 per player)

### **Tokens**
- **Longest Road token** (1 piece)
- **Largest Army token** (1 piece)

## Event Detection & Tracking
### **Game Events Tracked**
- **Rolling Dice & Resource Collection**  
  - Detect dice roll values and track resource distribution to players.
- **Development Card Play**  
  - Detect when a player reveals a Knight, Victory Point, or special action card.
- **Building Construction**  
  - Track new roads, settlements, and cities appearing on the board.
- **Resource Collection**  
  - Identify hexes producing resources and detect Robber placement impact.
- **Game Start & End Conditions**  
  - Detect initial settlement placements and victory conditions.

## Dataset Description
The dataset consists of **9 video clips** categorized into three difficulty levels based on recording conditions:
1. **Easy**: Well-lit, stable camera, directly overhead view.
2. **Medium**: Minor issues like shadows or slight camera tilt.
3. **Hard**: Rotated board, noticeable shadows, occasional camera shake.

Each video captures different game phases, making the dataset useful for training object detection and tracking models.

## Technologies Used
- **Computer Vision** (OpenCV)
- **Python** (NumPy, SciPy)
- **Video Processing** (OpenCV for frame extraction & tracking)

## Usage Instructions
1. Load video datasets and preprocess frames.
2. Apply object detection to identify game elements.
3. Track element movement and interactions over time.
4. Output insights such as detected moves, resource distributions, and game progress visualization.

---
**Authors**: Piotr Balewski 156037, Kuba Czech 156035
**Date**: January 2025
