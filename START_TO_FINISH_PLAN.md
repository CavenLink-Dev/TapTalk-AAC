# TapTalk AAC: Start-to-Finish Plan

This is the broad roadmap for taking TapTalk from an idea to a maintained iPad app in Australia. Keep version one small, offline-first, and focused on reliable communication.

> This plan is a product roadmap, not legal advice, regulatory clearance, NDIS approval, or a guarantee of App Store acceptance. Recheck official requirements before launch.

## The version-one product

Build four simple areas:

1. **Talk** — tap licensed symbol cards, build a message, speak it, stop speech, backspace, and clear.
2. **TapTalk** — type a message, speak it, and save it as a reusable phrase.
3. **QuickTalk** — tap, add, edit, reorder, and delete saved phrases.
4. **Settings** — speech, display, data, privacy, symbols and licences, about, and help.

Use on-device speech and local storage first. Do not add accounts, cloud sync, AI, advertising, or social sharing until they are genuinely needed and separately assessed.

## Phase 1 — Define the product

- [ ] Choose the primary audience: children, adults, or both.
- [ ] Write the app's intended purpose in one plain-language paragraph.
- [ ] List the iPads and iPadOS versions to support.
- [ ] Choose the version-one access methods: touch, VoiceOver, hardware keyboard, and/or Switch Control.
- [ ] Decide the business model: paid download, permanent unlock, subscription, or free.
- [ ] Decide whether sales will be App Store only or also supplied directly through NDIS arrangements.
- [ ] Choose the development approach before writing app code: native SwiftUI is the current starting recommendation.

**Done when:** a one-page product brief fixes the audience, purpose, features, devices, price, and sales route.

## Phase 2 — Clear the release blockers

- [ ] Select a symbol collection and obtain written permission for the exact commercial use.
- [ ] Record every symbol's source, creator, licence, version, notices, and modifications.
- [ ] Do not copy production symbols from mockups or other AAC apps.
- [ ] Get the intended purpose and likely TGA position reviewed by a suitable Australian adviser.
- [ ] Map every piece of data the app will create, store, transmit, back up, or delete.
- [ ] Confirm which Australian privacy obligations apply to the business and product.
- [ ] Check the TapTalk name, business setup, ABN, trade mark risk, tax, and ownership of commissioned work.

**Done when:** symbol rights, TGA position, privacy scope, and product ownership are documented well enough to build safely.

## Phase 3 — Design the complete flow

- [ ] Create simple wireframes for Talk, TapTalk, QuickTalk, Settings, onboarding, help, and empty/error states.
- [ ] Keep a consistent message bar and predictable navigation.
- [ ] Keep important card positions stable.
- [ ] Define large touch targets, readable text, clear focus, sufficient contrast, and non-colour status cues.
- [ ] Plan calm feedback, subtle haptics, Reduce Motion, Increase Contrast, and Dynamic Type behaviour.
- [ ] Review the flow with AAC users, families/support people, and a speech pathologist with AAC experience.

**Done when:** every main task can be completed in the prototype without a dead end or unnecessary step.

## Phase 4 — Set up engineering

- [ ] Create the iPad app project, bundle identifier, development team, environments, and signing setup.
- [ ] Establish reusable design tokens and components for cards, buttons, tabs, message bars, and sheets.
- [ ] Define local data models for boards, cards, messages, phrases, and settings.
- [ ] Add automated formatting, static checks, unit tests, and a simple continuous-integration build.
- [ ] Keep secrets, signing files, personal messages, and user data out of GitHub.

**Done when:** a clean starter app builds locally and in continuous integration.

## Phase 5 — Build the core app

Build in this order:

- [ ] Speech service using Apple's on-device voices, with preview, speed, fallback, interruption, and stop controls.
- [ ] Talk screen and message-building behaviour.
- [ ] TapTalk keyboard workflow and speak action.
- [ ] Save-to-QuickTalk flow.
- [ ] QuickTalk phrase list with add, edit, reorder, and confirmed deletion.
- [ ] Local persistence that survives restart, app update, and interrupted saves.
- [ ] Settings for voice, speech speed, speak-on-tap, card size, data reset, privacy, licences, about, and help.

**Done when:** a user can compose, speak, save, and reuse messages reliably without an account or internet connection.

## Phase 6 — Make it accessible and resilient

- [ ] Give every interactive control an accurate VoiceOver label and useful hint where needed.
- [ ] Use touch targets of at least 44 by 44 points.
- [ ] Test Dynamic Type, VoiceOver, Switch Control, hardware keyboard, Reduce Motion, and Increase Contrast.
- [ ] Test silence, missing voices, low volume, Bluetooth audio, rapid taps, speech interruption, and device rotation.
- [ ] Make refusal, help, pain, consent, and social communication available in the starting vocabulary.
- [ ] Ensure communication remains possible after errors, payment problems, or unavailable optional services.

