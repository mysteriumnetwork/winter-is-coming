# Talk to Zombies. Game "Winter is coming"

Hey, Backend Engineer, we'd like you to build a simple game engine! :)

## Requirements:
Build a Server which is able to establish bidirectional communication channel with a Game Participant (Client)

- [Game rules](../README.md#game-rules)
- Your friends can easily launch a server on their machines
- You can connect to your friend's server and play from your home
- Dont create a Client yet. Anyway your chosen protocol will be testable with *telnet*, *curl*, *Postman* etc.
- Client can start a game via communication channel
- Server announces Zombie’s coordinates to communication channel every 2 seconds
- Client sends coordinates of the Archer's shot

Task difficulty is for 1-2 days
- Choose a tool for problem solving
- Choose a technology/solution/library for the bidirectional communication channel
- Demonstrate your most clean code with good readability
- Only solve the problems scoped in the requirements
- Share code on VCS and send a link to jobs@mysterium.network

## Communication channel example
```
# Client send Archer's name
START john
```

```
# Server announces coordinates
WALK night-king 0 0
WALK night-king 0 1
WALK night-king 1 1
WALK night-king 1 2
WALK night-king 1 3
...
```

```
# Client sends Archer's coordinates
SHOOT 0 0
# Server responds with Archer's result
BOOM john 0
BOOM john 1 night-king
```
