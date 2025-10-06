# Matchmaking Simulator

Small, dependency-free Java matchmaking simulator demonstrating a greedy skill-based matcher and tiny HTTP API.

## Demo
Add a short demo GIF at `docs/demo.gif` showing:
- starting the server
- submitting a few /join requests
- inspecting /queue and /matches

## Quickstart
```bash
git clone https://github.com/[github-username]/matchmaking-simulator.git
cd matchmaking-simulator
chmod +x run_local.sh
./run_local.sh
# in another terminal:
curl -X POST "http://localhost:8080/join?playerId=alice&skill=2200"
curl -X POST "http://localhost:8080/join?playerId=bob&skill=2180"
curl http://localhost:8080/queue
curl http://localhost:8080/matches
