# Zombie Hole Punching. Game "Winter is coming"

Hey, P2P Developer, we're challenging you to punch a hole!

## Requirements:
Build a Server which is able to accept Client sessions behind NAT

- Your friends can easily launch a [Game server](../README.md#game-rules) on their home machines
- You can connect to your friend's server and play from your home
- Session should be alive for prolonged period of time
- Don't implement logic of Game engine yet, server which handshakes only is totally ok

Task difficulty is for 1-2 days
- Choose a tool for problem solving. Prefer less infrastructure, your friends will be hosting game servers
- Choose a solution/library to punch a hole. Or implement another creative solution to solve a problem
- Only solve the problems scoped in the requirements
- Share code on VCS and send a link to jobs@mysterium.network

Bonus points for:
- If UDP protocol is used
- Demonstrated clean code with good readability

## Example

Server announces a contact where to connect (means of announcement is yours to choose):
```
./server
Game started. Players should join with './client SERVER_CONTACT'
```

Clients can connect by given contact:
```
./client SERVER_CONTACT
```

Server announces he accepted Client
```
HELLO
```
