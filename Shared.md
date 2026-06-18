# Shared Validator Onboarding Material

This document contains material intended to be shared with team members, existing validators, or candidates. Replace bracketed placeholders before sending a message.

## Shared onboarding process

### Flow

1. A person asks to join in the general Discord channel.
2. A team member assigns `Testnet Validator Candidate`.
3. The candidate reads the pinned instructions in `#testnet-onboarding`.
4. The candidate follows the current instructions in the Valopers realm and submits the requested evidence.
5. The team reviews the evidence using the published criteria.
6. The result is `Approved` or `Needs retry`, with specific feedback.
7. An approved candidate receives `Testnet Validator`.
8. The existing Valopers registration is approved through GovDAO.
9. The validator enters the active set with voting power `1`.

### Challenge requirements

The Valopers realm is the single source of truth for challenge instructions:

https://gnoweb.test-13.gnoland.network/r/gnops/valopers

Candidates must:

- Complete the node setup, profile, introduction, and any other steps currently required in the realm.
- Share the public Valoper profile link in `#testnet-onboarding`.
- Join a short technical call only when written evidence leaves material questions.

If challenge instructions change, update the realm rather than copying detailed instructions into Discord.

### Acceptance criteria

A candidate is approved when all mandatory criteria are met:

- [ ] Followed the published setup procedure successfully.
- [ ] Submitted the required evidence that the node is running and synchronized on test13.
- [ ] Required transaction is valid and publicly verifiable.
- [ ] Valoper registration is complete and accurate.
- [ ] Demonstrated basic understanding of keys, backups, monitoring, upgrades, and incident response.
- [ ] Communicated clearly enough for operational coordination.
- [ ] Did not expose secrets or demonstrate unsafe key handling.

A candidate receives `Needs retry` when evidence is missing, a task is incomplete, or a safety or operational issue must be corrected. Feedback must identify the failed criterion and required next action. Decisions should not rely on reputation or undocumented criteria.

## Existing-validator messages

### Announcement before changing roles

> **Update to the Testnet Validator onboarding process**
>
> We are introducing a consistent onboarding process for all external Testnet validators before opening new applications.
>
> As part of this change, the `Testnet Validator` role will be removed from some current members on `[DATE AND TIME WITH TIME ZONE]`. This is an administrative reset, not a ban or a negative judgment about anyone's previous contribution.
>
> The goal is to apply the same documented technical and operational criteria to external validators and make the path into the validator set clear to everyone.
>
> If your role is removed and you want to apply for the new validator set:
>
> 1. Ask for the `Testnet Validator Candidate` role in `[GENERAL CHANNEL]`.
> 2. Once the role is assigned, read the pinned instructions in `#testnet-onboarding`: `[MESSAGE OR CHANNEL LINK]`.
> 3. Complete the requested steps, or send evidence of equivalent work you have already completed.
> 4. A member of the Gno team will review the evidence and either assign the `Testnet Validator` role or explain what remains to be completed.
>
> Please do not share seed phrases, private keys, validator signing keys, passwords, or other secrets as evidence.
>
> If you request the Candidate role but cannot access `#testnet-onboarding`, ask a member of the Gno team for help in `[GENERAL CHANNEL]`.

### Short notification after removing a role

> Hi `[NAME]`, your previous `Testnet Validator` role has now been removed as part of the onboarding-process reset announced here: `[ANNOUNCEMENT LINK]`.
>
> If you want to apply for the new validator set, please ask for the `Testnet Validator Candidate` role in `[GENERAL CHANNEL]`. Once assigned, you will receive access to `#testnet-onboarding`. If you already completed equivalent technical steps, you may submit the existing public evidence instead of repeating unnecessary work.

## Candidate-facing Discord messages

### Reply to someone asking to become a validator

> Welcome! Anyone can apply to become a Testnet validator candidate.
>
> I have assigned you the `Testnet Validator Candidate` role. Please go to `#testnet-onboarding`, read the pinned instructions, and complete the onboarding challenge. Once you submit the requested evidence, a member of the Gno team will review it and send you the next steps.

