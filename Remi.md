# Rémi's Private Validator Onboarding Checklist

This file is Rémi's private working checklist and contains his personal templates for coordinating with the internal team. Public/shared onboarding material and messages for validators or candidates are in [Shared.md](Shared.md).

## 0. Do first: prepare the application launch

Complete these tasks in order before applications open:

- [ ] Ask Antoine and LOurs to confirm which current validators, if any, keep `Testnet Validator` without repeating onboarding. Use the private internal role-decision template below.
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

- [ ] Send the private message template to LOurs below.
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
- [ ] Send the appropriate private Ryan template below.

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
- [ ] Send the private README feedback template below.

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
- [ ] Send the private team-review template below.
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
- [ ] Send the private audit-decision template below and wait for confirmation.
- [ ] Notify affected people using the shared announcement before changing roles.
- [ ] Apply the approved role changes at the announced time.
- [ ] Assign the Candidate role only to people who request it.
- [ ] Confirm that requested Candidate access works correctly.

## 8. GovDAO handoff

- [ ] Confirm that the candidate passed all published criteria.
- [ ] Confirm the Valoper registration link and review record.
- [ ] Send the private GovDAO handoff template below to Antoine.
- [ ] Record the GovDAO status in the candidate tracker.

## Private internal message templates

These are Rémi's personal copy/paste templates for coordination with the team. They are not part of the shared onboarding document.

### Reply to Antoine about launch preparation

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

### Internal role-decision request

> Avant de modifier les rôles Discord existants, il nous faut valider explicitement la liste de migration.
>
> Validations directes proposées : Berty, Samourai, OnBloc `[À CONFIRMER OU MODIFIER]`
>
> Membres dont le rôle `Testnet Validator` sera retiré : `[NOMS]`
>
> Cas particuliers à discuter : `[NOMS ET RAISONS]`
>
> Antoine et LOurs, pouvez-vous confirmer ou modifier cette liste avant `[HEURE]` ? Une fois la liste validée, je publierai le message d'explication puis retirerai les anciens rôles Validator. Le rôle Candidate sera ensuite attribué uniquement aux personnes qui demanderont à candidater.

### Discord permission check — success

> Hey Ryan, I tested the validator onboarding permissions. Rémi and LOurs can manage the candidate and validator roles, and the channel visibility works as expected. Thanks.

### Discord permission check — changes required

> Hey Ryan, I tested the validator onboarding permissions. The following still needs to be adjusted:
>
> - `[MISSING PERMISSION OR CHANNEL ACCESS]`
> - `[MISSING PERMISSION OR CHANNEL ACCESS]`
>
> The intended setup is that candidates can access `#testnet-onboarding` but not the validator-only channels, while accepted validators can access the full Testnet Validator section.

### README feedback to Antoine

> Hey Antoine, I completed a clean run of the Test13 validator README.
>
> Environment: `[OS, ARCHITECTURE, RELEVANT VERSIONS]`
> Result: `[SUCCESSFUL / BLOCKED AT STEP X]`
> Setup time: `[DURATION]`
>
> Blocking issues:
> - `[SECTION]: [ISSUE AND PROPOSED CORRECTION]`
>
> Non-blocking improvements:
> - `[SECTION]: [ISSUE AND PROPOSED CORRECTION]`
>
> Confirmed working:
> - Genesis download and verification
> - Node startup and synchronization
> - Transaction
> - Valoper registration
>
> Full notes: `[LINK OR ATTACHMENT]`

Remove any unverified item from "Confirmed working" before sending.

### Onboarding review request

> Hey everyone, we have prepared a first draft of the Testnet validator onboarding process: `[DOCUMENT LINK]`.
>
> The proposed flow is:
>
> 1. Assign the `Testnet Validator Candidate` role after a person asks to apply.
> 2. Ask the candidate to follow the Valopers realm instructions and submit the required evidence.
> 3. Review the result against objective criteria.
> 4. Give specific retry feedback or assign `Testnet Validator`.
> 5. Complete the Valopers registration review and GovDAO approval.
> 6. Add the validator with initial voting power `1`.
>
> Please review the criteria, Discord flow, RPC requirement, and public wording. Unless there are objections, we would like to finalize and pin it by `[DATE]`.

### Existing-validator audit decision

> J'ai vérifié les membres qui ont actuellement le rôle `Testnet Validator`. La proposition de migration est disponible ici : `[LIEN VERS L'AUDIT]`.
>
> - Conserver/valider directement : `[NOMS ET RAISONS]`
> - Retirer le rôle `Testnet Validator` : `[NOMS]`
> - À discuter : `[NOMS ET QUESTIONS OUVERTES]`
>
> Merci de confirmer la liste avant que je modifie les rôles. Il faut également valider quand et comment prévenir les validateurs concernés.

### GovDAO handoff to Antoine

> Salut Antoine, nous avons validé le candidat suivant selon les critères d'onboarding publiés :
>
> - Candidat : `[NOM / DISCORD]`
> - Inscription Valoper : `[LIEN PUBLIC OU IDENTIFIANT]`
> - Compte rendu de la revue : `[LIEN]`
> - Voting power initial proposé : `1`
>
> Peux-tu effectuer l'approbation GovDAO et nous confirmer quand le validateur a été ajouté ?

### Final launch-readiness report

> Discord onboarding is ready for the application launch.
>
> - Candidate role and channel access tested: `[YES/NO]`
> - Role-management permissions tested: `[YES/NO]`
> - Existing-validator role removal announced and completed: `[YES/NO]`
> - Onboarding introduction pinned: `[LINK]`
> - Challenge and acceptance criteria published: `[LINK]`
> - README tested: `[YES/NO + LINK]`
> - Candidate tracker ready: `[LINK]`
>
> Remaining blockers: `[NONE OR LIST]`

## Definition of done

- [ ] The README has been tested end to end and feedback has been addressed.
- [ ] Discord permissions and channel visibility have been verified.
- [ ] The onboarding process and acceptance criteria are approved.
- [ ] Both candidate onboarding messages are published and pinned.
- [ ] The existing-validator audit and role changes are complete.
- [ ] A shared candidate tracker is in use.
- [ ] At least one candidate has passed through the full process, including GovDAO handoff.

The voting-power progression process (`1 → 3 → 6`) is a later task and is not required to launch onboarding.
