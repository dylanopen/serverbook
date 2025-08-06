# Item action

Item actions are called whenever any item is dropped or picked up by a player.

## Syntax

You can use the item action query in one of these two ways:

```
action:item
a:item
```

## Example lookup

```
/co lookup action:item ...
```

## Item remove (pickup) action

To overspecify the action type to only return results for item *pickup* events,
you can use the `+item` action:

```
/co lookup action:+item...
```

This will *only* return results for item pickup events, and item drop events
will be ignored.

## Item remove (drop) action

To overspecify the action type to only return results for item *drop* events,
you can use the `-item` action:

```
/co lookup action:-item...
```

This will *only* return results for item drop events, and item pickup events
will be ignored.

