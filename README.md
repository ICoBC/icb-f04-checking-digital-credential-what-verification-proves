<!--
author:   ICoBC - International Council on Badges and Credentials
email:    info@icobc.net
version:  1.0.0
language: en
narrator: UK English Female
comment:  A practical course for recruiters, admissions officers and credential receivers on running a verification, reading the result and deciding how much further evidence to ask for.

@style
:root { --icobc-navy:#02375B; --icobc-orange:#F78222; --icobc-cyan:#5DCAE7; --icobc-lime:#B1CF37; --icobc-mist:#F1F5F8; --icobc-line:#D8E2E9; --icobc-muted:#4F6576; }
body { font-family: "Open Sans", Arial, sans-serif; }
h1, h2, h3, h4 { color: var(--icobc-navy); }
a { color: var(--icobc-navy); }
table th { background: var(--icobc-mist); color: var(--icobc-navy); }
blockquote { border-left: 4px solid var(--icobc-orange); background: var(--icobc-mist); padding: 8px 16px; }
@end
-->

# Checking a Digital Credential: What Verification Proves

*For recruiters, admissions officers and anyone who receives credentials.*

## About this course

This course is for people who receive digital credentials and have to decide what to do with them. That includes HR and talent acquisition teams, quality, registry and admissions staff, and staff at professional bodies and sector associations. You do not need any prior knowledge. You will practise on realistic cases, using a standard verifier, and you will finish with a lab in which you verify five sample credentials and record a decision with reasons for each.

A digital credential can pass every technical check and still leave important questions open. This course shows you what a verification result proves, what it leaves open, and how to ask for the right amount of extra evidence without slowing down every application.

**Learning outcomes.** After this course you can:

1. Verify a digital credential with a standard verifier and read the result correctly.
2. Separate what verification proves (integrity, issuer, status) from what it does not prove (quality of assessment, current competence, identity of the presenter).
3. Check issuer credibility using registries, quality labels and accreditation status.
4. Decide what further evidence to request in proportion to the stakes.

**Workload.** About 2 hours of self-paced study, including the lab. This course covers the self-paced part. Facilitator notes in each module describe optional live or workshop elements.

**Assessment.** You complete a lab: you verify five sample credentials (valid, expired, revoked, tampered, and valid but from an unknown issuer) and record a decision with reasons. A person assesses your log using the rubric in "Assessment and badge". The file also contains a short knowledge check. Nothing in this file grades your lab.

**Badge.** "Checking a Digital Credential: What Verification Proves (Ability, L1)", alignment code ICSF-STND-L1-A. The badge evidence is your completed verification log with decisions. A badge shows that you completed the tasks and met the rubric in a controlled setting. It does not prove competence in any specific job.

**Framework alignment.** ICoBC Credentialing Skills Framework (ICSF), skill STND "Standards and interoperability" (VRITE pillar: Trustworthiness), level L1 "Contribute", stage A "Ability".

| Outcome | Module | How it is assessed |
|---|---|---|
| 1. Verify a digital credential with a standard verifier and read the result correctly | Running a verification; Reading the result | Module quizzes; lab log (verification steps and result readings) |
| 2. Separate what verification proves from what it does not prove | Why verifiers matter; Reading the result; Beyond the signature: issuer and assessment quality | Module quizzes; lab log (statements of what is and is not proven); knowledge check |
| 3. Check issuer credibility using registries, quality labels and accreditation status | Beyond the signature: issuer and assessment quality | Module quiz; lab log (issuer check for the unknown issuer); knowledge check |
| 4. Decide what further evidence to request in proportion to the stakes | Decisions proportionate to the stakes | Module quiz; lab log (decisions with reasons); knowledge check |

**A note on status.** Some topics in this course are still developing, in particular wallets under the European digital identity framework. Status as of November 2026; check before publishing.

## Why verifiers matter

### The problem a verifier solves

Before digital credentials, a certificate was a piece of paper or a PDF. Anyone with a scanner and a little skill could change a name or a grade. Receivers had two options: trust the document or phone the issuer. Phoning scales badly. A recruiter who receives 300 applications for one post cannot call 300 institutions.

A digital credential built on an open standard carries its proof with it. The issuer signs the data cryptographically. A verifier, which is a tool that reads the credential and checks the signature, can then answer three questions in seconds:

- **Integrity:** has the data changed since the issuer signed it?
- **Issuer:** which organisation signed it, and can the signing key be linked to that organisation?
- **Status:** is the credential still in force, or has it expired or been revoked?

These three checks are the core of what verification proves. Everything else you want to know about a credential needs another source.

### Open standards and portability

Several open specifications describe how credentials are structured and secured. Open Badges 3.0 and Comprehensive Learner Record (CLR) 2.0 are current specifications for badges and richer learner records. They build on the W3C Verifiable Credentials Data Model 2.0, which has been a W3C Recommendation since 2025. Related specifications for status lists and for securing mechanisms continue to evolve, so tools may differ in which versions they support.

For a receiver, the value of open standards is portability. A credential issued by one organisation can be checked by a verifier built by a different organisation, because both follow the same published rules. The earner can also keep the credential in a wallet of their choice and share it with any receiver.

Platform support is still uneven. Some tools handle only part of a specification. When you choose a verifier, look for evidence of conformance certification from the standard's owner or a recognised test programme, and do not rely on a tool's own claim of "compatibility". <!-- VERIFY: name the current conformance certification programme for Open Badges 3.0 and CLR 2.0 and its status before publishing. -->

### Where this fits in the bigger picture

Verification is one step in a chain of trust. The chain runs from the learning and assessment, through the issuer's decision to award, to the signed credential, to the earner who presents it, to you. A verifier tests only the middle links. The links before and after need other kinds of checks, and later modules cover them.

**Graphic: what a verifier checks along the chain of trust**

<svg viewBox="0 0 800 300" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Chain of trust from assessment to receiver</title>
  <desc>Five boxes in a row: assessment, issuer decision, signed credential, presenter, receiver. A bracket under the middle box and the signature step shows that a verifier checks integrity, issuer and status only. Assessment quality and presenter identity sit outside the bracket.</desc>
  <rect x="0" y="0" width="800" height="300" fill="#FFFFFF"/>
  <rect x="20" y="40" width="130" height="70" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="85" y="80" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Assessment</text>
  <rect x="175" y="40" width="130" height="70" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="240" y="72" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Issuer</text>
  <text x="240" y="92" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">decision</text>
  <rect x="330" y="40" width="130" height="70" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
  <text x="395" y="72" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#FFFFFF">Signed</text>
  <text x="395" y="92" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#FFFFFF">credential</text>
  <rect x="485" y="40" width="130" height="70" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="550" y="80" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Presenter</text>
  <rect x="640" y="40" width="130" height="70" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
  <text x="705" y="80" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Receiver</text>
  <line x1="150" y1="75" x2="175" y2="75" stroke="#02375B" stroke-width="2"/>
  <line x1="305" y1="75" x2="330" y2="75" stroke="#02375B" stroke-width="2"/>
  <line x1="460" y1="75" x2="485" y2="75" stroke="#02375B" stroke-width="2"/>
  <line x1="615" y1="75" x2="640" y2="75" stroke="#02375B" stroke-width="2"/>
  <path d="M 330 150 L 330 165 L 460 165 L 460 150" fill="none" stroke="#B1CF37" stroke-width="2"/>
  <rect x="290" y="180" width="210" height="60" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="395" y="205" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Verifier checks:</text>
  <text x="395" y="225" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">integrity, issuer, status</text>
  <text x="85" y="150" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">Not checked by</text>
  <text x="85" y="170" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">the verifier</text>
  <text x="550" y="150" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">Not checked by</text>
  <text x="550" y="170" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">the verifier</text>
</svg>

### Credentials from agents and auto-filled forms

Some applications are now filled in by software, including AI assistants acting for the applicant. Such a tool may attach a credential file on the applicant's behalf. A verifier can confirm that the file is intact and issued by a particular organisation. It cannot tell you whether the person or agent presenting the file is the person the credential was issued to. The link between a credential and the person presenting it is called holder binding. Module 3 explains it and module 5 shows how to respond to it.

**Worked example: a bulk shortlisting task in a corporate academy**

Amara works in the HR department of a logistics company that runs its own corporate academy. For an internal move into a team-lead programme, 40 staff have attached badges from the academy's leadership course. Before the audit, Amara opened each PDF and checked that it "looked right". She now runs each badge through a standard verifier instead. In 10 minutes (illustrative) she can state three things for each badge: the data is unchanged, the signing organisation is the academy, and the badge has not been revoked. She notes that she has not yet checked how the course was assessed. That is a separate question, covered in module 4.

**Practice activity: sort the questions**

Below are six questions a receiver might ask. Decide which a verifier can answer and which need another source. Write your sorting in your own notes, then open the answer.

1. Has the credential data been altered since issue?
2. Did the course include a proctored exam?
3. Which organisation signed the credential?
4. Is the person on the screen the person named in the credential?
5. Has the credential been revoked?
6. Can this person still do the task today?

{{1}}
<details><summary>Answer</summary>
A verifier can answer questions 1, 3 and 5. Questions 2, 4 and 6 need other sources: the issuer's published assessment information, a check of the presenter's identity, and fresh evidence of current performance.
</details>

<details><summary>Facilitator notes</summary>
Optional 20-minute live element: show a printed paper certificate and a verifiable credential side by side. Ask participants what each lets them check without contacting the issuer. Collect answers on a flipchart under the headings "Integrity", "Issuer", "Status" and "Other". Keep vendor names out of the discussion.
</details>

**Quiz: Why verifiers matter**

**Question 1.** Which three things does a verification of a standard digital credential establish?

[( )] Quality of assessment, current competence and identity of the presenter
[(X)] Integrity of the data, identity of the signing issuer and current status
[( )] Learning hours, grade and employer reputation
[( )] Whether the earner will succeed in a job

****
Verification tests the cryptographic proof and the status information. These give you integrity, issuer and status. The other options describe matters that need separate evidence.
****

**Question 2.** Why is portability a benefit of open standards for a receiver?

[( )] It guarantees that every credential is of high quality
[( )] It removes the need to consider the issuer
[(X)] A verifier built by one organisation can check a credential issued by another, because both follow the same published rules
[( )] It makes every wallet and platform behave identically

****
Open standards let different tools interoperate. They do not guarantee quality, and support still varies between platforms, so conformance should be checked.
****

**Question 3.** A tool claims to be "compatible with Open Badges 3.0". What is a sensible next step?

[( )] Accept the claim, because the tool names the standard
[(X)] Look for evidence of conformance certification before relying on the tool
[( )] Use only tools from large organisations
[( )] Avoid digital credentials altogether

****
Platform support is uneven, so a claim on its own is weak evidence. Conformance certification gives you better assurance.
****

**Question 4.** A job application is filled in by software and attaches a credential file. What can a verifier tell you about the file?

[( )] That a human applicant approved the content
[( )] That the person who sent the application is the credential holder
[(X)] That the file is intact and which organisation signed it, but not who is presenting it
[( )] That the applicant is competent today

****
A verifier tests the credential, not the presenter. Linking the presenter to the credential is holder binding, covered later in this course.
****

## Running a verification

### What you need

You need three things to run a verification: the credential itself, a standard verifier, and a clear idea of what you want to learn. The credential may arrive as a file, a link, a QR code or a share from a wallet. A standard verifier is a tool that follows the open specifications and reports its results in a structured way.

When you choose a verifier, check these points:

- It states which specifications and versions it supports.
- It shows evidence of conformance certification or published test results.
- It shows the individual checks it ran, not just one green or red sign.
- It does not require you to upload the credential to a service you do not know. If the credential contains personal data, you need a lawful basis to process it, so follow your organisation's data protection policy.

<!-- VERIFY: confirm whether any public, vendor-neutral verifier is recommended by the standards owners at the time of publishing, and add a pointer in "Sources and further reading" if so. -->

### The steps

Follow the same steps for each credential. A fixed routine protects you from skipping a check when you are busy.

1. **Receive the credential through a trusted route.** Prefer a link or share action from the earner's wallet or the issuer's platform over a screenshot. A screenshot cannot be verified.
2. **Open it in the verifier.** Load the file, paste the link or scan the code.
3. **Wait for all checks to finish.** Some verifiers fetch the issuer's public key and the status information from the internet. If the verifier cannot reach these, it may show a partial result.
4. **Read the individual results.** Look at integrity, issuer and status separately.
5. **Record the result.** Write down the date and time, the verifier you used, and each result. A result can change later, for example if the credential is revoked.

### Common routes into the verifier

Credentials reach you in different forms. A badge image may carry the data inside the image file. A JSON file holds the data directly. A web link points to a page where the issuer or a platform hosts the credential. A QR code often encodes such a link. A wallet share sends the credential directly from the earner's wallet to your tool. If you only have a plain image or a PDF printout with no embedded data, a verifier has nothing to check, and you should ask for the original file or link.

**Graphic: the five steps of a verification**

<svg viewBox="0 0 800 260" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Five steps of running a verification</title>
  <desc>Five numbered boxes in a row: receive through a trusted route, open in a verifier, wait for all checks, read each result separately, record the result with date and verifier.</desc>
  <rect x="0" y="0" width="800" height="260" fill="#FFFFFF"/>
  <rect x="10" y="60" width="140" height="120" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="80" y="90" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">1</text>
  <text x="80" y="120" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Receive via a</text>
  <text x="80" y="140" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">trusted route</text>
  <rect x="165" y="60" width="140" height="120" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="235" y="90" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">2</text>
  <text x="235" y="120" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Open in a</text>
  <text x="235" y="140" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">verifier</text>
  <rect x="320" y="60" width="140" height="120" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="390" y="90" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">3</text>
  <text x="390" y="120" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Wait for all</text>
  <text x="390" y="140" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">checks</text>
  <rect x="475" y="60" width="140" height="120" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="545" y="90" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">4</text>
  <text x="545" y="120" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Read each</text>
  <text x="545" y="140" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">result separately</text>
  <rect x="630" y="60" width="160" height="120" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="710" y="90" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">5</text>
  <text x="710" y="120" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Record result,</text>
  <text x="710" y="140" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">date and verifier</text>
  <line x1="150" y1="120" x2="165" y2="120" stroke="#02375B" stroke-width="2"/>
  <line x1="305" y1="120" x2="320" y2="120" stroke="#02375B" stroke-width="2"/>
  <line x1="460" y1="120" x2="475" y2="120" stroke="#02375B" stroke-width="2"/>
  <line x1="615" y1="120" x2="630" y2="120" stroke="#02375B" stroke-width="2"/>
</svg>

**Worked example: admissions check at a college**

Tomasz is a registry officer at a vocational college. An applicant for a part-time course submits a digital badge from a short programming course as evidence of prior learning. Tomasz asks the applicant to share the badge through a link rather than a screenshot. He opens the link in his team's standard verifier. The verifier shows three separate checks: the data is intact, the signature is linked to a named issuer, and the status is "active". Tomasz writes in the admissions record: date, verifier name and version, and the three results. He has not yet looked at who the issuer is or how the course was assessed. He marks those as open items.

**Practice activity: pick the better route**

For each of these four situations, decide whether the receiver should ask for a different form of the credential before verifying. Then check your reasoning.

1. An applicant pastes a screenshot of a badge into an online form.
2. An applicant sends a link from their wallet's share function.
3. A candidate sends a PDF printout of a certificate with no link or QR code.
4. A university sends a QR code that opens a hosted credential page.

{{1}}
<details><summary>Answer</summary>
Situations 1 and 3 need a different form: a screenshot and a plain printout carry no verifiable data, so ask for the original file or a share link. Situations 2 and 4 can go straight into the verifier.
</details>

<details><summary>Facilitator notes</summary>
Optional 30-minute live element: prepare five sample credentials in different forms (file, link, QR code, wallet share, screenshot). Let pairs of participants open each in the verifier you have chosen and note which ones can be verified. Discuss what to say to an applicant who sends a screenshot.
</details>

**Quiz: Running a verification**

**Question 1.** Which form of a credential can a standard verifier check?

[( )] A screenshot of a badge
[( )] A photographed printout
[(X)] A credential file or share link that carries the signed data
[( )] A text message saying "I have the badge"

****
A verifier needs the signed data. Screenshots and printouts contain only an image and cannot be checked cryptographically.
****

**Question 2.** What is the main advantage of a verifier that shows each check separately?

[(X)] You can see which of integrity, issuer and status passed or failed
[( )] It makes the tool faster
[( )] It removes the need to record the result
[( )] It proves the course was good

****
Separate results let you judge each check and explain your decision. A single sign can hide the reason for a problem.
****

**Question 3.** The verifier cannot reach the internet and shows a partial result. What should you do?

[( )] Treat the credential as valid
[( )] Treat the credential as fake
[(X)] Restore the connection and run the verification again before deciding
[( )] Ask the earner to confirm that it is valid

****
Some checks, such as fetching the issuer's key or the status, need a connection. A partial result is incomplete, so repeat the check rather than guess.
****

**Question 4.** Why do you record the date, time and verifier used?

[( )] The standard requires you to publish it
[(X)] A result can change later, for example after revocation, and you may need to show what you checked and when
[( )] It improves the signature
[( )] It gives the earner a record

****
Status can change over time. A record lets you explain your decision and shows which tool and version produced the result.
****

## Reading the result

### The main outcomes

A verifier typically reports one of a small number of outcomes. The wording differs between tools, so learn the meaning rather than the label.

| Outcome | Meaning | Typical next step |
|---|---|---|
| Valid | Data is intact, the signature matches a key, and the status is active | Continue to issuer and assessment checks |
| Expired | The issuer set an end date and it has passed | Ask whether a renewal exists; decide whether expiry matters for your purpose |
| Revoked | The issuer withdrew the credential | Do not rely on it; ask the earner and, where appropriate, the issuer |
| Tampered | The data does not match the signature | Do not rely on it; treat as a serious warning |
| Valid but unknown issuer | The signature is correct, but you cannot link the issuer to a known organisation | Check the issuer using registries before relying on it |

Expired does not always mean the earner lacks the skill. Some credentials are time-limited by design, for example a safety certificate with a renewal cycle. An expired credential tells you that the issuer no longer vouches for it. Revoked is different: the issuer has withdrawn its statement, sometimes because of error or misconduct. Tampered means that something in the data changed after signing, which can come from a deliberate change or from a corrupted file. Either way you cannot rely on it.

### What "valid" proves and does not prove

A "valid" result proves three things: the data has not changed, a specific key signed it, and the issuer has not revoked it. A signature shows that a key holder signed this data. Whether that key belongs to a trustworthy organisation is a question for the issuer check in module 4.

A valid result does not prove:

- **Quality of assessment.** The credential may reward attendance, a quiz or a rigorous practical exam. The signature looks the same in all cases. A 2026 symposium discussion made this point clearly: a valid signature does not certify assessment quality.
- **Current competence.** Skills fade and fields change. A credential records a past decision.
- **Identity of the presenter.** The file can be passed to someone else, or presented by software acting for the applicant.

**Graphic: proves and does not prove**

<svg viewBox="0 0 800 400" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>What verification proves and does not prove</title>
  <desc>Two columns. The left column, labelled verification proves, lists integrity, issuer and status. The right column, labelled verification does not prove, lists quality of assessment, current competence and identity of the presenter.</desc>
  <rect x="0" y="0" width="800" height="400" fill="#FFFFFF"/>
  <rect x="30" y="30" width="350" height="340" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <rect x="420" y="30" width="350" height="340" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <rect x="30" y="30" width="350" height="50" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="205" y="62" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="18" fill="#02375B">Verification proves</text>
  <rect x="420" y="30" width="350" height="50" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
  <text x="595" y="62" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="18" fill="#02375B">Verification does not prove</text>
  <rect x="55" y="110" width="300" height="60" rx="6" fill="#FFFFFF" stroke="#D8E2E9" stroke-width="2"/>
  <text x="205" y="146" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Integrity: data unchanged</text>
  <rect x="55" y="190" width="300" height="60" rx="6" fill="#FFFFFF" stroke="#D8E2E9" stroke-width="2"/>
  <text x="205" y="226" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Issuer: which key signed</text>
  <rect x="55" y="270" width="300" height="60" rx="6" fill="#FFFFFF" stroke="#D8E2E9" stroke-width="2"/>
  <text x="205" y="306" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Status: not expired or revoked</text>
  <rect x="445" y="110" width="300" height="60" rx="6" fill="#FFFFFF" stroke="#D8E2E9" stroke-width="2"/>
  <text x="595" y="146" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Quality of assessment</text>
  <rect x="445" y="190" width="300" height="60" rx="6" fill="#FFFFFF" stroke="#D8E2E9" stroke-width="2"/>
  <text x="595" y="226" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Current competence</text>
  <rect x="445" y="270" width="300" height="60" rx="6" fill="#FFFFFF" stroke="#D8E2E9" stroke-width="2"/>
  <text x="595" y="306" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Identity of the presenter</text>
</svg>

### Holder binding

Holder binding links a credential to the person or agent presenting it. Some credential formats and wallets support a proof from the holder, for example the holder's wallet signs a fresh request from the verifier to show control of a key. If your verifier supports such a presentation check, a pass means the presenter controls the key the credential was issued to. It still does not prove that the person at the keyboard is a particular human being, because the key can sit in an app that software drives.

Without holder binding, a file can be copied and presented by anyone. This matters most when applications are auto-filled or when an AI agent submits on someone's behalf. In such cases, treat the credential as a claim about the earner and look for a separate way to link the presenter to the earner when the stakes call for it. Module 5 covers when and how.

The European digital identity framework is relevant here. Member States must offer at least one EUDI Wallet by 24 December 2026. Germany plans its state wallet ("d-you") for 2 January 2027, with basic functions first. Regulated private sectors must accept the wallet about one year after issuance starts. Readiness varies widely between Member States. This is an emerging area, so do not assume that applicants or institutions can use a wallet today. Status as of November 2026; check before publishing. <!-- VERIFY: confirm Member State wallet availability, the German wallet date, and the acceptance timeline against current official sources before publishing. -->

**Worked example: a revoked badge at a corporate academy**

Priya works in talent acquisition at a manufacturing firm. A candidate for a quality technician role attaches a "Lean Practitioner" badge. Priya runs it through the verifier. The result is: integrity intact, issuer recognised, status revoked. She does not reject the candidate at once. She writes in her notes: "Badge revoked by the issuer; reason unknown." She asks the candidate to explain and to supply any replacement credential. The candidate replies that the badge was reissued after a name correction and sends the new link. Priya verifies the new one: all three checks pass. Her note records both results.

**Practice activity: read five results**

Read these five short result summaries. For each, write in one line what you can state and what you cannot state. Then compare with the answer.

A. Integrity intact, issuer recognised, status active.
B. Integrity failed.
C. Integrity intact, issuer not recognised, status active.
D. Integrity intact, issuer recognised, status expired on 1 March 2026.
E. Integrity intact, issuer recognised, status revoked.

{{1}}
<details><summary>Answer</summary>
A: you can state that the data is unchanged, a known issuer signed it and it is in force; you cannot state anything about assessment quality, current skill or who presents it. B: you cannot rely on the data at all. C: the data is unchanged but you cannot say who the issuer really is, so run the issuer checks. D: the issuer no longer vouches for it; ask whether a renewal exists. E: the issuer withdrew it; do not rely on it and ask for an explanation and replacement.
</details>

<details><summary>Facilitator notes</summary>
Optional 20-minute live element: show the five result screens from your chosen verifier on a shared screen and ask participants to say, in one sentence each, what they would write in the log. Stress that "invalid" is not a single category and that the reasons differ.
</details>

**Quiz: Reading the result**

**Question 1.** A verifier reports "tampered". What does this mean?

[( )] The credential has expired
[(X)] The data does not match the signature, so it cannot be relied on
[( )] The issuer is unknown but the data is fine
[( )] The earner has left the organisation

****
A tampered result means the data was altered after signing, or the file is corrupted. Either way, the credential cannot be relied on.
****

**Question 2.** A credential is "valid". Which statement is correct?

[( )] The earner is competent today
[( )] The assessment was rigorous
[(X)] The data is intact, a key signed it and the issuer has not withdrawn it
[( )] The person presenting it is the earner

****
A valid result covers integrity, issuer key and status. It says nothing about assessment quality, current competence or presenter identity.
****

**Question 3.** What does holder binding provide?

[( )] Proof that the assessment was fair
[(X)] A link between the credential and the key or wallet of the presenter
[( )] A guarantee that the issuer is accredited
[( )] A permanent guarantee of competence

****
Holder binding shows that the presenter controls the key the credential was issued to. It does not certify assessment quality or issuer standing, and it does not prove a human identity by itself.
****

**Question 4.** A credential has expired. What is a reasonable reading?

[( )] The earner never had the skill
[(X)] The issuer no longer vouches for it; ask whether a renewal exists and decide whether expiry matters for your purpose
[( )] The credential is tampered
[( )] The credential should be deleted from the record

****
Expiry shows that the issuer's statement has lapsed. Some credentials are time-limited by design, so ask about renewal before deciding.
****

**Question 5.** An application is auto-filled by software and attaches a valid credential. What is the correct reading?

[( )] The presenter is the credential holder
[(X)] The credential is intact and in force, but nothing yet links the presenter to the earner
[( )] The software has proved the assessment was rigorous
[( )] The application must be rejected

****
A valid file can be presented by anyone or anything. You need holder binding or another identity check when the stakes call for it.
****

## Beyond the signature: issuer and assessment quality

### Who is the issuer?

A signature proves that a key signed the data. It does not prove that the organisation behind the key is trustworthy. Anyone can create a key and sign a credential with an impressive name. The issuer check asks: is this organisation real, is it who it claims to be, and is it a credible source for this kind of credential?

Useful sources for an issuer check:

- **Registries.** Public registers of education providers, awarding organisations or professional bodies. Many countries and regions keep official lists. Check the register directly, not a link supplied by the earner.
- **Accreditation and recognition status.** For regulated qualifications, the competent public body or accrediting organisation publishes who is recognised. Check the status and the scope: an accredited provider may be accredited for some programmes only.
- **Quality labels and quality assurance outcomes.** Some sectors use quality labels or external review reports. Check who awards the label, whether the label is current, and whether it covers the credential in question.
- **The issuer's own information.** A credible issuer publishes who it is, how to contact it, and how its credentials are assessed and revoked.

An issuer's absence from a registry does not prove bad faith. A corporate academy or a small training provider may not appear in a national register because none applies to it. In that case, you rely on other signals and on your own proportionate checks, which module 5 covers.

<!-- VERIFY: add pointers to the relevant national or regional registries (for example the recognised-qualification registers) for the audiences' countries before publishing. -->

### How good was the assessment?

The second question is about what the credential stands for. Two credentials with the same title can reflect very different effort. Ask:

- **What was assessed?** Knowledge recall, applied tasks, workplace performance?
- **How was it assessed?** Self-declared, automated quiz, assessor judgement, supervised exam?
- **By whom?** Who made the award decision, and were they independent of the teaching?
- **Against what?** Published criteria, a framework level, an occupational standard?
- **Is there a rule for the award?** Pass mark, retake policy, evidence retention.

Open Badges 3.0 and CLR 2.0 allow issuers to include criteria, evidence and alignment to frameworks in the credential data. Look for these fields. A credential with clear criteria and an alignment statement gives you more to work with than one with only a title and an image. Fields can be filled in with marketing language, so read them critically and compare the stated criteria with the issuer's public description.

This is the point of the 2026 symposium remark: a valid signature does not certify assessment quality. The signature says nothing about how hard or easy the award was. Assessment quality needs its own evidence.

**Graphic: two separate questions after a valid result**

<svg viewBox="0 0 800 380" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Two questions after a valid signature</title>
  <desc>A navy box labelled valid signature at the top leads to two boxes below. The left box, in cyan, asks who the issuer is and lists registries, accreditation status and quality labels. The right box, in lime, asks how good the assessment was and lists criteria, evidence and independence of the assessor.</desc>
  <rect x="0" y="0" width="800" height="380" fill="#FFFFFF"/>
  <rect x="290" y="20" width="220" height="60" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="56" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#FFFFFF">Valid signature</text>
  <line x1="400" y1="80" x2="400" y2="110" stroke="#02375B" stroke-width="2"/>
  <line x1="200" y1="110" x2="600" y2="110" stroke="#02375B" stroke-width="2"/>
  <line x1="200" y1="110" x2="200" y2="140" stroke="#02375B" stroke-width="2"/>
  <line x1="600" y1="110" x2="600" y2="140" stroke="#02375B" stroke-width="2"/>
  <rect x="40" y="140" width="320" height="200" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="200" y="175" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">Who is the issuer?</text>
  <text x="200" y="215" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Registries</text>
  <text x="200" y="245" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Accreditation status</text>
  <text x="200" y="275" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Quality labels</text>
  <text x="200" y="305" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Issuer's own information</text>
  <rect x="440" y="140" width="320" height="200" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="600" y="175" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="16" fill="#02375B">How good was the assessment?</text>
  <text x="600" y="215" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Published criteria</text>
  <text x="600" y="245" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Evidence and alignment</text>
  <text x="600" y="275" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Independent assessor</text>
  <text x="600" y="305" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Award rule and retakes</text>
</svg>

### Putting the checks together

You do not need to run every check for every credential. Match the effort to the stakes, which module 5 covers. For now, practise the checks themselves. A short issuer check typically takes a few minutes: find the issuer's name in the credential, search the relevant register or accreditation list through its official site, and note whether the issuer appears, with what status and scope. A short assessment check asks you to read the criteria in the credential and the issuer's public description, and to note any gaps.

**Worked example: an unknown issuer at a university**

Sofia is an admissions officer at a university. An applicant for a master's programme submits a digital badge titled "Advanced Data Analysis". The verifier shows: integrity intact, status active, signature valid, issuer name "Northfield Learning Hub" with no match in the verifier's list of known issuers. Sofia searches the national register of recognised providers through the official site and finds no entry. She then opens the issuer's own website and finds a short description, a contact address and no information on assessment. She records: "Valid signature; issuer not found in the register; assessment method unknown." She does not call the badge fake. She writes to the applicant to ask for the course syllabus, the assessment description and a transcript or work sample, and she sets the badge aside as supporting evidence only, pending a reply.

**Practice activity: draft an issuer and assessment check**

You are a recruiter and receive a valid badge titled "Project Management Professional Skills" from an issuer called "Brightpath Academy", which is not in your verifier's list. Write four short questions you would put to the issuer's public information or to the earner, two about the issuer and two about the assessment. Compare with the sample answer.

{{1}}
<details><summary>Sample answer</summary>
Issuer: Is Brightpath Academy listed in a relevant register or accreditation list, and with what scope? Does it publish contact details and a revocation policy? Assessment: What did the earner have to do to receive the badge (for example a supervised exam, a project, or attendance only)? Who decided on the award and against which published criteria?
</details>

<details><summary>Facilitator notes</summary>
Optional 30-minute live element: give small groups the same issuer name and ask them to list the sources they would check, in order, for their own country or sector. Collect the lists and compare. Highlight that corporate academies and small providers often have no register entry, and discuss what to ask for instead.
</details>

**Quiz: Beyond the signature**

**Question 1.** A credential has a valid signature from an issuer you do not know. What is the best next step?

[( )] Accept it, because the signature is valid
[( )] Reject it, because the issuer is unknown
[(X)] Check the issuer through registries, accreditation lists or quality labels, and ask for more information about the assessment
[( )] Ask the earner to vouch for the issuer

****
A valid signature shows that a key signed the data. It does not show that the organisation behind the key is credible. Check the issuer through independent sources and ask about the assessment.
****

**Question 2.** Why should you check a register directly rather than follow a link supplied by the earner?

[( )] Links from earners are always false
[(X)] A supplied link may lead to a copy that is not the official register
[( )] Registers do not accept links
[( )] It saves time

****
Going to the official source yourself avoids relying on a page that someone else controls. Search for the register through its official site.
****

**Question 3.** An accredited provider issues a badge. What should you still check?

[( )] Nothing, accreditation covers everything
[(X)] Whether the accreditation covers the programme and is current, and how the credential was assessed
[( )] Only the colour of the badge image
[( )] Whether the earner has a wallet

****
Accreditation often applies to specific programmes and periods. Check the scope and the date, and read the assessment information.
****

**Question 4.** Which of these tells you most about assessment quality?

[( )] A well-designed badge image
[( )] A long credential title
[(X)] Published criteria, evidence and information on who made the award decision
[( )] The number of badges the earner holds

****
Criteria, evidence and the independence of the assessor describe how the award was made. Design and title say little about rigour.
****

## Decisions proportionate to the stakes

### Matching effort to the stakes

Every decision has a cost of being wrong and a cost of checking. Shortlisting someone for a first interview carries low risk, because the later steps catch errors. Awarding a place on a regulated programme, or hiring for a safety-critical or financial post, carries high risk. The further evidence you request should match the stakes. Too little leaves you exposed. Too much slows everyone and can exclude honest applicants who lack easy access to documents.

A simple way to think about stakes uses three questions:

1. **What happens if this credential is false or overstated?** Consider harm to people, legal exposure and cost.
2. **How much does this credential weigh in the decision?** A supporting detail needs less checking than the sole evidence for a requirement.
3. **Can the later steps catch an error?** A later practical test, probation or supervised work reduces the risk.

### A decision path

After the verification, use a decision path. The graphic below shows one version. You may adapt it to your organisation's policy, as long as you record the reasons.

- **Integrity failed (tampered):** reject the credential as evidence. Where there is reason to suspect deliberate falsification, follow your organisation's procedure for reporting concerns.
- **Revoked:** do not rely on it. Ask for an explanation and for replacement evidence.
- **Expired:** ask whether a renewal exists; decide whether the expiry matters for the requirement.
- **Valid, known issuer, low stakes:** accept as supporting evidence and record the checks.
- **Valid, unknown issuer or unclear assessment, low stakes:** accept with a note, or ask for a brief description of the assessment.
- **Valid, medium or high stakes:** run the issuer and assessment checks, and ask for further evidence such as a work sample, a transcript, an interview or a practical task.
- **High stakes or auto-filled application:** add a presenter check, for example a live check against an identity document or a holder-bound presentation from a wallet, in line with your data protection rules and policy.

### What further evidence can you ask for?

Choose evidence that fits what the credential claims. For a skill, a short practical task or a work sample shows current performance. For a qualification, an official transcript from the awarding organisation or a confirmation from its registry service helps. For identity, use a lawful identity check suited to your setting. For current competence, ask for recent work, a reference or a live demonstration. Explain why you ask, keep requests consistent across applicants, and offer a reasonable alternative where an applicant cannot provide the first form of evidence.

### Handling auto-filled and agent-submitted applications

When an application arrives through a form-filling tool or an AI agent, you cannot assume the applicant has seen or approved each attachment. A valid credential in such an application is still only a claim until it is linked to the person. Reasonable responses include asking the applicant to confirm and present the credential directly at a later step, using a holder-bound presentation where your tools support it, and recording that the presenter was not yet bound to the credential. Do this fairly: applicants may legitimately use assistive tools, so treat the tool as a channel and not as a sign of bad faith.

**Graphic: decision path after verification**

<svg viewBox="0 0 800 460" width="100%" role="img" xmlns="http://www.w3.org/2000/svg">
  <title>Decision path from verification result to accept, ask for more or reject</title>
  <desc>A navy start box leads to a question whether the result is tampered or revoked, which leads to reject. Otherwise a second question asks whether the issuer is known and the assessment clear. If yes and the stakes are low, accept. If no or the stakes are medium or high, ask for more evidence. High stakes or auto-filled applications add a presenter check.</desc>
  <rect x="0" y="0" width="800" height="460" fill="#FFFFFF"/>
  <rect x="290" y="15" width="220" height="50" rx="6" fill="#02375B" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="46" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="15" fill="#FFFFFF">Verification result</text>
  <line x1="400" y1="65" x2="400" y2="95" stroke="#02375B" stroke-width="2"/>
  <rect x="250" y="95" width="300" height="55" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="118" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Tampered or revoked?</text>
  <text x="400" y="138" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">(expired: ask about renewal)</text>
  <line x1="550" y1="122" x2="620" y2="122" stroke="#02375B" stroke-width="2"/>
  <text x="585" y="112" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">Yes</text>
  <rect x="620" y="95" width="160" height="55" rx="6" fill="#F78222" stroke="#02375B" stroke-width="2"/>
  <text x="700" y="128" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="15" fill="#02375B">Reject as evidence</text>
  <line x1="400" y1="150" x2="400" y2="190" stroke="#02375B" stroke-width="2"/>
  <text x="415" y="175" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">No</text>
  <rect x="250" y="190" width="300" height="55" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="213" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">Issuer known and assessment</text>
  <text x="400" y="233" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">clear, and stakes low?</text>
  <line x1="250" y1="217" x2="150" y2="217" stroke="#02375B" stroke-width="2"/>
  <text x="200" y="207" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">Yes</text>
  <rect x="20" y="190" width="130" height="55" rx="6" fill="#B1CF37" stroke="#02375B" stroke-width="2"/>
  <text x="85" y="223" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="15" fill="#02375B">Accept, record</text>
  <line x1="400" y1="245" x2="400" y2="285" stroke="#02375B" stroke-width="2"/>
  <text x="415" y="270" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#4F6576">No</text>
  <rect x="250" y="285" width="300" height="60" rx="6" fill="#5DCAE7" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="311" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="15" fill="#02375B">Ask for more evidence</text>
  <text x="400" y="332" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">in line with the stakes</text>
  <line x1="400" y1="345" x2="400" y2="380" stroke="#02375B" stroke-width="2"/>
  <rect x="200" y="380" width="400" height="60" rx="6" fill="#F1F5F8" stroke="#02375B" stroke-width="2"/>
  <text x="400" y="406" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">High stakes or auto-filled application:</text>
  <text x="400" y="426" text-anchor="middle" font-family="Open Sans, Arial, sans-serif" font-size="14" fill="#02375B">add a presenter check</text>
</svg>

**Worked example: proportionate evidence in a corporate academy and a college**

*Corporate academy.* Lena in an HR department reviews internal applications for a trainer role. A candidate presents a valid badge from an external facilitation course. The issuer is not in any register. The stakes are medium: the trainer will teach new starters but works under a lead trainer for six months. Lena accepts the badge as supporting evidence, asks for a 10-minute teach-back demonstration, and records: "Valid, issuer unlisted, assessment unknown; proportionate step: demonstration."

*College.* Marcus, a registry officer at a training provider, receives a valid certificate from a recognised awarding body for a prerequisite unit. The issuer is in the national register and the unit is within its accredited scope. The stakes are low because the course includes an early skills check. Marcus accepts, records the register check, and takes no further steps. If the applicant had applied for a licensed practice route, he would also ask for a transcript from the awarding body and a live identity check.

**Practice activity: choose the proportionate step**

For each case, choose accept, ask for more or reject, and name the further evidence if any. Then compare with the answer.

1. A valid, recognised-issuer badge supports a CV line for a junior marketing role. Stakes: low.
2. A valid badge from an unknown issuer is the only evidence of a safety qualification for a site supervisor post. Stakes: high.
3. A badge is reported as tampered by the verifier.
4. A valid badge arrives in an auto-filled application for a role with access to client funds.

{{1}}
<details><summary>Answer</summary>
1. Accept and record the checks. 2. Ask for more: run the issuer and assessment checks, request a transcript or confirmation from an awarding body and a practical assessment. 3. Reject as evidence and follow your organisation's procedure. 4. Ask for more: confirm the issuer and assessment, and add a presenter check such as a holder-bound presentation or a live identity check under your policy.
</details>

<details><summary>Facilitator notes</summary>
Optional 40-minute workshop: groups draw up a one-page evidence policy for their own organisation with three stakes levels and the evidence each level requires. Groups swap policies and test them against two or three case cards. Remind groups to include a fair alternative route for applicants who cannot supply a given form of evidence.
</details>

**Quiz: Decisions proportionate to the stakes**

**Question 1.** What does "proportionate" mean in this course?

[( )] Ask for the same evidence from everyone
[( )] Always ask for the maximum evidence
[(X)] Match the amount of further evidence to the cost of being wrong and the weight of the credential in the decision
[( )] Accept every valid credential

****
Proportionate checks balance risk and effort. Uniform minimum or maximum checks either expose you or burden applicants unnecessarily.
****

**Question 2.** Which is a sensible further step for a valid credential from an unknown issuer used as sole evidence for a high-stakes requirement?

[( )] Accept it and move on
[(X)] Check the issuer through independent sources, ask for assessment information and request supporting evidence such as a work sample or confirmation from an awarding body
[( )] Reject it without further enquiry
[( )] Ask the earner to promise it is genuine

****
High stakes and an unknown issuer call for independent checks and additional evidence. Immediate rejection may treat a legitimate provider unfairly, and reassurance from the earner is not independent.
****

**Question 3.** A valid credential arrives in an application submitted by an AI agent. What is a fair response?

[( )] Reject the application because an agent was used
[( )] Accept the credential as proof that the applicant is competent
[(X)] Treat the credential as a claim, link the presenter to the earner at a later step in proportion to the stakes, and record that this was done
[( )] Ignore the verification result

****
Assistive tools are a channel and not a sign of bad faith. A presenter check, such as a holder-bound presentation or a lawful identity check, closes the gap where the stakes call for it.
****

**Question 4.** Why should requests for further evidence be consistent across applicants?

[( )] To make the process longer
[( )] To avoid keeping records
[(X)] To treat applicants fairly and to be able to explain and defend decisions
[( )] To hide the policy from applicants

****
Consistent, documented requests support fairness and accountability. Offer a reasonable alternative where an applicant cannot supply the usual evidence.
****

## Assessment and badge

### The lab

You now complete the assessed task. It is a controlled lab: you work with sample credentials provided by your course facilitator or training provider, in a sandbox, so no real person's data is involved.

**Task.** Verify five sample credentials with a standard verifier and record a decision with reasons for each:

1. A valid credential from a known issuer.
2. An expired credential.
3. A revoked credential.
4. A tampered credential.
5. A valid credential from an unknown issuer.

For each credential, complete one row of the verification log with these fields:

- Credential reference and date and time of the check.
- Verifier used (name and version).
- Result for integrity, issuer and status, as shown by the verifier.
- What the result proves, in one or two sentences.
- What the result does not prove, in one or two sentences.
- Issuer check: sources consulted and finding (required for credential 5, and for credential 1 where the issuer is not obvious).
- Stakes level you assume for the scenario you have been given (low, medium or high).
- Decision: accept, ask for more, or reject.
- Reasons for the decision.
- Further evidence requested, if any, and why it fits the stakes.
- Note on presenter binding: whether the presenter is linked to the credential and what you would do if not.

Write in your own words. Use the sample scenario sheet from your facilitator to set the stakes.

<details><summary>Facilitator notes</summary>
Prepare five sample credentials in a sandbox, clearly marked as samples, one for each of the five types. Provide a scenario sheet that states the role or programme and the stakes for each credential, and a blank verification log template. Allow about 45 minutes for the lab. Assess the logs with the rubric below, using a person trained in the rubric. If you use two assessors, have them compare one log together first to align their judgements. Offer a second attempt after feedback. Do not grade inside this file.
</details>

### Rubric

The assessor rates each criterion as Not yet, Meets or Strong.

| Criterion | Not yet | Meets | Strong |
|---|---|---|---|
| 1. Running the verification (outcome 1) | Verification steps missing or the wrong form of credential was used | All five credentials verified with a standard verifier; tool, date and time recorded | As Meets, plus notes on the limits of the tool or the route in which each credential arrived |
| 2. Reading the result (outcome 1) | Results misread, for example expired treated as tampered | Integrity, issuer and status read correctly for all five | As Meets, plus clear explanation of why each outcome type differs in meaning |
| 3. Proves and does not prove (outcome 2) | Claims that a valid result proves quality, competence or identity | For each credential, states what is proven and what is not, including assessment quality, current competence and presenter identity | As Meets, plus links each "not proven" item to a specific follow-up check |
| 4. Issuer credibility (outcome 3) | No issuer check, or reliance on the issuer's own claims only | Issuer checked through at least one independent source (registry, accreditation status or quality label); finding recorded with scope and date | As Meets, plus compares several sources and explains what an absent entry does and does not mean |
| 5. Proportionate decisions (outcome 4) | Decisions without reasons, or the same evidence requested whatever the stakes | A decision and reasons for each credential; further evidence fits the stated stakes | As Meets, plus offers a fair alternative route and notes how the decision would change at higher or lower stakes |
| 6. Presenter binding and agents (outcomes 2 and 4) | Not mentioned | Notes that the presenter is not proven by verification and states a proportionate response | As Meets, plus applies the point to an auto-filled or agent-submitted case |
| 7. Record quality | Log incomplete or unclear | Log complete, clear and in the learner's own words | As Meets, plus consistent wording that another reader could use to repeat the decision |

### Pass rule

To earn the badge, the learner must:

- complete all five rows of the verification log with all required fields;
- reach Meets or Strong on all seven criteria (no criterion at Not yet);
- complete the knowledge check below (the module quizzes are for practice and are not scored for the badge).

A learner with any criterion at Not yet receives written feedback and may resubmit the affected rows. The assessor makes the final decision, not this file.

### Evidence submitted for the badge

- The completed verification log with decisions (all five rows).
- The assessor's rubric record, held by the awarding organisation.
- The date of completion of the knowledge check.

The badge "Checking a Digital Credential: What Verification Proves (Ability, L1)" carries the alignment code ICSF-STND-L1-A. It records that you completed the tasks and met the rubric in a controlled setting. It does not prove competence in a specific job.

### Final knowledge check

Answer all ten questions. Each has four options and one correct answer.

**Question 1.** A verifier reports that the data is intact, the signing key links to a named issuer and the credential is active. What has been proven?

[( )] The assessment was rigorous and the earner is competent today
[(X)] Integrity, issuer and status
[( )] The presenter is the earner
[( )] The issuer is accredited

****
Verification proves integrity, issuer key and status. Assessment quality, current competence, presenter identity and accreditation need separate evidence.
****

**Question 2.** An applicant sends a screenshot of a badge. What should you do?

[( )] Verify the screenshot with your standard verifier
[( )] Accept it because the image looks professional
[(X)] Ask for the original file or a share link that carries the signed data
[( )] Reject the application

****
A screenshot carries no signed data, so it cannot be verified. Ask for a form that can.
****

**Question 3.** The verifier shows "expired" for a safety certificate that renews every two years. What is the best reading?

[( )] The earner never held the skill
[( )] The credential was tampered with
[(X)] The issuer no longer vouches for it; ask whether a renewal exists and judge whether expiry matters for the requirement
[( )] The issuer is not credible

****
Expiry shows the issuer's statement has lapsed. For time-limited credentials, ask about renewal.
****

**Question 4.** A verifier reports "tampered". What follows?

[( )] Treat it as valid with a warning
[(X)] Do not rely on the credential and follow your organisation's procedure
[( )] Ask the earner to run the check again until it passes
[( )] Accept it at low stakes

****
The data does not match the signature, so it cannot be relied on at any stakes level.
****

**Question 5.** What does a valid signature say about assessment quality?

[( )] That it was rigorous
[( )] That it was independent
[(X)] Nothing, because the signature looks the same whatever the assessment method
[( )] That it matched a published framework

****
A valid signature does not certify assessment quality. Look at criteria, evidence and the award decision to judge it.
****

**Question 6.** Which source is best for checking whether an issuer is recognised?

[( )] A link in the earner's email
[( )] The issuer's own marketing page alone
[(X)] The official register or accreditation list of the competent body, reached through its official site
[( )] A social media profile of the issuer

****
Independent, official sources give the most reliable evidence. Supplied links and self-descriptions are weaker.
****

**Question 7.** An issuer does not appear in a national register. What is a fair conclusion?

[( )] The credential is fake
[( )] The credential is high quality because it is unregulated
[(X)] The absence is a signal to follow up with other checks, not proof of bad faith
[( )] The verifier is faulty

****
Many corporate academies and small providers do not appear in registers. Use other signals and proportionate further evidence.
****

**Question 8.** Which approach matches the idea of proportionate evidence?

[( )] Ask for identical documents from every applicant, whatever the role
[(X)] Ask for more evidence as the cost of error and the weight of the credential increase, and record the reasons
[( )] Accept all valid credentials at every stakes level
[( )] Reject all credentials from unknown issuers

****
Proportionate checks match effort to risk and are documented so that they can be explained.
****

**Question 9.** An AI agent submits an application with a valid credential for a role with access to client funds. What is the best response?

[( )] Reject the application because an agent submitted it
[( )] Accept the credential because the verifier passed it
[(X)] Treat the credential as a claim and add a presenter check, such as a holder-bound presentation or a lawful identity check, in line with the stakes and your policy
[( )] Ask the agent to confirm its own identity

****
A valid file can be presented by anyone or anything. Holder binding or an identity check links the presenter to the earner when the stakes call for it.
****

**Question 10.** Which statement about open standards for credentials is accurate?

[( )] Conformance claims by tools need no checking
[( )] Open standards guarantee the quality of every credential
[(X)] Open standards support portability, but platform support is uneven, so check conformance certification of tools
[( )] Open Badges 3.0 and CLR 2.0 are no longer current

****
Open Badges 3.0 and CLR 2.0 are current specifications built on the W3C Verifiable Credentials Data Model 2.0. They help portability, and tool support varies.
****

## Sources and further reading

Status as of November 2026; check before publishing.

- 1EdTech Consortium: Open Badges 3.0 specification and Comprehensive Learner Record (CLR) Standard 2.0 specification, published on the 1EdTech website (1edtech.org). Check the website for the current version and the conformance certification programme.
- World Wide Web Consortium (W3C): Verifiable Credentials Data Model v2.0, W3C Recommendation, published on the W3C website (w3.org/TR). Check the same site for related specifications on securing mechanisms and status lists, which continue to evolve.
- European Union: Regulation (EU) 2024/1183 amending Regulation (EU) No 910/2014 as regards establishing the European Digital Identity Framework (eIDAS 2.0), published in the Official Journal of the European Union and available through EUR-Lex (eur-lex.europa.eu). <!-- VERIFY: confirm the regulation number and the Member State wallet and sector acceptance dates against EUR-Lex and the European Commission's digital identity pages before publishing. -->
- European Commission: pages on the European Digital Identity Wallet, published on the European Commission website. Check the current implementation status for your Member State, including the German state wallet plan.
- ICoBC: Credentialing Skills Framework (ICSF) and VRITE pillars, published by the International Council on Badges and Credentials (icobc.net). Check the ICoBC website for the current framework text.

**Time-sensitive facts in this course.** The dates for the EUDI Wallet (24 December 2026 for Member State offers, 2 January 2027 for the planned German wallet, and acceptance by regulated private sectors about one year after issuance starts) and the state of tool and platform support for Open Badges 3.0, CLR 2.0 and related W3C specifications can change. Status as of November 2026; check before publishing.
