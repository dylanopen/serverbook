# Whitelisting bedrock players

There are two options for whitelisting bedrock players:

1. Turn off the whitelist, allow them to join, add the user to the whitelist and
   then turn back on the whitelist
2. Use the `/fwhitelist` (floodgate whitelist) command.

## /fwhitelist add

You can add players to the whitelist using the `/fwhitelist add` command. For
example:

```
/fwhitelist add Bedrock123
```

> Note above that we **do not** add the dot before the user's name, like you
  would if using the default `/whitelist` command.

Running that will allow the `Bedrock123` user to join, if they have a Microsoft
account linked to their Minecraft profile.

> Important note: the `/fwhitelist` command requires a player to have joined a
  Geyser server before. If they have never connected to any Geyser server, this
  command will fail and you will need to first temporarily disable the
  whitelist to allow them to join.

## /fwhitelist remove

Similar to the default `/whitelist` command, you can remove players from the
whitelist. For example:

```
/fwhitelist remove Bedrock123
```

> Note again that we **do not** add the dot before the user's name, like you
  would if using the default `/whitelist` command.

