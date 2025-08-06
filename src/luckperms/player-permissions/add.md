# Adding a permission to a player

To add a permission from a player, use this command:

``` text
/lp user <player> permission set <permission> true
```

Luckperms will infer you want to set the permission to `true`, so you don't have
to type the true:

```
/lp user <player> permission set <permission>
```

Using our example above, we can give the teleport permission to user
`Minecraft123` like this:

``` text
/lp user Minecraft123 permission set minecraft.command.teleport
```

