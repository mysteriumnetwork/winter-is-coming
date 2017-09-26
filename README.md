Technical task “Winter is coming”

Build Game Engine (Server), which is able to establish bidirectional communication channel with Game Participant (Client).

The game:
- There is a board of 10x30 cells (like chess board), one side of the broad has Zombie army, another has Wall with Archers on it.
- Zombie Army sends one attacker towards The Wall and Zombie is aiming is to reach The Wall
- Archers are trying to shoot Zombie from The Wall
- If Zombie dies or reaches The Wall, new Zombie starts to walk thru a board

Game logic:
- If Game Participant joins to Game Engine, new board is created and Zombie rush is started for this Game Participant
- Game Engine announces Zombie’s coordinates to communication channel every 2 seconds
- Every 2 seconds Game Participant is allowed to send coordinates for Archer to shoot
- Game Engine sends message if Zombie was killed, another message when Zombie reached the Wall
- After 5 games Game Engine stops the game
 
Recommendations:
- Don’t spend more than 2 days