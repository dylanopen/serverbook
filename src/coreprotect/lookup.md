# CoreProtect lookup

Lookups are a way of listing the actions that match the query, but not actually
doing anything about it. In other words, just *looking up* what happened.

## Command usage

```
/co lookup <query>
```

## Example: action, radius and time

For  a simple example, to lookup results matching the `block` action within a
`5` block radius in the last `1 hour`, use:

```
/co lookup action:block radius:5 time:1h
```

## Example: item type, global radius, time and excluding a user

This example will return all logs created in the last `1 day` which include an
`elytra` item and **were not** carried out by user `Minecraft123`.

```
/co lookup radius:#global include:elytra exclude:Minecraft123 time:1d
```

## Query parameters

There are lots of different parameters you can use to narrow down your search.  
You can find a full list on the [query parameters](./query-parameters.md) page.

