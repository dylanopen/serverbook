# Removing a permission from a group

To remove a permission from a group, use this command:

``` text
/lp group <group> permission unset <permission>
```

Using our example above, we can remove the teleport permission from
`Moderator` like this:

``` text
/lp group Moderator permission unset minecraft.command.teleport
```
