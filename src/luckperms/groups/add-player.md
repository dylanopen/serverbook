# Adding a player to a group

``` text
/lp user <player> parent add <group>
```

Note that we use `parent add` here instead of `parent set`: that's because you
usually want to keep somebody's existing groups, but just add another. If you
want to delete all groups from a player and just have the new one, use `parent
set` instead.
