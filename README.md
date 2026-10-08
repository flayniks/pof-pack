# pof-pack

The resource pack for the Pillars of Fortune server. Nothing else lives here.

The server downloads it from:

```
https://raw.githubusercontent.com/flayniks/pof-pack/main/PillarsOfFortune-Resources.zip
```

`resource-pack-sha1` in server.properties has to match this file byte for byte.
If you replace the zip, update the hash too, or every player's download is
refused:

```
sha1sum PillarsOfFortune-Resources.zip
```
