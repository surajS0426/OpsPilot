# OpsPilot build notes

## Decisions
-16/11/26: Defined impact levels precisely. Without this, the same ticket coule be labelled P1 or P2 which would make the evals unreliable

## AI output I corrected
-16/11/26: runbooks (Claude Code draft of vpn-drops): Reviewed the first draft before approving the rest. Issues found: 
    -Used an ad hoc "more than 5 users" threshold that conflicted with the priority matrix. 
    -Checked VPN service status but never said what to do if it was degraded
    -Sent a P4 single-user issue to on-call; changed to the normal team queue
    Fed these back as rules before generating  the remaining 14 runbooks, so the fix applied to all of them not just 1. 
## Experiments