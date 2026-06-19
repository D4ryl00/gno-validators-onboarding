# Shared Validator Onboarding Material

Material to share with team members, validators, and candidates. Replace every
bracketed placeholder before sending.

## Onboarding process

### Flow

1. Someone asks to join in the general Discord channel.
2. A team member assigns `Testnet Validator Candidate`.
3. They read the pinned instructions in `#testnet-onboarding`.
4. They follow the Valopers realm requirements and submit the evidence.
5. The team reviews against the published criteria.
6. Result: `Approved` or `Needs retry`, with specific feedback.
7. Approved candidates get `Testnet Validator`.
8. GovDAO approves the Valopers registration.
9. The validator joins the active set with voting power `1`.

### Requirements

The Valopers realm is the single source of truth:
https://gnoweb.test-13.gnoland.network/r/gnops/valopers

Candidates must:

- Set up a node per the Test13 README:
  https://github.com/gnolang/gno/blob/chain/test13/misc/deployments/test13.gno.land/README.md
- Complete every application step the Valopers realm currently requires.
- Post their public Valoper profile link in `#testnet-onboarding`.
- Join a short call only if written evidence leaves open questions.

Requirements change in the realm, not in Discord. Node setup stays in the README.

### Acceptance criteria

Approve when all are met:

- [ ] Followed the published setup successfully.
- [ ] Submitted evidence the node is connected to test13 and synced.
- [ ] Required transaction is valid and publicly verifiable.
- [ ] Valoper registration is complete and accurate.
- [ ] Shows basic grasp of keys, backups, monitoring, upgrades, and incident
      response.
- [ ] Communicates clearly enough to coordinate operations.
- [ ] Never exposed a secret or mishandled a key.

Otherwise mark `Needs retry`. In the feedback, name the failed criterion and the
next action. Base every decision on the published criteria alone, never on
reputation or undocumented rules.

Example feedback: `Sync evidence missing: node not shown at the current block
height. Post your node's block-height query output, then resubmit.`

## Existing-validator messages

### Announcement before changing roles

> **Update to the Testnet Validator onboarding process**
>
> We are introducing one onboarding process for all external Testnet validators
> before we open new applications. The requirements are the pinned instructions
> in `#testnet-onboarding` and the Valopers realm.
>
> Thank you to everyone who has validated on the testnet so far. On
> `[DATE AND TIME WITH TIME ZONE]` we will remove the `Testnet Validator` Discord
> role from `[WHO IS AFFECTED]`. We remove it so every external validator is
> onboarded through the same documented criteria, with one clear and fair path
> into the validator set. This is an administrative reset, not a ban or a judgment
> on your past work. To get the role back, re-apply through the steps below.
>
> 1. Ask for `Testnet Validator Candidate` in `[GENERAL CHANNEL]`.
> 2. Read the pinned instructions in `#testnet-onboarding`: `[MESSAGE OR CHANNEL LINK]`.
> 3. Complete the steps, or send evidence of equivalent work you already did.
> 4. The Gno team reviews and either assigns `Testnet Validator` or tells you what
>    remains.
>
> Security rules: `[SECURITY PIN]`
>
> Requested the role but cannot see `#testnet-onboarding`? Ask the Gno team in
> `[GENERAL CHANNEL]`.

### Short notification after removing a role

> Hi `[NAME]`, thanks for validating on the testnet so far. Your
> `Testnet Validator` role was removed as part of the onboarding reset announced
> here: `[ANNOUNCEMENT LINK]`.
>
> To apply for the new set, ask for `Testnet Validator Candidate` in
> `[GENERAL CHANNEL]`. You will then get access to `#testnet-onboarding`. If you
> already did equivalent steps, submit the existing public evidence instead of
> redoing them.

## Candidate-facing Discord messages

### Reply to someone asking to become a validator

> Welcome! Anyone can apply to be a Testnet validator candidate.
>
> I assigned you the `Testnet Validator Candidate` role. Go to
> `#testnet-onboarding`, read the pinned instructions, and complete the challenge.
> Once you submit the evidence, the Gno team reviews it and sends your next steps.

