# Adding a permission to a group

To add a permission from a group, use this command:

``` text
/lp group <group> permission set <permission> true
```

Luckperms will infer you want to set the permission to `true`, so you don't have
to type the true:

```
/lp group <group> permission set <permission>
```

Using our example above, we can give the teleport permission to group
`moderator` like this:

``` text
/lp group moderator permission set minecraft.command.teleport
```

