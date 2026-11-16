# Cannot access a shared mailbox

runbook_id: shared-mailbox-access
category: email

## Symptoms
The user can send and receive email from their own mailbox, but a shared mailbox, such as a team inbox, is missing from their mail app or shows "access denied". Only the shared mailbox is affected.

## First checks
1. Check service status (get_service_status: email).
2. Confirm the shared mailbox name and whether the user has had access before.
3. Check in the admin console whether the user has permission on the mailbox.

## Fix
1. If permission is missing, get the mailbox owner's approval, then grant full access in the admin console.
2. Ask the user to restart the mail app; a new mailbox can take 60 minutes to appear.
3. If it still does not appear, add it manually in the mail app settings.
4. Test by opening the shared mailbox in webmail.

## Escalate when
- Email status shows down: escalate to messaging as P1. If status shows degraded: escalate to messaging as P2.
- One team cannot open their shared mailbox: escalate to messaging as P2.
- One person still without access after all fix steps: assign to the messaging queue as P4.
