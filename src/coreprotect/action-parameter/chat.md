# Chat action

Chat actions are called whenever any message is sent in chat.

This action is generally only triggered by *player* events.

## Syntax

You can use the chat action query in one of these two ways:

```
action:chat
a:chat
```

## Example lookup

```
/co lookup action:chat ...
```

## Rollbacks

> Chat events can't be rolled back or restored, as they were already sent to
  clients.

