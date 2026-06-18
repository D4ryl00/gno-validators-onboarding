# External Validator Onboarding Plan

## 1. Documentation and technical validation

**Owner:** Antoine  
**Reviewers:** Rémi, LOurs  
**Priority:** Immediate

- Write the Test13 validator README covering:
  - Joining Test13
  - Downloading and verifying genesis
  - Running and syncing a node
  - Registering through the Valopers realm
  - Submitting the required transaction/application
- Rémi and LOurs deploy validators by following the README.
- Record unclear, missing, or incorrect instructions.
- Antoine updates the README based on their feedback.
- Publish the validated final version.

## 2. Define the candidate onboarding process

**Owners:** Rémi, LOurs  
**Reviewers:** Antoine, Manfred, Michelle, Ryan  
**Priority:** Immediate

Create a shared draft describing:

- How someone requests to become a validator candidate.
- How moderators assign the `Testnet Validator Candidate` role.
- Instructions shown in `#testnet-onboarding`.
- The technical challenge, potentially including:
  - Running and syncing a Gnoland node
  - Registering as a valoper
  - Providing a public RPC endpoint that remains reachable throughout the review
  - Demonstrating basic operational and troubleshooting knowledge
  - Joining a short voice call if needed
- Objective pass/fail criteria.
- How Rémi and LOurs record and communicate decisions.
- How successful candidates receive the `Testnet Validator` role.
- How unsuccessful candidates receive constructive feedback and may retry.
- How approved candidates are submitted and accepted through Valopers/GovDAO.

The Valopers realm is the single source of truth for challenge instructions: https://gnoweb.test-13.gnoland.network/r/gnops/valopers. Before applications open, Rémi and LOurs must write a concise Discord introduction that links to the realm, lists the evidence to submit in `#testnet-onboarding`, requires a public RPC endpoint for the duration of the review, and explains the review process. After approval, pin it in `#testnet-onboarding`.

## 3. Finalize Discord operations

**Owner:** Ryan  
**Operational owners:** Rémi, LOurs  
**Status:** Mostly complete

Already completed:

- Created `Testnet Validator Candidate`.
- Created the testnet onboarding channel.
- Granted administrative permissions to Antoine, Rémi, and LOurs.

Remaining checks:

- Verify Rémi and LOurs can assign and remove both validator roles.
- Verify they can write to and moderate all Testnet Validator channels.
- Configure channel access so candidates only see the onboarding area, while accepted validators see the full section.
- Pin the onboarding instructions once approved.

## 4. Review existing validator access

**Owners:** Rémi, LOurs, Antoine  
**Priority:** Before the public announcement

- Audit everyone currently holding `Testnet Validator`.
- Confirm whether Berty, Samourai, and OnBloc should retain or receive the role directly.
- Remove `Testnet Validator` from other external validators unless explicitly approved.
- Assign `Testnet Validator Candidate` only when a former validator explicitly asks to apply again.
- Notify affected validators before changing their roles.
- Give migrated validators clear instructions for completing the new process.

## 5. Define acceptance and governance flow

**Owners:** Rémi, LOurs  
**Approver:** Antoine  
**Priority:** Immediate

Document the operational sequence:

1. Candidate requests access.
2. Candidate receives the Discord candidate role.
3. Candidate completes the onboarding challenge.
4. Rémi and LOurs approve or reject the candidate.
5. Approved candidate receives the validator role.
6. Candidate registers through the Valopers realm.
7. Registration is accepted through GovDAO; currently Antoine can execute approval directly.
8. Validator enters the active set with voting power `1`.

The criteria must remain welcoming and transparent while filtering validators based on clear technical and operational requirements.

## 6. Communications and migration

**Owner:** Michelle  
**Dependencies:** README and onboarding process approved

Prepare and publish:

- Discord announcement.
- Telegram migration message for existing validators.
- Application instructions across planned communication channels.
- A clear summary:
  - Anyone may become a validator candidate.
  - Candidates request access in the general channel.
  - Candidates complete an onboarding challenge.
  - Successful candidates are progressively added to the validator set.
- Links to:
  - Discord
  - Test13 README
  - Onboarding channel/process
  - Valoper registration

## 7. Voting-power progression

**Owners:** Rémi, LOurs  
**Priority:** Later

Design a separate process for progressively increasing voting power, for example `1 → 3 → 6`, based on measurable criteria such as:

- Uptime and reliability
- Upgrade responsiveness
- Participation in testnet exercises
- Technical competence
- Community responsiveness
- Security and operational maturity

Core-team validators currently retain voting power `10`.

## Next tasks by person

### Antoine

- Complete the first draft of the Test13 validator README.
- Update the README after Rémi and LOurs test it.
- Review and approve the candidate onboarding process.
- Decide with Rémi and LOurs how to handle existing validators.
- Approve successful valoper applications through GovDAO.

### Rémi

- Deploy a Test13 validator by following the README from start to finish.
- Report documentation gaps and propose improvements.
- Draft the onboarding challenge and its objective acceptance criteria with LOurs.
- Write and pin the candidate-facing introduction and challenge message in `#testnet-onboarding` after approval.
- Define how candidate decisions and retry feedback will be recorded.
- Audit existing validator roles with LOurs and Antoine.
- Verify the required Discord role and channel permissions.

### LOurs

- Deploy a Test13 validator by following the README from start to finish.
- Report documentation gaps and propose improvements.
- Draft the onboarding challenge and its objective acceptance criteria with Rémi.
- Review and approve the candidate-facing introduction and challenge message before it is pinned.
- Define how candidate decisions and retry feedback will be recorded.
- Audit existing validator roles with Rémi and Antoine.
- Verify the required Discord role and channel permissions.

### Michelle

- Review the onboarding process and provide communication feedback.
- Prepare the public Discord and validator-application announcement.
- Prepare the Telegram migration message for existing validators.
- Publish the communications once the README and onboarding process are approved.

### Ryan

- Verify that Rémi and LOurs can assign and remove both validator roles.
- Verify their moderation access across the Testnet Validator channels.
- Configure channel visibility for candidates and accepted validators.
- Help pin the final onboarding instructions in `#testnet-onboarding`.

### Manfred

- Review the proposed onboarding process.
- Confirm that its openness, selection criteria, and messaging align with the agreed validator strategy.

## Immediate next actions

1. Antoine completes the first README draft.
2. Rémi and LOurs test it through full validator deployments.
3. Rémi and LOurs complete the shared onboarding-process draft.
4. Reviewers comment on and approve the process.
5. Rémi, LOurs, and Antoine decide how to handle existing validator roles.
6. Ryan verifies Discord permissions and channel visibility.
7. Pin the approved process in the onboarding channel.
8. Michelle publishes the announcement and migration communications.
