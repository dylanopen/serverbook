# Adding temporary permissions

You can set a permission for a player, but only for a certain amount of time,
using this syntax:

``` text
/lp user <player> permission settemp <permission> <true/false> <duration>
```

For example, to give `Minecraft123` permission to use the `/ban` command but
*only for two days*:

``` text
/lp user Minecraft123 permission settemp minecraft.command.ban true 2d
```

Or, to prevent them from using the `/tell` command for 5 minutes:

``` text
/lp user Minecraft123 permission settemp minecraft.command.tell false 5m
```
