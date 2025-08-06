# Plugin installation

Install Simple Voice Chat like you would any other plugin: to do it manually,
upload the `jar` file to your server's `plugins` directory.

> <https://modrinth.com/plugin/simple-voice-chat>

## Configuration

You shouldn't need to do any extra configuration except for specifying the SVC
port.

1. Start your server and Simple Voice Chat will generate the
   `plugins/VoiceChat/config.yml` file.
2. Find the `port` field and change its value to be the port number you
   allocated in [the previous page](./port.md).
3. Save the config file and restart your server

> By default, members without `op` may not be able to hear other players or
  speak. Please see the [good starting permissions](./starting-permissions.md)
  page to fix this.

