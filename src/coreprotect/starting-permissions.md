# Good starting permissions

## Default permissions

The `default` group doesn't need any CoreProtect permissions.

If you trust your players, you *could* give players these permissions so they
can lookup griefing and stealing themselves (but not do any rollbacks):

- coreprotect.inspect
- coreprotect.lookup
- coreprotect.help

This is rare, though. Usually restricting access to only moderators is a good 
idea.

## Moderator permissions

- coreprotect.inspect
- coreprotect.lookup
- coreprotect.rollback
- coreprotect.restore
- coreprotect.teleport
- coreprotect.help

## Admin permissions

- coreprotect.reload
- coreprotect.status
- *coreprotect.purge* -- if you completely trust your admins