### Pinned message 1 of 3: Technical challenge

> **Testnet Validator Onboarding: test13 (1/3)**
>
> Anyone can apply to be a test13 validator candidate.
>
> **1. Set up your test13 node**
>
> Follow the Test13 README:
> https://github.com/gnolang/gno/blob/chain/test13/misc/deployments/test13.gno.land/README.md
>
> **2. Complete your validator application**
>
> Follow the current Valopers realm requirements:
> https://gnoweb.test-13.gnoland.network/r/gnops/valopers
>
> **3. Submit your evidence here**
>
> Once the node and application are done, post in `#testnet-onboarding`:
>
> - Your moniker and validator address
> - The public link to your Valoper profile
> - A short intro: who you are, your validator experience, and why you want to
>   join test13

### Pinned message 2 of 3: Review

> **Testnet Validator Onboarding: test13 (2/3)**
>
> **Review**
>
> Once every step is done, the Gno team reviews:
>
> - Evidence the node is connected to test13 and synced
> - Validator profile completeness and accuracy
> - Basic validator-operations knowledge
> - Participation and communication during onboarding
>
> We may ask follow-up questions. If something is missing or wrong, we tell you
> what to fix and you resubmit.
>
> We decline applications for false or misleading information, unsafe operations,
> abusive behavior, or failure to show the basic knowledge a validator needs.
>
> If approved, you get the `Testnet Validator` Discord role. Joining the active
> set still needs GovDAO approval and free capacity. New external validators start
> with voting power `1`.

### Pinned message 3 of 3: Security

> **Testnet Validator Onboarding: test13 (3/3)**
>
> Never share seed phrases, private keys, validator signing keys, passwords,
> private IP addresses, or other secrets. Validator addresses, validator public
> keys, and public Valoper links are safe to share. Unsure? Ask before posting.

Other messages link here as `[SECURITY PIN]`.

### Acknowledge a submission

> Thanks, we received your validator onboarding submission. The Gno team will
> review it against the published criteria and reply by `[DATE OR TIMEFRAME]`.
> Security rules: `[SECURITY PIN]`

### Request missing information

> Thanks. Before we can finish the review, please provide or correct:
>
> - `[MISSING OR INVALID ITEM]`
> - `[MISSING OR INVALID ITEM]`
>
> Reply with the updated public evidence. Security rules: `[SECURITY PIN]`

### Approve a candidate

> Congratulations, you passed the onboarding challenge. We assigned you the
> `Testnet Validator` role.
>
> Next: wait for GovDAO approval and confirmation before treating your validator
> as active. New external validators start with voting power `1` and may earn more
> later through a separate, documented process.

### Ask a candidate to retry

> Thanks for completing the challenge. We cannot approve it yet because these
> published criteria are not met:
>
> - `[CRITERION]: [OBSERVED ISSUE]`
> - `[CRITERION]: [OBSERVED ISSUE]`
>
> To retry, `[SPECIFIC ACTIONS]` and submit the updated evidence here. Ask if any
> instruction is unclear.

### Escalate an unclear result to a technical call

> Thanks for the submission. Before we decide, we need to clarify `[TOPIC]`. Can
> you join a short technical call at one of these times: `[OPTIONS]`? It will
> focus on `[SCOPE]`.

## Shared candidate tracker

No secrets, no unnecessary personal information.

| Candidate | Discord | Status | Challenge submitted | Reviewers | Missing criteria | Decision date | Valoper link | GovDAO status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Example | @example | Challenge in progress | YYYY-MM-DD | Team | Sync evidence | - | - | - |

Allowed statuses: `Candidate`, `Challenge in progress`, `Needs retry`,
`Approved`, `GovDAO pending`, `Added to valset`.

For every `Needs retry` or `Approved`, record which published criteria were
evaluated. Two reviewers must agree before assigning the role. Escalate
disagreements to Antoine.
