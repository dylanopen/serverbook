# Adding temporary permissions

You can set a permission for a group, but only for a certain amount of time,
using this syntax:

``` text
/lp group <group> permission settemp <permission> <true/false> <duration>
```

For example, to give `Moderator` permission to use the `/ban` command but
*only for two days*:

``` text
/lp group Moderator permission settemp minecraft.command.ban true 2d
```

Or, to prevent them from using the `/tell` command for 5 minutes:

``` text
/lp group Moderator permission settemp minecraft.command.tell false 5m
```
