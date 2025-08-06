# Group inheritance

If you want one group to take all permissions from another (and then possibly
add some) run this command:

``` text
/lp group <group> parent set <parentGroup>
```

For example, to make the `admin` group inherit from the `moderator` group:

``` text
/lp group admin parent set moderator
```

> You should **always** inherit from at least one group (which itself will
  inherit from the `default` group). If a group doesn't have a logical parent,
  you should instead make it inherit from the `default` group.

## Setting group weight

Each group has a weight. When LuckPerms decides what permission it has, it will
prioritise the permissions of higher-weighted groups.

For example, if the `moderator` group specifically *prevents access* to the
`/tp` command but the `admin` group allows it, if `admin` has a higher weight,
then players with `admin` will have that permission, as `admin` takes priority
over `moderator`.

You can set a group's weight like this:

``` text
/lp group <group> setweight <weight>
```

... where `<weight>` is a number.

