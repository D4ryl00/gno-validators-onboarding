# Rémi's Validator Onboarding Tasks

This document is Rémi's working checklist. Text inside blockquotes is ready to copy and paste into Discord after replacing placeholders such as `[README LINK]`.

## Start here

Yes: complete section 0 first. It is the minimum launch-readiness work required before the blog post opens validator applications. The later numbered sections contain the detailed procedures and reusable messages for the complete onboarding workflow.

## 0. Do first: prepare the application launch

The blog post is expected tomorrow. Complete these tasks in this order before it is published:

- [ ] Get Antoine and LOurs to confirm which current validators, if any, keep `Testnet Validator` without repeating onboarding.
- [ ] Record the current members and roles before making changes.
- [ ] Confirm that `Testnet Validator Candidate` can see `#testnet-onboarding` but cannot see validator-only channels.
- [ ] Confirm that Rémi and LOurs can assign and remove both validator roles.
- [ ] Finalize and pin the candidate introduction and challenge messages.
- [ ] Post the migration announcement for current validators.
- [ ] Give affected members a clear effective time for the role change.
- [ ] Remove `Testnet Validator` from affected members at the announced time.
- [ ] Assign `Testnet Validator Candidate` only to members who explicitly ask to apply again.
- [ ] Verify that members who request the Candidate role can access `#testnet-onboarding`.
- [ ] Publish the application announcement only after the Discord flow has been tested end to end.

Do not remove the existing role before the explanation and onboarding instructions are visible. Do not apply the migration until the exception list has been explicitly approved.

### Reply to Antoine

> Bien reçu. Avant la publication, LOurs et moi allons finaliser et tester le parcours Discord, préparer les messages d'introduction et vérifier les permissions.
>
> Pour les membres qui ont actuellement le rôle `Testnet Validator`, je propose l'ordre suivant :
>
> 1. Valider ensemble la liste des personnes qui conservent directement le rôle.
> 2. Publier un message expliquant le nouveau processus.
> 3. Retirer le rôle `Testnet Validator` aux autres membres à l'heure annoncée.
> 4. Leur demander de manifester leur intérêt s'ils souhaitent candidater à nouveau.
> 5. Attribuer `Testnet Validator Candidate` uniquement à ceux qui en font la demande, puis vérifier leur accès à `#testnet-onboarding`.
>
> Comme ça, personne ne perd son rôle sans explication et chacun dispose d'une prochaine étape claire s'il souhaite candidater. Je prépare les textes aujourd'hui. Il nous faut simplement confirmer la liste des exceptions avant d'appliquer les changements.

### Internal role decision request

> Avant de modifier les rôles Discord existants, il nous faut valider explicitement la liste de migration.
>
> Validations directes proposées : Berty, Samourai, OnBloc `[À CONFIRMER OU MODIFIER]`
>
> Membres dont le rôle `Testnet Validator` sera retiré : `[NOMS]`
>
> Cas particuliers à discuter : `[NOMS ET RAISONS]`
>
> Antoine et LOurs, pouvez-vous confirmer ou modifier cette liste avant `[HEURE]` ? Une fois la liste validée, je publierai le message d'explication puis retirerai les anciens rôles Validator. Le rôle Candidate sera ensuite attribué uniquement aux personnes qui demanderont à candidater.

### Announcement to existing validators before changing roles

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

### Short notification after removing a member's role

> Hi `[NAME]`, your previous `Testnet Validator` role has now been removed as part of the onboarding-process reset announced here: `[ANNOUNCEMENT LINK]`.
>
> If you want to apply for the new validator set, please ask for the `Testnet Validator Candidate` role in `[GENERAL CHANNEL]`. Once assigned, you will receive access to `#testnet-onboarding`. If you already completed equivalent technical steps, you may submit the existing public evidence instead of repeating unnecessary work.

### Final launch check message

