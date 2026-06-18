# Rémi's Private Validator Onboarding Checklist

This file is Rémi's private working checklist. All content intended to be sent to the team, existing validators, or candidates is in [Shared.md](Shared.md).

## 0. Do first: prepare the application launch

Complete these tasks in order before applications open:

- [ ] Ask Antoine and LOurs to confirm which current validators, if any, keep `Testnet Validator` without repeating onboarding. Use the internal role-decision message in `Shared.md`.
- [ ] Record the current members and roles before making changes.
- [ ] Confirm that `Testnet Validator Candidate` can see `#testnet-onboarding` but cannot see validator-only channels.
- [ ] Confirm that Rémi and LOurs can assign and remove both validator roles.
- [ ] Get the shared onboarding process and acceptance criteria approved.
- [ ] Post and pin the two candidate onboarding messages from `Shared.md`.
- [ ] Post the announcement for existing validators before changing roles.
- [ ] Give affected members a clear effective time for the role change.
- [ ] Remove `Testnet Validator` from affected members at the announced time.
- [ ] Assign `Testnet Validator Candidate` only to members who explicitly ask to apply again.
- [ ] Verify that members who request the Candidate role can access `#testnet-onboarding`.
- [ ] Publish the application announcement only after the Discord flow has been tested end to end.

Do not remove an existing role before the explanation and onboarding instructions are visible. Do not apply role changes until the exception list is explicitly approved.

## Full task order

- [ ] 1. Align with LOurs on ownership and timing.
- [ ] 2. Verify Discord permissions and candidate channel visibility.
- [ ] 3. Test Antoine's Test13 README from a clean environment.
- [ ] 4. Send structured README feedback to Antoine.
- [ ] 5. Agree on the onboarding process and acceptance criteria with LOurs.
- [ ] 6. Share the onboarding proposal for team review.
- [ ] 7. Audit existing holders of `Testnet Validator`.
- [ ] 8. Agree on which existing validators remain accepted.
- [ ] 9. Publish and pin the approved onboarding messages.
- [ ] 10. Start processing candidates and recording decisions.

## 1. Align with LOurs

- [ ] Send the message to LOurs from `Shared.md`.
- [ ] Agree on who leads each part.
- [ ] Agree where candidate decisions will be recorded.
- [ ] Set a deadline for the first reviewable draft.
- [ ] Agree that both reviewers validate a candidate before assigning `Testnet Validator`.

## 2. Verify Discord permissions

Test without changing access for real validators unless the change has already been approved:

- [ ] Rémi can assign and remove `Testnet Validator Candidate`.
- [ ] Rémi can assign and remove `Testnet Validator`.
- [ ] LOurs has the same permissions.
- [ ] Candidates can see `#testnet-onboarding`.
- [ ] Candidates cannot see validator-only channels.
- [ ] Accepted validators can see all required Testnet Validator channels.
- [ ] Rémi and LOurs can write, pin messages, and moderate the section.
- [ ] Send the appropriate Ryan message from `Shared.md`.

## 3. Test Antoine's README

Run the documented process exactly as written. Do not silently fix commands: record the problem first, then test the correction separately.

### Test checklist

- [ ] Start from a clean machine, VM, container, or empty data directory.
- [ ] Record the operating system, architecture, and software versions.
- [ ] Follow only the prerequisites listed in the README.
- [ ] Download and verify the genesis file.
- [ ] Start the Gnoland node.
- [ ] Confirm that it discovers peers and synchronizes.
- [ ] Restart the node and confirm that it resumes correctly.
- [ ] Create or use the required account safely.
- [ ] Complete the required transaction.
- [ ] Register through the Valopers realm.
- [ ] Confirm that every command, expected output, and link is accurate.
- [ ] Record the total setup time and any blocking issue.
- [ ] Send the README feedback message from `Shared.md`.

Never include seed phrases, private keys, validator signing keys, passwords, or other secrets in notes, feedback, or screenshots.

### Private issue template

```text
Step/section:
Environment:
Command used:
Expected result:
Actual result:
Error output:
Suggested correction:
Severity: blocking / confusing / minor
```

## 4. Finalize the onboarding process

- [ ] Review the shared flow in `Shared.md` with LOurs.
- [ ] Confirm that the Valopers realm remains the single source of truth for challenge instructions.
- [ ] Confirm the RPC availability requirement.
- [ ] Confirm the acceptance and retry criteria.
- [ ] Send the team review request from `Shared.md`.
- [ ] Apply approved feedback to the shared process and Discord messages.

## 5. Publish candidate messages

- [ ] Post pinned message 1, then pinned message 2, from `Shared.md`.
- [ ] Pin both messages in `#testnet-onboarding`.
- [ ] Test every link from Discord.
- [ ] Confirm that the realm instructions and Discord summary do not conflict.
- [ ] Use the candidate response templates from `Shared.md` during reviews.

## 6. Track candidate decisions

- [ ] Create the shared tracker using the template in `Shared.md`.
- [ ] Do not store secrets or unnecessary personal information.
- [ ] Record the published criteria evaluated for every `Needs retry` or `Approved` result.
- [ ] Get agreement from LOurs before assigning `Testnet Validator`.
- [ ] Escalate reviewer disagreements to Antoine.

## 7. Audit existing validators

- [ ] Export or manually record current holders of `Testnet Validator`.
- [ ] Identify core-team validators and external validators.
- [ ] Confirm the treatment of Berty, Samourai, and OnBloc with Antoine and LOurs.
- [ ] Decide whether each remaining external validator keeps the role or has it removed.
- [ ] Send the audit-decision message from `Shared.md` and wait for confirmation.
- [ ] Notify affected people using the shared announcement before changing roles.
- [ ] Apply the approved role changes at the announced time.
- [ ] Assign the Candidate role only to people who request it.
- [ ] Confirm that requested Candidate access works correctly.

## 8. GovDAO handoff

- [ ] Confirm that the candidate passed all published criteria.
- [ ] Confirm the Valoper registration link and review record.
- [ ] Send the GovDAO handoff message from `Shared.md` to Antoine.
- [ ] Record the GovDAO status in the candidate tracker.

## Definition of done

- [ ] The README has been tested end to end and feedback has been addressed.
- [ ] Discord permissions and channel visibility have been verified.
- [ ] The onboarding process and acceptance criteria are approved.
- [ ] Both candidate onboarding messages are published and pinned.
- [ ] The existing-validator audit and role changes are complete.
- [ ] A shared candidate tracker is in use.
- [ ] At least one candidate has passed through the full process, including GovDAO handoff.

The voting-power progression process (`1 → 3 → 6`) is a later task and is not required to launch onboarding.
