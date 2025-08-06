# Good starting permissions

One page you will notice comes up in almost every plugin chapter is the
`Good starting permissions` page.

Every plugin defines *permissions* that determine who can access which commands.
Using a plugin called LuckPerms, we can give different groups of people access
to different commands. See the [LuckPerms chapter](../luckperms.md) for help on
adding permissions to groups, users, etc.

For each plugin you install, if you want to restrict or give access to its
commands, you need to set up the permissions for it. Each chapter has a page
which outlines some good permissions you should give to three groups: `default`,
`moderator` and `admin`.

## Default permissions

Default permissions are those permissions that are given to every player on your
server.

Any permissions under this section should be given to your `default` group. You
should run this command for every `PERMISSION` in the list:

```
/lp group default permission set PERMISSION
```

## Moderator permissions

Moderator permissions are those permissions given to your mods: moderators
usually teleport around the server in spectator, catching cheaters and rolling
back any griefing that occurs.  
They **do not** deal with plugin issues or any other server-side issue; that's
reserved for *admins*.

Any permissions under this section should be given to your `moderator` group.
You should run this command for every `PERMISSION` in the list:

```
/lp group moderator permission set PERMISSION
```

## Admin permissions

Admin permissions are those permissions given to your admins: admins generally
do what mods do, and so your admin group should inherit from your moderator
group.  
Admins do more than that, though: they also deal with configuring plugins,
server configuration and anything else regarding the server itself. So admins
need more permissions than moderators.

Any permissions under this section should be given to your `admin` group.
You should run this command for every `PERMISSION` in the list:

```
/lp group admin permission set PERMISSION
```

