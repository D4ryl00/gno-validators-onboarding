# Shared Validator Onboarding Material

Material to share with team members, validators, and candidates. Replace every
bracketed placeholder before sending.

## Onboarding process

### Flow

1. In `┋💬ㆍgeneral-chat`, someone runs `/candidate-testnet`.
2. The bot assigns `Testnet Validator Candidate` and grants access to
   `#testnet-onboarding`.
3. They read the pinned instructions and follow the Valopers realm requirements.
4. In `#testnet-onboarding`, they run `/submit-request` and provide only their
   operator address.
5. The team reviews against the published criteria.
6. Result: `Approved` or `Needs retry`, with specific feedback.
7. Approved candidates get `Testnet Validator`.
8. GovDAO approves the Valopers registration.
9. The validator joins the active set with voting power `1`.

### Requirements

The Valopers realm is the single source of truth:
https://test13.testnets.gno.land/r/gnops/valopers

Candidates must:

- Set up a node per the Test13 guide:
  https://github.com/gnolang/gno/blob/chain/test13/misc/deployments/test13.gno.land/VALIDATOR.md
- Complete every application step the Valopers realm currently requires.
- In `#testnet-onboarding`, run `/submit-request` and provide only the operator
  address.
- Join a short call only if the submitted address leaves open questions.

Requirements change in the realm, not in Discord. Node setup stays in the guide.

### Acceptance criteria

#### Approve

All criteria met:

- [ ] Followed the published setup successfully.
- [ ] Submitted the operator address with `/submit-request`.
- [ ] The submitted address identifies a validator connected to test13 and synced.
- [ ] Required transaction is valid and publicly verifiable.
- [ ] Valoper registration is complete and accurate.
- [ ] Shows basic grasp of keys, backups, monitoring, upgrades, and incident
      response.
- [ ] Communicates clearly enough to coordinate operations.
- [ ] Never exposed a secret or mishandled a key.

#### Needs retry

Any criterion unmet. In the feedback, name the failed criterion and the next
action. Base every decision on the published criteria alone, never on reputation
or undocumented rules.

Example feedback: `The validator at the submitted address is not synced to the
current test13 height. Fix the node, then run /submit-request again with the
operator address.`

## Existing-validator messages

### Announcement before changing roles

> **Update to the Testnet Validator onboarding process**
>
> We are introducing one onboarding process for all external Testnet validators
> before we open new applications. The requirements are the pinned instructions
> in `#testnet-onboarding` and the Valopers realm.
>
> Thank you to everyone who has validated on the testnet so far. On
> June 22, 2026, we will remove the `Testnet Validator` Discord
> role. We remove it so every external validator is
> onboarded through the same documented criteria, with one clear and fair path
> into the validator set. This is an administrative reset, not a ban or a judgment
> on your past work. To get the role back, re-apply through the steps below.
>
> 1. In `┋💬ㆍgeneral-chat`, run `/candidate-testnet`.
> 2. The bot assigns `Testnet Validator Candidate` and grants access to
>    `#testnet-onboarding`.
> 3. Read the pinned instructions and complete the steps.
> 4. In `#testnet-onboarding`, run `/submit-request` and provide only your
>    operator address.
> 5. The Gno team reviews and either assigns `Testnet Validator` or tells you what
>    remains.
>
> If the bot command or channel access does not work, ask the Gno team in
> `┋💬ㆍgeneral-chat`.

### Short notification after removing a role

> Hi `[NAME]`, thanks for validating on the testnet so far. Your
> `Testnet Validator` role was removed as part of the onboarding reset announced
> here: `[ANNOUNCEMENT LINK]`.
>
> To apply for the new set, run `/candidate-testnet`
> in `┋💬ㆍgeneral-chat`. The bot will assign the Candidate role and grant access
> to `#testnet-onboarding`, where `/submit-request` accepts only your operator
> address.

## Candidate-facing Discord messages

### Bot reply after `/candidate-testnet`

> Welcome! The `Testnet Validator Candidate` role has been assigned.
>
> You now have access to `#testnet-onboarding`. Read the pinned instructions and
> complete the challenge. Once the node and application are ready, run
> `/submit-request` in `#testnet-onboarding` and provide only the operator
> address.

### Pinned message 1 of 3: Technical challenge

> **Testnet Validator Onboarding: test13 (1/3)**
>
> Anyone can apply to be a test13 validator candidate.
>
> **1. Set up your test13 node**
>
> Follow the Test13 guide:
> https://github.com/gnolang/gno/blob/chain/test13/misc/deployments/test13.gno.land/VALIDATOR.md
>
> **2. Complete your validator application**
>
> Follow the current Valopers realm requirements:
> https://test13.testnets.gno.land/r/gnops/valopers
>
> For additional guidance on steps 1 and 2, see:
> https://gnops.io/
>
> **3. Submit your evidence with the Discord bot**
>
> Once the node and application are ready, run `/submit-request` in
> `#testnet-onboarding`. Provide only your operator address. The Gno team uses
> that address to review the validator and its Valoper application.

### Pinned message 2 of 3: Review

> **Testnet Validator Onboarding: test13 (2/3)**
>
> **Review**
>
> Once `/submit-request` is complete, the Gno team uses the submitted operator
> address to review:
>
> - Connection to test13 and synchronization
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

### Acknowledge a submission

> Thanks, we received the operator address submitted with `/submit-request`.
> The Gno team will review it against the published criteria and reply.

### Request missing information

> Thanks. Before we can finish the review, please correct:
>
> - `[MISSING OR INVALID ITEM]`
> - `[MISSING OR INVALID ITEM]`
>
> After fixing it, run `/submit-request` again and provide only the operator
> address.

### Approve a candidate

> Congratulations, you passed the onboarding challenge. We assigned you the
> `Testnet Validator` role.
>
> Next: wait for GovDAO approval and confirmation before treating your validator
> as active. New external validators start with voting power `1` and may earn more
> later through a separate, documented process.

### Decline a candidate and explain how to reapply

> Thanks for completing the challenge. We cannot approve this application because
> the following published criteria are not met:
>
> - `[CRITERION]: [OBSERVED ISSUE]`
> - `[CRITERION]: [OBSERVED ISSUE]`
>
> The `Testnet Validator Candidate` role will now be removed.
>
> To apply again, restart the process from the beginning: run
> `/candidate-testnet` in `┋💬ㆍgeneral-chat`, complete every pinned onboarding
> step, then run `/submit-request` with only the operator address. The new
> application will be reviewed independently.

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
