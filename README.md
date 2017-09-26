# Game "Winter is coming"

Hey, Backend developer, can You build Game Engine?

## The game:
- There is a board of 10x30 cells (like chess board), one side of the broad has Zombie, another side has Wall with Archer on it.
- Zombie is walking through the board, aiming to reach The Wall
- Archer is trying to shoot walking Zombie from The Wall
- Zombie dies or reaches The Wall

**Destiny of corrupted Westeros is your hands!**

## Requirements:
Build Server which is able to establish bidirectional communication channel with Game Participant (Client)

- Your friends can easily launch Server on threir machines
- You can connect to your friend's Server and play from your home
- Dont create Client yet, your chosen protocol should be checkable (telnet, curl, Postman etc.)
- Client can start a game via communication channel
- Server announces Zombie’s coordinates to communication channel every 2 seconds
- Client sends coordinates of Archer's shoot

Task difficulty is for 1-2 days
- Choose tool for problem solving
- Choose technology/solution/library for bidirectional communication channel
- Solve just problems scoped in requirements
- Share Clean and readable code on VCS and send a link to jobs@mysterium.network

## Communication channel example
```
# Client send Archer's name
START john
```

```
# Server announces coordinates
WALK night-king 0 0
WALK night-king 0 2
WALK night-king 2 2
WALK night-king 2 4
WALK night-king 2 6
...
```

```
# Client sends Archer's coordinates
SHOOT 0 0
# Server responds with Archer's result
BOOM john 0
BOOM john 1 night-king
```