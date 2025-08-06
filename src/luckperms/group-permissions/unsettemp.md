# Removing permissions temporarily

You can temporarily remove a permission for a group (for only a certain amount
of time) using this syntax:

``` text
/lp group <group> permission unsettemp <permission> <duration>
```

For example, to remove `Moderator`'s permission to use the `/ban` command but
*only for two hours*:

``` text
/lp group Moderator permission unsettemp minecraft.command.ban 2h
```

