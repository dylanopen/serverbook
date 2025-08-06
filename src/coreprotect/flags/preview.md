# Preview flag

The `#preview` flag lets you see what the result of a rollback or restore would
be, without actually applying it.

It's incredibly useful for if you're not sure which command to use and so you
don't want to fully apply a rollback/restore.

## Example: rolling back griefing

If you want to roll back griefing on user Minecraft123's house but *aren't sure
exactly which command to use*, you can test out the results of a rollback like
this:

```
/co rollback radius:30 exclude:Minecraft123 time:7d #preview
```

That way, you can check the rollback will actually do what you want it to do,
so you won't accidentally break something that can't fully be reverted using
[/co undo](../undo.md).

## Example: restoring an incorrect rollback

Let's say you didn't learn your lesson above and rolled back the house without
previewing first. You accidentally deleted the house above because you forgot
the `exclude:Minecraft123`. You'd restore it like this:

```
/co restore radius:30 time:7d user:Minecraft123
```

... in order to restore any actions done by Minecraft123.

But you could make sure that this would restore the house by adding the
`#preview` flag:

```
/co restore radius:30 time:7d user:Minecraft123 #preview
```

## A note about rollbacks

If you add the `#preview` flag, coreprotect won't actually roll anything back.  
You'll need to rerun the rollback command without the `#preview` if you want
to complete a rollback.