**Done when:** intended users can complete the key communication tasks on physical supported iPads.

## Phase 7 — Add privacy, legal, and support surfaces

- [ ] Publish a truthful privacy policy based on the finished data flow.
- [ ] Add in-app Privacy, Symbols & Licences, About, and Help pages.
- [ ] Add clear reset/delete controls with confirmation and an explanation of backup limitations.
- [ ] Create a support website with privacy, support, terms/licence information, product details, accessibility information, and accurate NDIS wording if used.
- [ ] Prepare an incident and privacy-breach response process.
- [ ] Avoid claims such as “NDIS approved”, guaranteed funding, or medical outcomes unless formally supported.

**Done when:** app behaviour, policies, licences, marketing, and support information all agree.

## Phase 8 — Test with real people

- [ ] Recruit a small, diverse group of AAC users using appropriate consent and child-safety processes.
- [ ] Test the main tasks: speak a card, build a message, type, save a phrase, and use it again.
- [ ] Include users with different communication, vision, motor, sensory, and cognitive needs.
- [ ] Record problems without collecting unnecessary message content or sensitive information.
- [ ] Fix communication failures and accessibility blockers before cosmetic improvements.
- [ ] Run a second round to confirm the fixes.

**Done when:** users can communicate successfully and the team has evidence for the release acceptance criteria.

## Phase 9 — Prepare the business and NDIS pathway

- [ ] Confirm the seller name, Apple Developer membership, banking, bookkeeping, tax, and support contact.
- [ ] Decide whether NDIS purchases are ordinary App Store purchases or direct provider supplies.
- [ ] If selling directly, prepare compliant invoices, written agreements, records, complaints handling, and any required registration.
- [ ] Keep pricing fair and never promise reimbursement.
- [ ] Create a factual product sheet covering price, supported iPads, access methods, offline behaviour, support, and limitations.

**Done when:** a customer can understand, buy, document, and receive support for the product without misleading claims.

## Phase 10 — App Store preparation

- [ ] Build with Apple's current required Xcode and SDK versions.
- [ ] Set the app name, icon, category, age rating, description, keywords, support URL, and privacy-policy URL.
- [ ] Capture genuine screenshots from the working app, not concept mockups.
- [ ] Complete App Privacy, privacy manifest, encryption/export, accessibility, and content-rights declarations accurately.
- [ ] Add StoreKit, restore purchases, subscription disclosures, or account deletion only if those features exist.
- [ ] Prepare reviewer notes explaining speech, offline behaviour, accessibility, and any non-obvious controls.

**Done when:** App Store metadata and declarations exactly match the tested release build.

## Phase 11 — Beta and launch

- [ ] Distribute the release candidate through TestFlight.
- [ ] Test fresh install, upgrade, restore, offline use, local data retention, and all supported iPad layouts.
- [ ] Fix crashes, data loss, blocked communication, purchase failures, and accessibility problems.
- [ ] Freeze the version, archive evidence, and submit it for App Review.
- [ ] Respond to review questions and change only what is understood and retested.
- [ ] Publish the support website and launch materials when the app is approved.

**Done when:** the approved app is available, support is active, and the exact shipped version is documented.

## Phase 12 — Maintain and improve

- [ ] Monitor crashes, support requests, accessibility feedback, and speech failures without logging private messages.
- [ ] Protect saved vocabulary during every update and migration.
- [ ] Keep symbol agreements, dependencies, policies, SDK requirements, TGA position, NDIS claims, and laws under review.
- [ ] Patch serious issues quickly and communicate clearly with users.
- [ ] Add cloud sync, AI, accounts, photos, recording, sharing, or overseas markets only through a new privacy, licensing, security, and regulatory review.
- [ ] Plan improvements with AAC users rather than feature volume alone.

**Done when:** each release remains supportable, accessible, legally reviewed where needed, and safer than the last.

## Final release gate

Do not launch until all of these are true:

- [ ] Every symbol and third-party dependency has documented distribution rights.
- [ ] The intended purpose and TGA position are documented.
- [ ] Actual data behaviour matches the privacy policy and App Store disclosures.
- [ ] Talk, TapTalk, QuickTalk, speech, settings, and saved data work on physical iPads.
- [ ] Critical VoiceOver and alternative-input workflows pass.
- [ ] Users have tested the main communication tasks and critical failures are fixed.
- [ ] Purchases, NDIS information, support, licences, and marketing are accurate.
- [ ] A responsible person can support and maintain the live app.

## Start here

Complete Phase 1 before building screens. The first concrete deliverable should be a one-page product brief, followed by written symbol, TGA, and privacy decisions. Those choices prevent expensive redesign later.

For the detailed legal and compliance notes behind this roadmap, read [the Australian launch checklist](docs/AAC_iPad_Australia_Launch_Checklist.md).