> Discord onboarding is ready for the application launch.
>
> - Candidate role and channel access tested: `[YES/NO]`
> - Rémi and LOurs role-management permissions tested: `[YES/NO]`
> - Existing-validator role removal announced and completed: `[YES/NO]`
> - Onboarding introduction pinned: `[LINK]`
> - Challenge and acceptance criteria published: `[LINK]`
> - README tested: `[YES/NO + LINK]`
> - Candidate tracker ready: `[LINK]`
>
> Remaining blockers: `[NONE OR LIST]`

## Full task order

After the urgent launch preparation above, use this checklist to track the complete onboarding work. Some items overlap with section 0 and may already be complete.

- [ ] 1. Align with LOurs on ownership and timing.
- [ ] 2. Verify Discord permissions and candidate channel visibility.
- [ ] 3. Test Antoine's Test13 README from a clean environment.
- [ ] 4. Send structured README feedback to Antoine.
- [ ] 5. Agree on the onboarding challenge and acceptance criteria with LOurs.
- [ ] 6. Share the onboarding proposal for review.
- [ ] 7. Audit existing holders of the `Testnet Validator` role.
- [ ] 8. Agree on which existing validators remain accepted.
- [ ] 9. Publish and pin the approved onboarding instructions.
- [ ] 10. Start processing candidates and recording decisions.

## 1. Align with LOurs

Agree on who will lead each part, where candidate decisions will be recorded, and when the first draft will be ready.

### Message to LOurs

> Salut LOurs, je te propose qu'on se répartisse le travail d'onboarding des validateurs comme ceci :
>
> - On teste tous les deux le README d'Antoine indépendamment, depuis un environnement propre.
> - Je prépare une première version du processus d'onboarding et des messages destinés aux candidats.
> - Tu relis le challenge technique et les critères d'acceptation.
> - On examine ensemble les résultats des candidats avant d'attribuer le rôle `Testnet Validator`.
>
> Il nous faut aussi un tableau partagé pour suivre les candidats. Je propose les statuts suivants : `Candidate`, `Challenge en cours`, `À retenter`, `Approuvé` et `Ajouté au valset`.
>
> Est-ce que cette répartition te convient ? Si oui, je prépare la première version pour relecture.

## 2. Verify Discord permissions

Test the following without changing access for real validators unless the change has already been agreed:

- [ ] Rémi can assign and remove `Testnet Validator Candidate`.
- [ ] Rémi can assign and remove `Testnet Validator`.
- [ ] LOurs has the same permissions.
- [ ] Candidates can see `#testnet-onboarding`.
- [ ] Candidates cannot see validator-only channels.
- [ ] Accepted validators can see all required Testnet Validator channels.
- [ ] Rémi and LOurs can write, pin messages, and moderate the section.

### Message to Ryan if everything works

> Hey Ryan, I tested the validator onboarding permissions. Rémi and LOurs can manage the candidate and validator roles, and the channel visibility works as expected. Thanks.

### Message to Ryan if something is missing

> Hey Ryan, I tested the validator onboarding permissions. The following still needs to be adjusted:
>
> - [MISSING PERMISSION OR CHANNEL ACCESS]
> - [MISSING PERMISSION OR CHANNEL ACCESS]
>
> The intended setup is that candidates can access `#testnet-onboarding` but not the validator-only channels, while accepted validators can access the full Testnet Validator section.

## 3. Test Antoine's README

Run the documented process exactly as written. Do not silently fix commands while testing: first record the problem, then test the correction separately.

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

Never share seed phrases, private keys, validator signing keys, passwords, or other secrets in feedback or screenshots.

### README issue format

Use one entry per issue:

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

### Feedback message to Antoine

> Hey Antoine, I completed a clean run of the Test13 validator README.
>
> Environment: `[OS, architecture, relevant versions]`
> Result: `[successful / blocked at step X]`
> Setup time: `[duration]`
>
> Blocking issues:
> - `[section]: [issue and proposed correction]`
>
> Non-blocking improvements:
> - `[section]: [issue and proposed correction]`
>
> Confirmed working:
> - Genesis download and verification
> - Node startup and synchronization
> - Transaction
> - Valoper registration
>
> Full notes: `[LINK OR ATTACHMENT]`

Remove any item from "Confirmed working" that was not actually validated.

## 4. Draft onboarding process

