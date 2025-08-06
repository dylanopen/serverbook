# Exclude parameter

The `exclude` parameter allows us to narrow down our search by *ignoring* events
that match a specific item, block, entity type **or player**.

The ability to ignore players makes this incredibly useful for cases such as
*checking for stealing from chests*, as you can exclude the owner from the
lookup so any stealing is immediately obvious.

## Types of exclude parameters

The `include` parameter can be any one of:

- a block
- an item
- an entity
- **a player**

## Specifying multiple patterns

Sometimes, you don't want to just exclude up a single item but rather a list of
items. You can do this by separating the different item IDs using a comma, for
example:

```
include:stone,cobblestone,smooth_stone
```

## Example: excluding a shop owner from a lookup

```
/co lookup radius:5 action:container time:3d exclude:Minecraft123
```

## Example: excluding multiple shop owners from a lookup

```
/co lookup radius:5 action:container time:3d exclude:Minecraft123,Minecraft456
```


