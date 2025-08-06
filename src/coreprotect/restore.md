# CoreProtect restore

Restores are essentially the opposite of [rollbacks](./rollback.md).

Their function is to undo the actions of a rollback. For example, if you
accidentally rolled back somebody's base too far, it may delete parts you
didn't want it to. If `/co undo` won't do the job, you can rerun the same
command you used to roll it back but with `rollback` replaced with `restore`,
and if you stand in the same place, the rollback will be reverted.

## Command usage

```
/co rollback <query>
```

## Example: action, radius and time

For a simple example, we rolled back events matching the `block` action within a
`5` block radius in the last `1 hour`. This was a mistake, so we can restore
(undo the rollback) using:

```
/co restore action:block radius:5 time:1h
```

## Example: item type, global radius, time and excluding a user

In this example, we accidentally rolled back all events in the last `1 day`
which include an `elytra` item and **were not** carried out by user
`Minecraft123`. To undo this, you can run:

```
/co restore radius:#global include:elytra exclude:Minecraft123 time:1d
```

## Query parameters

There are lots of different parameters you can use to narrow down your search.  
You can find a full list on the [query parameters](./query-parameters.md) page.