The following is a concrete proposal to review with LOurs, Antoine, Manfred, Michelle, and Ryan. It is not final policy until they approve it.

### Proposed flow

1. A person asks to join in the general Discord channel.
2. Rémi or LOurs assigns `Testnet Validator Candidate`.
3. The candidate reads the pinned instructions in `#testnet-onboarding`.
4. The candidate completes the technical challenge.
5. Rémi and LOurs review the evidence using the same criteria for every candidate.
6. The result is `Approved` or `Needs retry`, with specific feedback.
7. An approved candidate receives `Testnet Validator` and registers through the Valopers realm.
8. Antoine approves the registration through GovDAO.
9. The validator enters the active set with voting power `1`.

### Proposed technical challenge

Ask the candidate to:

- Introduce their validator operation and provide a reliable Discord contact.
- Set up and synchronize a Test13 Gnoland node using the official README.
- Provide non-sensitive proof that the node is synchronized.
- Complete the specified on-chain transaction and provide its public identifier.
- Submit a valoper registration and provide its public link or identifier.
- Explain briefly how they monitor the node and respond to downtime or upgrades.
- Join a short technical call only when written evidence leaves material questions.

The final challenge must specify exactly which commands and public evidence are required once the Test13 README is ready.

### Proposed acceptance criteria

A candidate is approved when all mandatory criteria are met:

- [ ] Followed the published setup procedure successfully.
- [ ] Node is running and synchronized on the correct network.
- [ ] Required transaction is valid and publicly verifiable.
- [ ] Valoper registration is complete and accurate.
- [ ] Demonstrated basic understanding of keys, backups, monitoring, upgrades, and incident response.
- [ ] Communicated clearly enough for operational coordination.
- [ ] Did not expose secrets or demonstrate unsafe key handling.

A candidate receives `Needs retry` when evidence is missing, a task is incomplete, or a safety/operational issue must be corrected. Feedback must identify the failed criterion and the required next action. Decisions should not be based on reputation alone or on undocumented criteria.

### Review request to the team

> Hey everyone, LOurs and I have prepared a first draft of the Testnet validator onboarding process: `[DOCUMENT LINK]`.
>
> The proposed flow is:
>
> 1. Assign the `Testnet Validator Candidate` role.
> 2. Ask the candidate to complete a documented technical challenge.
> 3. Review the result against objective criteria.
> 4. Give specific retry feedback or assign `Testnet Validator`.
> 5. Complete Valopers registration and GovDAO approval.
> 6. Add the validator with initial voting power `1`.
>
> Please review in particular the challenge scope, acceptance criteria, Discord flow, and public wording. Unless there are objections, we would like to finalize and pin it by `[DATE]`.

## 5. Candidate-facing Discord text

Use these messages only after the process and links have been approved.

### Reply to someone asking to become a validator

> Welcome! Anyone can apply to become a Testnet validator candidate.
>
> I have assigned you the `Testnet Validator Candidate` role. Please go to `#testnet-onboarding`, read the pinned instructions, and complete the onboarding challenge. Once you submit the requested evidence, a member of the Gno team will review it and send you the next steps.

### Pinned onboarding message

> **Testnet Validator onboarding**
>
> Anyone may apply to become a Testnet validator candidate. Admission to the validator set is based on the same technical and operational criteria for every candidate.
>
> **Process**
>
> 1. Ask for the `Testnet Validator Candidate` role in `[GENERAL CHANNEL]`.
> 2. Follow the Test13 setup guide: `[README LINK]`.
> 3. Complete the challenge below.
> 4. Post the requested public evidence in `[SUBMISSION LOCATION]`.
> 5. A member of the Gno team will review your submission and either approve it or explain what needs to be retried.
> 6. Approved candidates receive the `Testnet Validator` role, complete their Valopers registration, and are progressively added to the validator set.
>
> **Challenge**
>
> - Set up and synchronize a Test13 Gnoland node.
> - Submit: `[EXACT NON-SENSITIVE SYNC EVIDENCE]`.
> - Complete: `[TRANSACTION INSTRUCTION]` and submit its public identifier.
> - Register through the Valopers realm: `[VALOPERS LINK]`.
> - Briefly describe your monitoring, upgrade, backup, and incident-response setup.
>
> Never post seed phrases, private keys, validator signing keys, passwords, or other secrets. If you are unsure whether information is safe to share, ask before posting it.
>
> Completing the challenge does not guarantee immediate entry into the active validator set. Approved validators begin with voting power `1`, subject to available capacity and GovDAO approval.

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
> 1. Confirm that your Valopers registration is complete: `[VALOPERS LINK]`.
> 2. Send us the public registration link or identifier.
> 3. Wait for GovDAO approval and confirmation before considering your validator active.
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

