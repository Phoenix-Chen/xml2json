# XML2JSON

### What is this repo for?
This repo contains the sources for the competition at https://www.topcoder.com/challenge-details/30052650/?type=develop

### How to use this repo?
1. Clone this repo
2. Install the python dependencies (see instructions below)
3. Run the server (refer to entry point)
4. Fork and make pull requests to propose changes to this repo

### Installing python requirements
```bash
pip install -r requirements.txt
```

### Requirements
```python >= 2.6```

### Entry point
```bash
./run-server.sh   # Installs dependencies and spins up the server.
```

### Test in local
1. Run CouchDB:
```bash
couchdb```
2. Run server:
```bash
./run-server.sh   # Installs dependencies and spins up the server.
```
3. You can use any api testing app. Here, we use Postman:

Post:
Make post request at:
```http://localhost:5000/api/save```
In the Body tab, you can choose to input as raw (xml string) or binary (xml file). Then send. You’ll get a response:
```{"message": "processing feed"}```

Get:
Make get request at:
```http://localhost:5000/api/game/game_id```
Replace the game_id with the number of game_id 