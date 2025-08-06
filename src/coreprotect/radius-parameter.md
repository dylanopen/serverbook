# Radius parameter

The `radius` filter allows us to get only the events within a certain radius of
the player, or another radius type.

## Syntax

You can query for results only within a certain radius using one of the
following:

```
radius:RADIUS
r:RADIUS
```

## Types of radius

- `numerical radius`: up to how many blocks away to check?
- `#world`: search the entire overworld dimension
- `#world_nether`: search the entire nether dimension
- `#world_the_end`: search the entire end dimension
- `#worldedit` or `#we`: search only within your worldedit selection

## Example: lookup within 5 blocks of you

```
/co lookup radius:5
```

## Example: lookup in overworld dimension

```
/co lookup radius:#world
```

## Example: lookup in nether dimension

```
/co lookup radius:#world_nether
```

## Example: lookup in end dimension

```
/co lookup radius:#world_the_end
```

## Example: lookup within worldedit region

> Note: to use the `#worldedit` radius, you need to have first selected a region
  using the worldedit wand (wooden axe). You can get it by running `//wand`.
  Select the region by left clicking and then right clicking on each corner of
  the selection.  
  See the [WorldEdit chapter](../worldedit.md) for more help using WorldEdit.

```
/co lookup radius:#worldedit
```

