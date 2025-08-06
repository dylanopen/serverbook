# Geyser configuration

Restart your server and Geyser should generate its `config.yml` file in the
`plugins/Geyser-Spigot` folder.

Search for the `port` field and set that to whichever port number you allocated
and noted down earlier.

Importantly, if you are using [Floodgate](../floodgate.md), you
**must** set these config options in that file:

``` yml
address: auto
auth-type: floodgate
```

You can also set the MOTD and server name to change how your server appears in
the bedrock server listings.

