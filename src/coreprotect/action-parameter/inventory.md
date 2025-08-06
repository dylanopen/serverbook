# Inventory action

Inventory actions are called whenever any item leaves or enters a player's
inventory.

## Syntax

You can use the inventory action query in one of these two ways:

```
action:inventory
a:inventory
```

## Example lookup

```
/co lookup action:inventory ...
```

## Example: rolling back diamonds

```
/co rollback user:Minecraft123 action:inventory include:diamond time:90m
```

## Inventory item insert action

To overspecify the action type to only return results for *item add* events,
you can use the `+inventory` action:

```
/co lookup action:+inventory ...
```

This will *only* return results for inventory item insert (gain) events, and
item removal events will be ignored.

## Inventory item remove action

To overspecify the action type to only return results for *item remove* events,
you can use the `-inventory` action:

```
/co lookup action:-inventory ...
```

This will *only* return results for inventory item removal (loss) events, and
item insertion events will be ignored.

