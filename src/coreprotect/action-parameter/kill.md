# Kill action

Kill actions are called whenever a player or another mob kills an entity.

For example, if a zombie killed a villager, coreprotect would log that as:
- user: \#zombie
- action: kill
- target: \#villager


## Syntax

You can use the kill action query in one of these two ways:

```
action:kill
a:kill
```

## Example lookup

```
/co lookup action:kill ...
```

## Example lookup for villager death

```
/co lookup action:kill include:villager ...
```

## Example: roll back dogs dying

```
/co rollback action:kill include:wolf
```

