# Explicit false player permissions

Some commands are available to everyone by default, even if they are not an
operator.

For example, the `/plugins` command is available to everyone by default on
Bukkit servers, but you might not want this.

To explicitly block a command, use:

``` text
/lp user <player> permission set <permission> false
```

For example, to block `Minecraft123` from using `/plugins`, you can use:

``` text
/lp user Minecraft123 permission set minecraft.command.plugins false
```
