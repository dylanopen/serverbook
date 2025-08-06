# Session action

Session actions are created when a player logs into the server or logs out of
the server.

## Syntax

You can use the session action query in one of these two ways:

```
action:session
a:session
```

## Example lookup

```
/co lookup action:session ...
```

## Log-in action

To overspecify the session action type to only return results for when a user
logged *in* to the server, you can use the `+session` action:

```
/co lookup action:+session ...
```

This will *only* return results for *log-ins*, and *log-outs* will be ignored.

## Log-out action

To overspecify the session action type to only return results for when a user
logged *out* of the server, you can use the `-session` action:

```
/co lookup action:-session ...
```

This will *only* return results for *log-outs*, and *log-ins* will be ignored.

