# Click action

Click actions are called whenever a player interacts with a block or other part
of the world (through a mouse click).

There are hundreds of different causes of a click action, such as interacting
with a crafting table, opening a chest or opening a door/trapdoor.

## Syntax

You can use the click action query in one of these two ways:

```
action:click
a:click
```

## Uses

I've personally found the `click` action very useful when looking up which
player clicked the trapdoor above another player's ender pearl stasis chamber.

There are probably far more uses than this. You can also see when players
clicked buttons, flipped levers, etc.

## Example lookup

```
/co lookup action:click ...
```

## Example lookup: only oak trapdoors

```
/co lookup action:click include:oak_trapdoor ...
```

