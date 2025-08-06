# Verbose flag

The `#verbose` flag simply tells CoreProtect to give us extra information while
the rollback or restore is running.

This means it tells you exactly what it's doing at each tick.

## Syntax

Add the flag to the end of your command like any other flag:

```
/co rollback <query> #verbose
/co restore <query> #verbose
```

