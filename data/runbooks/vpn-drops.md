# VPN disconnects repeatedly

runbook_id: vpn-drops
category: network

## Symptoms
The user is working remotely and their VPN connection keeps dropping every few minutes, so internal systems and file shares stop responding until they reconnect. Their home internet still works and public websites load normally; only the VPN is unstable.

## First checks
1. Check service status (get_service_status: vpn).
2. Ask whether other remote colleagues see the same drops, and how many.
3. Confirm the user's internet is stable with the VPN switched off.
4. Check the VPN client is version 4.2 or later.

## Fix
1. Ask the user to fully quit the VPN client and reconnect.
2. If on Wi-Fi, move closer to the router or use a network cable.
3. Update the VPN client from the self-service portal.
4. Restart the laptop and test the connection for ten minutes.

## Escalate when
- VPN status shows down, or many users cannot connect: escalate to network-oncall as P1. If status shows degraded: escalate to network-oncall as P2.
- One team cannot work because of VPN drops: escalate to network-oncall as P2.
- One person still dropping after all fix steps: assign to the desktop-support queue as P4.
