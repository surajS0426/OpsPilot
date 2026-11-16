# Account locked after failed sign-ins

runbook_id: account-locked
category: access

## Symptoms
The user knows their password but sees a message saying their account is locked after too many failed sign-in attempts. Often an old password saved on a phone keeps retrying after a password change. They cannot sign in anywhere.

## First checks
1. Verify the user's identity using the approved method.
2. In the admin console, confirm the account is locked and note where the failed attempts came from.
3. Ask whether they changed their password recently and which devices use their account.

## Fix
1. Unlock the account in the admin console.
2. Ask the user to update the saved password on their phone, tablet and other devices.
3. Ask the user to sign in once and confirm it works.
4. If it locks again, find which device the failed attempts come from.

## Escalate when
- Failed attempts come from an unknown location or device: do not unlock; assign to the security queue as P3.
- Many users locked out at the same time: escalate to security as P1.
- One person keeps relocking after all fix steps: assign to the identity queue as P3.