## 6. Track candidate decisions

Use a shared document accessible to Rémi and LOurs. Do not store secrets or unnecessary personal information.

| Candidate | Discord | Status | Challenge submitted | Reviewers | Missing criteria | Decision date | Valoper link | GovDAO status |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Example | @example | Challenge in progress | YYYY-MM-DD | Rémi, LOurs | Transaction proof | — | — | — |

Allowed statuses:

- `Candidate`
- `Challenge in progress`
- `Needs retry`
- `Approved`
- `GovDAO pending`
- `Added to valset`

For every `Needs retry` or `Approved` result, record which published criteria were evaluated. Rémi and LOurs should both agree before assigning the validator role; escalate disagreements to Antoine.

## 7. Audit existing validators

Before changing any role:

- [ ] Export or manually record the current holders of `Testnet Validator`.
- [ ] Identify core-team validators and external validators.
- [ ] Confirm the treatment of Berty, Samourai, and OnBloc with Antoine and LOurs.
- [ ] Decide whether each remaining external validator keeps the role or has it removed.
- [ ] Notify affected people before changing roles.
- [ ] Apply the agreed role changes.
- [ ] Confirm that nobody lost necessary access accidentally.

### Decision message to Antoine and LOurs

> J'ai vérifié les membres qui ont actuellement le rôle `Testnet Validator`. La proposition de migration est disponible ici : `[LIEN VERS L'AUDIT]`.
>
> - Conserver/valider directement : `[NOMS ET RAISONS]`
> - Retirer le rôle `Testnet Validator` : `[NOMS]`
> - À discuter : `[NOMS ET QUESTIONS OUVERTES]`
>
> Merci de confirmer la liste avant que je modifie les rôles. Il faut également valider quand et comment prévenir les validateurs concernés.

### Role-removal message to an existing validator

> We are introducing a consistent onboarding process for external Testnet validators. As part of this reset, your current `Testnet Validator` role will be removed.
>
> This is not a ban or a negative judgment. If you want to apply for the new validator set, ask for the `Testnet Validator Candidate` role in `[GENERAL CHANNEL]`. You will then receive access to the instructions in `#testnet-onboarding`.
>
> If you have already completed equivalent steps, you can send us the existing evidence after receiving the Candidate role, and we will review it without asking you to repeat unnecessary work.

## 8. GovDAO handoff

### Message to Antoine after approval

> Salut Antoine, LOurs et moi avons validé le candidat suivant selon les critères d'onboarding publiés :
>
> - Candidat : `[NOM / DISCORD]`
> - Inscription Valoper : `[LIEN PUBLIC OU IDENTIFIANT]`
> - Compte rendu de la revue : `[LIEN]`
> - Voting power initial proposé : `1`
>
> Peux-tu effectuer l'approbation GovDAO et nous confirmer quand le validateur a été ajouté ?

## Definition of done for Rémi's immediate work

Rémi's immediate onboarding work is complete when:

- [ ] The README has been tested end to end and feedback has been addressed.
- [ ] Discord permissions and channel visibility have been verified.
- [ ] The challenge and acceptance criteria are approved and published.
- [ ] The pinned candidate instructions contain final commands and links.
- [ ] The existing-validator audit and migration are complete.
- [ ] A shared candidate tracker is in use.
- [ ] At least one candidate has passed through the full process, including GovDAO handoff.

The voting-power progression process (`1 → 3 → 6`) is a later task and is not required to launch onboarding.
