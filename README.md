# Two hardware keys in. No document that counts.

> **Status, November 4, 2026: unresolved.** I met OpenAI Daybreak's account-security requirements, including physical FIDO2 keys from the OpenAI + Yubico bundle, and reached identity verification. Persona then rejected my country of citizenship. When I chose my country of residence instead, it offered only documents I don't hold. OpenAI's support assistant says Daybreak verification **"can include residence permits"**, but the flow offers none, and Support **"can't override the verification decision or force a manual review."**

I live lawfully in Japan. I am a Russian citizen. Like every mid- to long-term foreign resident, I carry a **Japanese Residence Card (在留カード)**, a government-issued photo ID.

OpenAI's Daybreak program (its Trusted Access for Cyber program for individual security work) asks for a paid plan, Advanced Account Security and at least one physical hardware key before identity verification opens. I set all of that up, including two YubiKeys from OpenAI's own Yubico promotion. Verification is where it stops:

- **Country: Russia.** Persona: **"We're unable to verify IDs from this country."**
- **Country: Japan.** Persona offers only a **driver's license or a passport**. There is no residence card option. A foreign resident cannot hold a Japanese passport, and I don't drive.

So the flow has no document path for a lawful resident of a supported country, even though OpenAI's own support assistant says residence permits can be accepted.

## Start here

- **[Open the public incident page](https://coolak.github.io/openai-daybreak-persona-id-gap/)**
- **[Where this has been reported, and the status of each report](reports.md)**
- **[Dated timeline](timeline.md)**
- **[Machine-readable state](incident-state.json)**
- **[Bug ticket #1](https://github.com/COOLak/openai-daybreak-persona-id-gap/issues/1)**

## Short summary

| | |
|---|---|
| **Program** | OpenAI Daybreak, individual Trusted Access for Cyber |
| **Prerequisites** | Completed far enough to open identity verification, which OpenAI only opens after plan and account-security steps are done. Two YubiKeys from the OpenAI + Yubico bundle are registered |
| **Verification vendor** | Persona |
| **Citizenship path (Russia)** | "We're unable to verify IDs from this country." |
| **Residence path (Japan)** | Driver's license or passport only. No Japanese Residence Card option |
| **Documents the owner holds** | Japanese Residence Card. Neither a Japanese driver's license nor a passport usable for this check |
| **OpenAI support assistant** | "the document types can include residence permits"; Support "can't override the verification decision or force a manual review"; Daybreak "isn't available in every region" |
| **Human support** | Escalated November 4, 2026. Reply promised "in the coming days", also by email. Pending |
| **Cause** | Not established: a nationality rule, a regional rule, or a document-configuration gap in the Japan flow |
| **Remedy** | None offered |

## What is established, and what is not

**Established:** the two Persona outcomes above, as reported by the account owner; the quoted statements from OpenAI's Help Center support assistant on November 4, 2026; and OpenAI's own [Daybreak troubleshooting article](https://help.openai.com/en/articles/20001259-troubleshooting-openai-daybreak), which says Daybreak "isn't available in every region" and that Support "cannot override the decision".

**Not established:** whether OpenAI excludes Russian citizens from individual Daybreak access regardless of residence, and if so, under which published rule. Also unknown is why the Japan flow omits residence permits that the support assistant says can be accepted. No human at OpenAI has answered yet.

This report does **not** claim that OpenAI must grant Daybreak access to anyone. Trusted-access programs for cyber-capable models may legitimately have eligibility limits. The problem is that the limit, if there is one, is invisible until after a user has bought hardware keys, enabled Advanced Account Security and started identity verification. The documented path also contradicts the flow.

## The question for OpenAI

1. Is individual Daybreak access unavailable to Russian citizens who reside in a supported country? If so, please say so plainly, cite the rule, and show it on the eligibility page before users set up hardware keys and Advanced Account Security.
2. If nationality is not disqualifying, why does the Japan path omit the Japanese Residence Card, when the support assistant says Daybreak documents "can include residence permits"?
3. Is there any supported alternative: manual document review, a residence-permit path, or organization-level verification?
4. For foreign residents generally: what is the intended path for a lawful resident of Japan who holds a Residence Card but no Japanese driver's license or usable passport?

A support acknowledgement, a wait suggestion or a link to the generic troubleshooting article does not answer these questions.

## Reports and support

- OpenAI Help Center ChatKit support assistant. It answered the two points above, then **escalated the case to a support specialist** on November 4, 2026. A reply was promised "in the coming days" and by email. No human response or case identifier yet.
- [Bug ticket #1 in this repository](https://github.com/COOLak/openai-daybreak-persona-id-gap/issues/1).

See [reports.md](reports.md) for current status.

## Privacy

Names, account identifiers, email addresses, residence-card images, document numbers and the full support transcript are omitted. Quotes from OpenAI's support assistant are limited to the sentences needed to state its position. Persona's messages are quoted as the account owner observed them; no screenshot of the identity document flow is published.
