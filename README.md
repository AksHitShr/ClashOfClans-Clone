Clash Of Clans (Clone)

- To run the game : `python3 game.py`
- To view replays : `python3 replay.py`  and select the replay you want to watch according to mentioned date and time.
- For Victory : All buildings apart from walls get destroyed from the map in all three levels.
- For Defeat : If all troops and King die before destroying all buildings apart from walls.

## Controls :

### Hero :

- w : move up
- a : move left
- d : move right
- s : move down
- 1 : Special Attack
- space : Normal Attack

### Barbarian :

- z : spawn at point 1
- x : spawn at point 2
- c : spawn at point 3

### Dragon :

- v : spawn at point 1
- b : spawn at point 2
- n : spawn at point 3

### Archer :

- i : spawn at point 1
- o : spawn at point 2
- p : spawn at point 3

### Balloon :

- j : spawn at point 1
- k : spawn at point 2
- l : spawn at point 3

### StealthArcher :

- t : spawn at point 1
- u : spawn at point 2
- f : spawn at point 3 

### Healer :

- 6 : spawn at point 1
- 7 : spawn at point 2
- 8 : spawn at point 3

q : Quit Game

## Assumptions :

- Rage and Heal Spell can be applied multiple times.
- The limit for troops in each level is as follows :
    - Barbarians : 10
    - Archers : 7
    - Balloon : 5
    - Dragon : 3
    - StealthArchers : 7
    - Healers : 5
- You have to choose the type of troop movement at start of the game.
- You have to choose the hero after each level.
- Stealth Archer is white in color till it is invisble to the attacking buildings and becomes magenta after 10 seconds to indicate
- Healer heals like Wizard Tower damages. It targets a troop in a 7 tile range and then heals it, along with other troops in a 3x3 square area with the initial troop in the middle.
- Healer will not move (stays at a point) until it finds a troop whose health is less than its max_health (i.e. target only if health < max_health)
- Explosive damage done by walls only to ground troops (including hero king/queen) in a 5x5 tile area (any grounded troop with x between [wall.x-2,wall.x+2] and y between [wall.y-2, wall.y+2])
- Healer will not follow the closest troop if its health is low but it is inside the 7 tile range as it can still heal it from back.
- Levels for cannons,walls and wizard Towers have been hard coded and assigned to village class and their attributes are changed depending on this level.
- Healer only heals troops other than healers.
- Number of Healers limited to 5 and Stealth Archers limited to 7.