### Pinned message 1 of 2 — Technical challenge

> **Testnet Validator Onboarding — test13 (1/2)**
>
> Anyone may apply to become a test13 validator candidate.
>
> **1 — Follow the official onboarding instructions**
>
> The Valopers realm is the single source of truth for the technical challenge and application requirements:
>
> https://gnoweb.test-13.gnoland.network/r/gnops/valopers
>
> Follow the latest instructions published there. If Discord text differs from the realm, follow the realm.
>
> **2 — Submit your evidence in this channel**
>
> Once you have completed the realm instructions, post the following in `#testnet-onboarding`:
>
> - Your moniker and validator address
> - The public link to your Valoper profile
> - A short introduction covering who you are, your validator experience, and why you want to join test13

### Pinned message 2 of 2 — Review and safety

> **Testnet Validator Onboarding — test13 (2/2)**
>
> **Review**
>
> Once all challenge steps are complete, a member of the Gno team will review:
>
> - Evidence that the node is connected to test13 and synchronized
> - Validator profile completeness and accuracy
> - Basic validator-operations knowledge
> - Participation and communication during onboarding
>
> Additional questions may be asked when clarification is needed. If information is missing or incorrect, you will normally be told what to fix and may submit updated evidence.
>
> Applications may be declined for false or misleading information, unsafe operational practices, abusive behavior, or an inability to demonstrate the basic knowledge required to operate a validator.
>
> If approved, you will receive the `Testnet Validator` Discord role. Entry into the active validator set remains subject to GovDAO approval and available capacity. New external validators start with voting power `1`.
>
> **Security**
>
> Never post a seed phrase, private key, validator signing key, password, private IP address, or other secret. Validator addresses, validator public keys, and public Valoper links are safe to share. If you are unsure whether something is safe, ask before posting it.

### Acknowledge a submission

> Thanks, we received your validator onboarding submission. A member of the Gno team will review it against the published criteria and reply by `[DATE OR TIMEFRAME]`. Please do not send any private key or seed phrase during the review.

### Request missing information

> Thanks for the submission. Before we can complete the review, please provide or correct the following:
>
> - `[MISSING OR INVALID ITEM]`
> - `[MISSING OR INVALID ITEM]`
>
> Please reply with the updated public evidence. Do not share private keys, seed phrases, or validator signing keys.

### Approve a candidate

> Your onboarding challenge has been approved. We have assigned you the `Testnet Validator` role.
>
> Next steps:
>
> 1. Wait for GovDAO approval and confirmation before considering your validator active.
>
> New external validators start with voting power `1` and may receive more voting power later under a separate, documented process.

### Ask a candidate to retry

> Thanks for completing the onboarding challenge. We cannot approve it yet because the following published criteria are not complete:
>
> - `[CRITERION]: [OBSERVED ISSUE]`
> - `[CRITERION]: [OBSERVED ISSUE]`
>
> To retry, please `[SPECIFIC ACTIONS]` and submit the updated evidence here. You are welcome to ask technical questions if any instruction is unclear.

### Escalate an unclear result to a technical call

> Thanks for the submission. Most of the challenge is complete, but we need to clarify `[TOPIC]` before making a decision. Could you join a short technical call at one of these times: `[OPTIONS]`? The call will focus on `[SCOPE]`.

## Shared candidate tracker

Do not store secrets or unnecessary personal information.

| Candidate | Discord | Status | Challenge submitted | Reviewers | Missing criteria | Decision date | Valoper link | GovDAO status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Example | @example | Challenge in progress | YYYY-MM-DD | Team | Sync evidence | — | — | — |

Allowed statuses:

- `Candidate`
- `Challenge in progress`
- `Needs retry`
- `Approved`
- `GovDAO pending`
- `Added to valset`

For every `Needs retry` or `Approved` result, record which published criteria were evaluated. Two reviewers should agree before assigning the validator role; escalate disagreements to Antoine.
