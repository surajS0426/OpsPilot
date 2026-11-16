# Laptop disk full or low storage warning

runbook_id: disk-full
category: hardware

## Symptoms
The laptop shows a "low disk space" warning, runs slowly, or cannot save files or install updates because its storage is almost full. Everything else, including the network, works normally.

## First checks
1. Open storage settings and note the free space and which folders use the most.
2. Check the size of the Downloads folder and the recycle bin.
3. Confirm the cloud file-sync app is running and is version 3.0 or later.

## Fix
1. Empty the recycle bin and run the built-in disk clean-up.
2. Ask the user to delete or move large files in Downloads they no longer need.
3. Set synced folders to "online only" so files stay in the cloud, not on the disk.
4. Uninstall unused applications through the self-service portal.

## Escalate when
- The user still cannot save work after all fix steps: assign to the desktop-support queue as P3.
- The disk fills again quickly with no clear cause: assign to the desktop-support queue as P4.
- Unknown large files or files with strange extensions appear suddenly: assign to the security queue as P3.
