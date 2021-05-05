# FollowingMusic


## Technologies used
- [Mopidy](https://mopidy.com/) - Mopidy is an extensible music server written in Python. Mopidy plays music from local disk, Spotify, SoundCloud, TuneIn, and more. 
- [Snapcast](https://github.com/badaix/snapcast) - Snapcast is a multiroom client-server audio player, where all clients are time synchronized with the server to play perfectly synced audio. It's not a standalone player, but an extension that turns your existing audio player into a Sonos-like multiroom solution. Audio is captured by the server and routed to the connected clients.
- [Node-beacon-scanner](https://github.com/futomi/node-beacon-scanner) - The node-beacon-scanner is a Node.js module which allows you to scan BLE beacon packets and parse the packet data. This module supports iBeacon, Eddystone, and Estimote.
- [Paho MQTT](https://pypi.org/project/paho-mqtt/) - Python library for handling the MQTT protocol, which is responsible for communication between the server and individual clients
- [Noble](https://github.com/abandonware/noble) - A Node.js BLE (Bluetooth Low Energy) central module.


# Installation TODO

# Run
On main device run **server.py** script using:
```
python server.py
```
And run Snapcast server:
```
snapserver
```

On devices in rooms run **scanner.js** script using:
```
node scanner.js <room_name> <uuid_beacon_list>
```

And Snapcast client using:
```
snapclient --hostID <room_name>
```

You also need a BLE Beacon, there are apps simulating it or you can just buy one