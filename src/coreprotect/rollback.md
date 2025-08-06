# CoreProtect rollback

When running a **rollback** with coreprotect, it essentially runs a
[lookup](./lookup.md) and rolls back each event that lookup returns.

This means that when you run a rollback, you can be sure that it will roll back
everything and only everything that is returned by the same query as a lookup
(assuming you don't move and all query parameters stay the same).

## Command usage

```
/co rollback <query>
```

## Example: action, radius and time

For a simple example, to rollback results matching the `block` action within a
`5` block radius in the last `1 hour`, use:

```
/co rollback action:block radius:5 time:1h
```

## Example: item type, global radius, time and excluding a user

This example will roll back all events in the last `1 day` which include an
`elytra` item and **were not** carried out by user `Minecraft123`.

```
/co rollback radius:#global include:elytra exclude:Minecraft123 time:1d
```

## Query parameters

There are lots of different parameters you can use to narrow down your search.  
You can find a full list on the [query parameters](./query-parameters.md) page.

