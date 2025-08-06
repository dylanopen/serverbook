# Include parameter

The `include` parameter allows us to *massively* narrow down our search by only
including events that match a specific item, block or entity type.

## Types of include parameters

The `include` parameter can be any one of:

- a block
- an item
- an entity

## Specifying multiple patterns

Sometimes, you don't want to just look up a single item but rather a list of
items you want to check. You can do this by separating the different item IDs
using a comma, for example:

```
include:stone,cobblestone,smooth_stone
```

## Example: rolling back diamond blocks

For example, we could roll back only events that a user called `Minecraft123`
did and that included a `diamond_block` item, by 3 days, like this:

```
/co rollback user:Minecraft123 include:diamond_block time:3d
```


