# Block action

Block actions are called whenever any blocks are created or destroyed in the
world.

CoreProtect logs block events from many sources: creeper and TNT explosions,
worldedit commands, etc, not just from players.

## Syntax

You can use the block action query in one of these two ways:

```
action:block
a:block
```

## Example lookup

```
/co lookup action:block ...
```

## Block place action

To overspecify the action type to only return results for block *place* events,
you can use the `+block` action:

```
/co lookup action:+block ...
```

This will *only* return results for block place events, and block break events
will be ignored.

## Block break action

To overspecify the action type to only return results for block *break* events,
you can use the `-block` action:

```
/co lookup action:-block ...
```

This will *only* return results for block break events, and block place events
will be ignored.

