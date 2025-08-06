# Worldborder command

The `chunky worldborder` command tells Chunky to pregenerate every chunk within
the world border. The world is set using the [`chunky world`](./world.md)
command.

## What does it do?

Under the hood, the `chunky worldborder` command does two things:

- Sets the centre to `0,0` (you can manually set the centre with the [chunky
  center](./center.md) command).
- Sets the radius to the same radius as the worldborder.

## Command usage

```
/chunky worldborder
```

The command doesn't take any arguments.

## Changing the vanilla world border

To set the diameter of the vanilla world border, you use the `/worldborder`
command:

```
/worldborder set <diameter>
```

For example, for a world border of diameter `20,000`, use:

```
/worldborder set 20000
```

