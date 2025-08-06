# Count flag

The `#count` flag lets you see how many rows a lookup returned.

It allows you to see exactly how many events occured that match the filter
parameters.

## Example: counting the number of container logs

Let's say you want to find out how many logs there are of player `Minecraft123`
taking out diamonds from nearby containers. Here's how you would do that:

```
/co lookup radius:5 user:Minecraft123 action:-container include:diamond #count
```

> The `#count` tells CoreProtect to tell us how many logs it found that matched
  our query filter.

