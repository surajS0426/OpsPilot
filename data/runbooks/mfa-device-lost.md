# Lost or replaced MFA device

runbook_id: mfa-device-lost
category: access

## Symptoms
The user cannot complete multi-factor authentication (MFA), the second sign-in step approved on their phone, because the phone was lost, stolen, replaced or reset. Their password works, but no code arrives.

## First checks
1. Verify the user's identity using the approved method, ideally via their line manager.
2. Ask whether the old phone was lost or stolen, or simply replaced.
3. Check in the identity admin console which MFA methods are registered.

## Fix
1. Remove the old MFA device in the identity admin console.
2. Issue a temporary access code valid for one hour.
3. Guide the user to sign in with the code and register the authenticator app on the new phone; if they cannot, re-register it in the identity admin console.
4. Test sign-in with the new device.

## Escalate when
- The phone was stolen, or the user got MFA prompts they did not trigger: suspected account compromise; escalate to security as P2.
- Identity cannot be verified: do not reset; assign to the identity queue as P3.
- Several users in one team cannot complete MFA: escalate to identity as P2.
