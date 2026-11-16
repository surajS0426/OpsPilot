# Emails stuck in outbox or not sending

runbook_id: email-not-sending
category: email

## Symptoms
Emails the user sends from their own mailbox stay in the Outbox or bounce back as "not delivered". They can usually still open their mailbox and receive email; only outgoing messages fail. This is not about shared mailboxes.

## First checks
1. Check service status (get_service_status: email).
2. Ask whether colleagues can send email and what any bounce message says.
3. Check the stuck message's size; attachments over 25 MB are rejected.

## Fix
1. Remove large attachments and share a file link instead.
2. Ask the user to close and reopen the mail app, then send again.
3. If the mailbox is full, archive or delete old items.
4. Test sending from webmail; if that works, repair the mail app profile.

## Escalate when
- Email status shows down, or many users cannot send: escalate to messaging as P1. If status shows degraded: escalate to messaging as P2.
- One team cannot send email: escalate to messaging as P2.
- One person still cannot send after all fix steps: assign to the messaging queue as P3.
