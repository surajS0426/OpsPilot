# Lost or replaced MFA device

runbook_id: mfa-device-lost
category: access

## Symptoms
The user cannot complete multi-factor authentication (MFA), the second sign-in step approved on their phone, because the phone was lost, stolen, replaced or reset. Their password is correct, but no approval request or code arrives.

## First checks
1. Verify the user's identity using the approved method, ideally confirmed by their line manager.
2. Ask whether the old phone was lost or stolen, or simply replaced.
3. Check in the admin console which MFA methods are registered.

## Fix
1. Remove the old MFA device from the user's account in the admin console.
2. Issue a temporary access code valid for one hour.
3. Guide the user to sign in with the code and register the authenticator app, version 6.0 or later, on the new phone.
4. Test sign-in with the new device.

## Escalate when
- The phone was lost or stolen: assign to the security queue as P3 so active sessions can be reviewed.
- Identity cannot be verified: do not reset; assign to the identity queue as P3.
- Several users in one team cannot complete MFA: escalate to identity as P2.
