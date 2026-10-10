# pof-pack

The resource pack for the Pillars of Fortune server. Nothing else lives here.

## Current pack

The plugin sends the pack to players itself. Each plugin build knows the exact
file made for it, by name, and that name is the file's SHA-1:

```
packs/<sha1>.zip
https://raw.githubusercontent.com/flayniks/pof-pack/main/packs/<sha1>.zip
```

A file in `packs/` never changes once it is here - a new pack gets a new name -
so an older plugin build keeps working while a newer one uses the newer pack.

With the current plugin, the `resource-pack=` and `resource-pack-sha1=` lines
in server.properties should be **empty**.

## Old pack

`PillarsOfFortune-Resources.zip` at the top is the pack from before the plugin
sent it. It is left exactly as it was so a server still pointing at it with
its old hash keeps working until the plugin is updated. Newer clients (26.2)
reject that pack's pack.mcmeta, which is why its textures show purple and
black; the packs in `packs/` fix that.
