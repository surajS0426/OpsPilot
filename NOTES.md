# OpsPilot build notes

## Decisions
-16/11/26: Defined impact levels precisely. Without this, the same ticket coule be labelled P1 or P2 which would make the evals unreliable
-16/11/26: Added a security override to the priority rules. The impact x urgency matrix measures current disruption, but a compromised account is a risk that can spread, so suspected compromise is at least P2 regardless of users affected. Claude code flagged the gap when generating runbooks; I decided the rule. 
-16/11/26: Added environement definitions which allows all runbooks to refer to the same, defined tools. 

## AI output I corrected
-16/11/26: runbooks (Claude Code draft of vpn-drops): Reviewed the first draft before approving the rest. Issues found: 
    -Used an ad hoc "more than 5 users" threshold that conflicted with the priority matrix. 
    -Checked VPN service status but never said what to do if it was degraded
    -Sent a P4 single-user issue to on-call; changed to the normal team queue
    Fed these back as rules before generating  the remaining 14 runbooks, so the fix applied to all of them not just 1. 

-16/11/26: runbook app-crash-on-launch: Claude code initially wrote a fix as update to version 8.3 or later. 8.3 is compeltely arbitrary and does not pertain to all applications
    -Removed all invented version numbers from any runbook that is not about a specific tool. 

-16/11/26: runbook new-starter-access: Claude Code treated finance-system access only as a priority question and missed that the real difference is control, not urgency.
    -Kept finance on the matrix: one blocked new starter = P3, the whole finance team blocked at month-end = P2. A fixed "finance is always P2" rule would rush routine requests just because of the system.
    -Added the missing control: finance access needs system-owner approval before it is granted (separation of duties, a standard fraud control). Added to the runbook and to CLAUDE.md.

## Experiments