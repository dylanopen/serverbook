# Removing permissions temporarily

You can temporarily remove a permission for a player (for only a certain amount
of time) using this syntax:

``` text
/lp user <player> permission unsettemp <permission> <duration>
```

For example, to remove `Minecraft123`'s permission to use the `/ban` command but
*only for two hours*:

``` text
/lp user Minecraft123 permission unsettemp minecraft.command.ban 2h
```

