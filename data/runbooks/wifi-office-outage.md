# Office Wi-Fi unavailable

runbook_id: wifi-office-outage
category: network

## Symptoms
Users in the office cannot connect to the office Wi-Fi, or connect but nothing loads. It usually affects a floor or the whole site, and the same laptops work normally at home. This is not a VPN problem.

## First checks
1. Check service status (get_service_status: wifi).
2. Find out which floor or area is affected and roughly how many people.
3. Check whether wired desk connections in that area still work.

## Fix
1. Ask users to switch Wi-Fi off and on, then rejoin the office network.
2. If only one laptop fails, restart it and update its Wi-Fi driver to the latest approved version in the software catalogue using the device-management tool.
3. Ask that user to forget the office network and rejoin it.
4. Meanwhile, move users to wired connections.

## Escalate when
- Wi-Fi status shows down, or a whole site cannot connect: escalate to network-oncall as P1. If status shows degraded: escalate to network-oncall as P2.
- One team or area without Wi-Fi: escalate to network-oncall as P2.
- One person cannot connect after all fix steps: assign to the desktop-support queue as P3.
