# VPN disconnects repeatedly

runbook_id: vpn-drops
category: network

## Symptoms
The user is working remotely and their VPN connection keeps dropping every few minutes, cutting them off from internal systems. Their home internet still works and public websites load normally; only the VPN is unstable.

## First checks
1. Check service status (get_service_status: vpn).
2. Ask how many remote colleagues see the same drops.
3. Confirm the user's internet is stable with the VPN switched off.
4. Check the VPN client is version 4.2 or later.

## Fix
1. Fully quit the VPN client and reconnect.
2. If on Wi-Fi, move closer to the router or use a network cable.
3. Ask the user to update the VPN client from the self-service portal; if they cannot, push the update with the device-management tool.
4. Restart the laptop and test the connection for ten minutes.

## Escalate when
- VPN status shows down, or many users cannot connect: escalate to network-oncall as P1. If status shows degraded: escalate to network-oncall as P2.
- One team cannot work: escalate to network-oncall as P2.
- One person still dropping after all fix steps: assign to the desktop-support queue as P4.
