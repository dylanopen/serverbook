# Container action

Container actions are called whenever items enter or exit a container. This
could be because a player transferred the items, or a hopper transferred them
to another container.

## Syntax

You can use the container action query in one of these two ways:

```
action:container
a:container
```

## Example lookup

```
/co lookup action:container ...
```

## Example: checking 5 block radius, last 7 days

```
/co lookup action:container radius:5 time:7d
```

## Container item insert action

To overspecify the action type to only return results for when items were
*added* to a container, you can use the `+container` action:

```
/co lookup action:+container ...
```

This will *only* return results for item insert events, and item remove events
will be ignored.

## Container item remove action

To overspecify the action type to only return results for when items were
*removed* from a container, you can use the `-container` action:

```
/co lookup action:-container ...
```

This will *only* return results for item remove events, and item insert events
will be ignored.

