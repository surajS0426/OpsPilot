# Suspected phishing email reported

runbook_id: phishing-reported
category: other

## Symptoms
The user received a suspicious email, such as an unexpected request to sign in, pay an invoice or open an attachment, and is unsure whether it is genuine. They may or may not have clicked a link or entered details.

## First checks
1. Ask whether they clicked a link, opened an attachment or entered a password.
2. Check the sender's address and how many colleagues received the same email.
3. Confirm the user reported it with the "Report phishing" button.

## Fix
1. If nothing was clicked, the user can delete the email.
2. If they entered a password, reset it straight away in the identity admin console.
3. If an attachment was opened, disconnect the laptop from the network.
4. Remind the user not to reply or forward it.

## Escalate when
- Many users entered details or opened the attachment: escalate to security as P1.
- One person entered a password or opened an attachment: suspected account compromise; escalate to security as P2.
- Nobody clicked or entered details: assign to the security queue as P4 for blocking and awareness.
