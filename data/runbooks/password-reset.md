# Password reset request

runbook_id: password-reset
category: access

## Symptoms
The user has forgotten their password, or it has expired and they must set a new one. There is no "account locked" message; they simply do not know a working password.

## First checks
1. Verify the user's identity using the approved method, such as a call-back to their directory number.
2. Confirm the message says the password is wrong or expired, not that the account is locked.
3. Check whether the user has registered for the "Forgot password" option.

## Fix
1. If registered, guide the user through "Forgot password" on the sign-in page.
2. Otherwise, set a temporary password in the identity admin console and tick "must change at next sign-in".
3. The new password must be at least 14 characters.
4. Remind them to update it on their phone.

## Escalate when
- Identity cannot be verified or the request seems suspicious: suspected account compromise; do not reset; escalate to security as P2.
- One person still cannot sign in after all fix steps: assign to the identity queue as P3.
- Several users in one team cannot reset passwords: escalate to identity as P2.
