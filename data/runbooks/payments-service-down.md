# Card payments failing

runbook_id: payments-service-down
category: software

## Symptoms
Card payments in a shop or on the website are declined or time out, even for customers with valid cards. Staff may see "payment service unavailable" on the till. Payments are a revenue system, so any failure counts as affecting many users.

## First checks
1. Check service status (get_service_status: payments).
2. Ask whether all tills fail or only one, and since when.
3. Check the till's network connection by opening another internal page.

## Fix
1. If only one till fails, restart the till and its card reader.
2. Reconnect the card reader cable and confirm it shows "ready".
3. Take payments on another till while the faulty one is investigated.
4. If store policy allows, switch to the documented backup payment process.

## Escalate when
- Payments status shows down, or card payments fail across a site or the website: escalate to payments-oncall as P1. If status shows degraded: escalate to payments-oncall as P2.
- One till still failing after all fix steps while others work: escalate to payments-oncall as P2.
