# Time parameter

The `time` parameter allows us to filter for only events that happened less than
a certain time ago, e.g. are more recent than 2 days ago.

> This parameter is often required.

## Syntax

You can specify the time parameter in one of two ways:

```
time:TIME
t:TIME
```

## Time format

The time is specified using units, for example, `3d` for *3 days*. A full list
of the units coreprotect understands is shown below:

- `s` - seconds
- `m` - minutes
- `h` - hours
- `d` - days
- `w` - weeks

## Combining units

You can combine different units together. For example, to filter for events that
happened less than 1 hour and 20 minutes ago:

```
time:1h20m
```

## Decimals

You can use decimals in your time values. For example, to filter for events
within 2 and a half days:

```
time:2.5d
```

## Time ranges

If you want to get events that occured *more recently than one time frame* but
*longer ago than another time frame*, you can use a time range.

For example, to check for events that happened between 2-3 hours ago:

```
time:2h-3h
```

