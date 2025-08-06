# Explicit false group permissions

Some commands are available to everyone by default, even if they are not an
operator.

For example, the `/plugins` command is available to everyone by default on
Bukkit servers, but you might not want this.

To explicitly block a command, use:

``` text
/lp group <group> permission set <permission> false
```

For example, to block `Moderator` from using `/plugins`, you can use:

``` text
/lp group Moderator permission set minecraft.command.plugins false
```
