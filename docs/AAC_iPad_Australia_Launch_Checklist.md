# AAC iPad App: Australian Launch Checklist

Prepared for Keanu Caven, Adelaide, South Australia  
Research checked: 7 September 2026  
Product: TapBoard, TapTalk and QuickTalk, with Settings

This is a practical development and compliance guide, not legal clearance or a guarantee of App Store acceptance. It assumes an Australian launch of a standalone communication app. Final obligations depend on its claims, users, data flows, payment model and services. Have an Australian technology/privacy lawyer review those decisions and obtain regulatory advice where indicated.

**Labels:** **Required** means an applicable legal, licence or Apple requirement. **Conditional** means it becomes required when the stated condition applies. **Recommended** means a product or risk-management recommendation, not a universal legal requirement.

## 1. The decisions to make before development

| Decision | Suggested starting point | Why it matters |
| --- | --- | --- |
| Intended purpose | Help people communicate their own messages using symbols and typed text | Determines product claims and helps assess regulatory scope |
| Initial territory | Australia | Overseas distribution introduces additional jurisdiction checks |
| Target users | Define ages, communication needs and access methods explicitly | Determines vocabulary, consent, usability and child-related requirements |
| Symbols | Evaluate Mulberry; obtain Widgit or PCS quotes if their vocabulary better suits users | Each collection has its own licence |
| Data | Local phrase storage, device speech, no account initially | Reduces collection, exposure and dependence on a server |
| Payment | Compare a paid download with a free app plus permanent unlock | Simpler to understand than a recurring subscription for fixed functionality |
| NDIS sales | Specify whether sales are ordinary App Store purchases or a separate provider supply arrangement | Funding, invoicing and registration depend on the arrangement |

These are recommendations, not decisions already made for your business. The first three release gates are **symbol rights**, **TGA classification**, and **privacy/data design**. Details and sources follow.

## 2. AAC symbols: where to get them and what permission means

**A credit or “shout-out” does not replace a licence.** Obtain the artwork from an authorised source and comply with that collection’s terms. The symbols and vocabulary shown in reference screenshots are not assets you can extract for production merely because you supplied the screenshot.

| Source | Published position | Action for this app |
| --- | --- | --- |
| [Mulberry Symbols](https://mulberrysymbols.org/) | CC BY-SA 4.0. The owner permits commercial products with attribution and sharing of derived symbols under the licence. Its site says not to charge separately for the symbols themselves. | Good candidate to evaluate. Download an identified release and preserve its notices. Test suitability with your intended users. |
| [Global Symbols](https://globalsymbols.com/about/terms-and-conditions?locale=en) | A catalogue containing collections with different terms. A collection being available there does not give every collection the same licence. | Check the individual collection and original rights holder. Keep the source and licence for each asset. |
| [ARASAAC collection and licence](https://globalsymbols.com/symbolsets/arasaac?locale=en) | Listed as CC BY-NC-SA 4.0, credited to Sergio Palao and the Government of Aragon. “NC” restricts commercial use. | Do not bundle it in a commercial app under this licence. A free download with paid features or advertising is not automatically noncommercial. Separate permission would be needed for an otherwise prohibited use; do not assume it is available. |
| [Widgit commercial licensing](https://www.widgit.com/symbol-services/licensing.htm) | Offers licensing for commercial software, apps and online products; fees and rights are agreed with Widgit. | Request an app-specific agreement, including offline bundling, territories, modifications and exports. Owning a Widgit authoring product is not permission to redistribute its library in your app. |
| [PCS licensing, Tobii Dynavox](https://www.tobiidynavox.com/pages/pcs-license-request-form) | Offers a licence-request process for Picture Communication Symbols, including software, subscriptions and perpetual purchases. | Request written terms for your product. Buying Boardmaker or another AAC app does not establish redistribution rights for your app. |
| Commissioned original artwork | Rights depend on your agreement with the illustrator | Obtain a written commercial licence or copyright assignment covering app distribution, editing, marketing and export. Confirm originality and any third-party components. |

### Symbol licence checklist

- [ ] **Required:** Record collection, asset identifier, creator, source, licence/version, copyright notices and any modifications.
- [ ] **Required:** Check permission for your actual use, including monetisation, bundling and distribution.
- [ ] **Conditional:** Check export, printing, cloud delivery and editable-symbol rights before adding those features.
- [ ] **Required:** Honour attribution and modification-notice requirements. Do not imply the rights holder endorses your app.
- [ ] **Recommended:** Keep licence files and agreements with release records, not only links that might later change.
- [ ] **Recommended:** Use one coherent symbol collection initially. Test meaning and recognition rather than choosing solely for appearance.

For CC BY-SA material, adaptations carry ShareAlike obligations, and you cannot impose additional legal or effective technological restrictions on recipients’ licensed rights. Review how your app terms and App Store distribution interact with those rights. A download link alone is not a guaranteed cure for an incompatible distribution arrangement. Get permission or legal advice if compatibility is unclear. This does **not automatically mean all separately written application code must be open source**; the treatment depends on what is adapted versus collected together. [Creative Commons licence terms](https://creativecommons.org/licenses/by-sa/4.0/)

### Where to place attribution

Use **Settings → About → Symbols & Licences**. Keep notices available inside the app and reproduce required credits in exported boards or other distributed outputs. Follow any provider-specific placement or logo requirements.

For Mulberry, an attribution layout to adapt after checking your release is:

> Symbol collection: Mulberry Symbols. Rights holder: Steve Lee. Licence: CC BY-SA 4.0. Source and licence links below. Changes made by this app: [describe changes, or state none].

Link **Source** to [Mulberry Symbols](https://mulberrysymbols.org/) and **Licence** to [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). This example must be adjusted to preserve any supplied notices and accurately describe your modifications.

**The generated mockup illustrations are concept artwork.** They have not been cleared as a production AAC symbol library or validated for communication use. Replace them with licensed, tested assets.

## 3. TGA: establish the app’s regulatory position

**Required assessment before supply:** determine whether the final intended purpose makes the software a medical device, and whether an exclusion or exemption applies. Disability-compensating software can fall within the definition even when it does not diagnose or prescribe. A disclaimer calling it “not a medical device” does not decide its status. [TGA software regulation guidance](https://www.tga.gov.au/resources/guidance/understanding-how-we-regulate-software-based-medical-devices)

| Outcome | Consequence |
| --- | --- |
| Not a medical device, or legally excluded | ARTG inclusion is not required on that basis; other laws still apply |
| An exempt medical device | Some regulatory obligations can remain even without ARTG inclusion |
| A regulated device without an applicable exemption | Obtain the required ARTG inclusion before supply and meet applicable device obligations |

An exclusion must fit the actual functions; adding another function can change eligibility. [TGA software exclusions](https://www.tga.gov.au/products/medical-devices/software-and-artificial-intelligence-ai/overview/software-based-medical-device-exclusions)

- [ ] Write a one-page intended-purpose statement covering users, functions, claims, setting and limitations.
- [ ] **Recommended:** Have a regulatory adviser assess standalone AAC, relevant assistive-technology exclusions and the current legislation. Professional advice is recommended here; hiring an adviser is not itself a universal legal requirement.
- [ ] If regulated, identify classification, sponsor/manufacturer responsibilities, evidence, labelling and post-market requirements.
- [ ] Review classification again before adding therapy, diagnosis, clinical scoring or health advice.

**Unresolved:** this research does not establish the specific TGA classification of your app. The TGA has consulted on changes to assistive-technology exclusions; an old consultation is not proof of the law at launch. [TGA assistive-technology consultation background](https://www.tga.gov.au/resources/industry-guidance-and-resources/tga-learn/self-paced-online-learning/presentations/future-regulation-assistive-technologies-information-session)

## 4. Privacy and user data

An AAC app can contain intimate messages, health details, names, family photos and routines. Treat these as potentially sensitive even if the app does not ask for a diagnosis.

### Determine which Australian privacy obligations apply

The federal Privacy Act generally covers businesses above the small-business turnover threshold and certain smaller businesses. Health service providers holding health information can be covered regardless of turnover. Whether this particular app business supplies a health service and holds such information requires assessment; “small startup” is not a reliable exemption. [OAIC small-business guidance](https://www.oaic.gov.au/privacy/privacy-guidance-for-organisations-and-government-agencies/organisations/small-business), [OAIC health-service definition](https://www.oaic.gov.au/privacy/your-privacy-rights/health-information/what-is-a-health-service-provider)

**Conditional requirements where the Australian Privacy Principles apply:**

- [ ] Publish a current privacy policy and give appropriate collection notices.
- [ ] Collect only necessary information; obtain consent for sensitive information unless a lawful exception applies.
- [ ] Control use and disclosure, including overseas recipients and service providers.
- [ ] Provide access and correction processes.
- [ ] Apply reasonable security and appropriate retention, destruction or de-identification practices.

These requirements concern actual practices, not just policy wording. Assess other applicable state health/privacy rules before expanding operations or handling clinical information nationally. [OAIC APP quick reference](https://www.oaic.gov.au/privacy/australian-privacy-principles/australian-privacy-principles-quick-reference)

### Recommended first-version data design

| Data or feature | Initial approach |
| --- | --- |
| Typed and saved phrases | Store on the device; exclude content from logs and analytics |
| Speech | Use device speech synthesis; test installed voices without internet |
| Photos | Optional user-selected images; avoid broad library access |
| Account | Omit unless genuinely needed for the chosen features |
| Diagnostics | Prefer minimal diagnostics without messages, photos or identifiers |
| Cloud backup or AI | Defer until consent, access control, retention and vendor arrangements are designed |

- [ ] Audit every SDK, crash reporter, server and support form; include them in the data map.
- [ ] Verify device backup behaviour before promising that data “never leaves the iPad.” Local storage may still enter a device backup.
- [ ] Protect files, secrets and any network traffic; limit staff access if a backend exists.
- [ ] Provide deletion/reset controls with clear confirmation and explain backup limitations.
- [ ] Assess decision-making capacity and lawful representative authority. An adult user’s disability does not automatically authorise a caregiver to access their messages.
- [ ] Prepare a breach-response process. If the NDB scheme applies, eligible breaches likely to cause serious harm require notification to the OAIC and affected people. [OAIC NDB scheme](https://www.oaic.gov.au/privacy/notifiable-data-breaches/about-the-notifiable-data-breaches-scheme)

Apple separately requires a privacy-policy URL for every app. Its privacy disclosures must reflect data collected by you and relevant partners. Select “Data Not Collected” only after checking the actual implementation against Apple’s definitions. [Apple privacy-policy setup](https://developer.apple.com/help/app-store-connect/manage-app-information/manage-app-privacy/), [Apple App Privacy Details](https://developer.apple.com/app-store/app-privacy-details/)

## 5. NDIS: funding and provider rules

### Funding is assessed for the participant

NDIS funding is not a general certification of your app. A purchase must fit the participant’s disability-related needs, plan, funding criteria and available budget. The NDIA explicitly lists text-to-voice apps as an example of low-cost assistive technology. Low-cost means **less than AUD 1,500**; low cost does not by itself establish low risk or eligibility. For qualifying low-cost, low-risk items, NDIA guidance says quotes, submitted assessments and prior purchase approval are not required. Suitability and funding conditions still matter. [NDIA low-cost assistive technology](https://www.ndis.gov.au/participants/assistive-technology/types-assistive-technology/what-low-cost-assistive-technology)

**Recommended:** prepare a factual product sheet covering features, compatible iPads, access methods, price, licence duration, offline behaviour, support and limitations. Make a trial available for suitability testing if practical. [NDIA assistive-technology provider process](https://www.ndis.gov.au/providers/working-participants/assistive-technology-providers/how-provide-assistive-technology-participants)

### When registration matters

| Supply arrangement | General position |
| --- | --- |
| Ordinary private purchase | NDIS registration is not an App Store submission requirement |
| Supply to self-managed or plan-managed participants | Unregistered providers can generally supply supports outside mandatory-registration categories |
| Direct supply funded through NDIA-managed plans | Provider registration is generally required |
| A service in a mandatory-registration category | Apply the category-specific requirements |

Registered providers have applicable Practice Standards, audit, complaints, incident and worker-screening obligations. Identify the correct registration scope before applying; do not assume another service’s registration covers your app business. [NDIS Commission registration guidance](https://www.ndiscommission.gov.au/provider-registration/about-registration)

The NDIS Code of Conduct applies to registered and unregistered NDIS providers. It covers rights, privacy, competent and safe delivery, integrity, response to concerns and fair pricing. Do not charge an NDIS participant a higher goods price without reasonable justification. [NDIS Code of Conduct](https://www.ndiscommission.gov.au/rules-and-standards/ndis-code-conduct)

**2026 distinction:** mandatory registration for defined NDIS digital platforms concerns intermediary services connecting participants and support providers and processing plan-funded payments. Based on the Commission’s description, a standalone AAC tool does not appear to become such a platform simply because it is an app. This is an inference, not a determination; recheck the operative rules if you add provider matching, booking or payment services. The Commission’s explanatory page still references draft definitions. [Digital-platform registration guidance](https://www.ndiscommission.gov.au/about-us/ndis-commission-reform-hub/mandatory-registration/mandatory-registration-digital)

### Payments, records and claims

- [ ] Decide who the supplier is and who receives payment in each sales channel.
- [ ] For direct provider sales, prepare invoices with supplier details, ABN where required, participant details, description, date, amount and applicable support information.
- [ ] Confirm any support item with current guidance and the plan manager; do not invent a universal AAC billing code.
- [ ] For App Store sales, confirm whether the Apple receipt and proposed reimbursement process are acceptable before promising a plan-managed route.
- [ ] Avoid duplicate invoices or claims for the same licence. A separate genuine setup service must be identified and priced separately.

The payment process differs for self-managed, plan-managed and NDIA-managed funding. [NDIA guide to getting paid](https://www.ndis.gov.au/providers/pricing-and-payments/payments/guide-getting-paid)

Do not advertise “NDIS approved,” guaranteed reimbursement or registered-provider status without a valid factual basis. The official NDIS logo needs written consent; registered-provider logos have their own eligibility rules. A normal informational funding page does not require you to display an NDIS logo. [NDIS logo guidelines](https://www.ndis.gov.au/contact/feedback-and-enquiries/ndis-logo-guidelines)

Suggested funding wording to review:

> Funding may be available where this app meets your individual plan and applicable NDIS funding requirements. Confirm your purchasing arrangements before buying. Funding is not guaranteed.

## 6. Apple App Store requirements

### Developer account and release build

- [ ] Enrol in the Apple Developer Program under the intended seller. Individual/sole-trader and organisation enrolments have different identity requirements; organisations generally need a legal entity and D-U-N-S number. Review the displayed seller name before choosing. [Apple enrolment](https://developer.apple.com/programs/enroll/)
- [ ] Meet the current submission SDK requirement. As checked, since 28 April 2026 Apple requires Xcode 26 or later and the applicable iOS/iPadOS 26 SDK or later. This is a build requirement, not a requirement to drop all older supported iPads. [Apple upcoming requirements](https://developer.apple.com/news/upcoming-requirements/)
- [ ] Supply an actual working build, accurate metadata and real app screenshots. Use TestFlight for pre-release testing. The generated mockups do not replace screenshots of the finished app. [Apple submission guidance](https://developer.apple.com/app-store/submitting/)
- [ ] Complete the age-rating questionnaire honestly, including relevant content and capabilities. A low age rating and Kids Category membership are different decisions. [Apple age ratings](https://developer.apple.com/help/app-store-connect/manage-app-information/set-an-app-age-rating/)
- [ ] Assess export compliance for encryption, including OS-provided encryption, and provide the required declaration or documentation. Do not remove security to avoid this assessment. [Apple export compliance](https://developer.apple.com/help/app-store-connect/manage-app-information/overview-of-export-compliance/)

### App Review essentials

**Required:** own or license content; use permitted APIs; provide a complete, secure, functional app and accurate claims. Give reviewers access and explain non-obvious features. Include an accessible privacy-policy link in the app. Request permissions only for features that need them. For Australian in-app digital unlocks, plan to use Apple’s payment system unless a specific permitted exception applies; do not assume another storefront’s external-payment rules apply.

**Conditional:** Kids Category apps require parental gates for external links and purchases and impose strict advertising/analytics restrictions. If you introduce public user-content sharing, implement applicable moderation, reporting and blocking controls. Local private AAC messages are a different product design from a public content platform.

Review sections 1.2, 1.3, 1.4, 2.1, 3.1, 5.1 and 5.2 against the finished app. [Apple App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/)

If adding third-party social login, also assess section 4.8 and its equivalent-login requirements and exceptions.

### Purchases and accounts

- [ ] **Conditional:** Use StoreKit for applicable in-app purchases and restore restorable purchases. Test cancelled, interrupted, refunded and restored transactions. [Apple In-App Purchase](https://developer.apple.com/in-app-purchase/)
- [ ] **Conditional:** A subscription needs clear duration, benefits, full renewal price, trial terms where offered, restoration/access for subscribers, and Terms of Use and Privacy Policy links. [Apple subscriptions](https://developer.apple.com/app-store/subscriptions/)
- [ ] **Conditional:** If accounts can be created, let users initiate account deletion inside the app; deactivation alone is insufficient. [Apple account deletion](https://developer.apple.com/support/offering-account-deletion-in-your-app/)
- [ ] Select Apple’s standard EULA or an appropriate custom agreement. Apple supplies a standard EULA when no custom one is provided; a bespoke agreement is not universally required. Preserve third-party symbol rights. [Apple licence agreements](https://developer.apple.com/help/app-store-connect/manage-app-information/provide-a-custom-license-agreement/)

**Recommended commercial design:** keep core communication available during routine billing recovery and preserve saved vocabulary after entitlement changes. Clearly explain what remains accessible. Do not make loss of a user’s words an accidental consequence of a payment error.

### Privacy implementation

- [ ] Review required-reason API use and declarations in privacy manifests. [Apple required-reason APIs](https://developer.apple.com/documentation/bundleresources/describing-use-of-required-reason-api)
- [ ] Include required third-party SDK manifests/signatures and audit their actual data behaviour. [Apple SDK requirements](https://developer.apple.com/support/third-party-SDK-requirements/)
- [ ] If you introduce cross-company tracking, assess App Tracking Transparency and legal consent; avoid tracking in the initial app. [Apple user privacy and data use](https://developer.apple.com/app-store/user-privacy-and-data-use/)

**Recommended technical starting point:** Apple’s `AVSpeechSynthesizer` for typed and card speech. Select from available device voices, offer a preview and test fallback behaviour. Text-to-speech playback does not itself require microphone recording. Add microphone permissions only if a later recording feature needs them. [Apple speech synthesis](https://developer.apple.com/documentation/avfaudio/avspeechsynthesizer)

## 7. Accessibility and communication quality

Australian disability-discrimination obligations can apply to digital goods and services. The Australian Human Rights Commission’s accessibility guidelines help interpret good practice; meeting a technical checklist does not itself guarantee legal compliance. Use the guidance and relevant standards as your baseline, then test the actual AAC workflows. [AHRC digital accessibility guidance](https://humanrights.gov.au/resource-hub/resources-for-organisations-businesses/disability-resources-employers/guidelines-equal-access-digital-goods-and-services)

**Recommended acceptance criteria for this app:**

- [ ] TapBoard, TapTalk, QuickTalk and Settings work with VoiceOver and supported alternative input methods.
- [ ] Symbol labels remain readable with enlarged text, sufficient contrast and without relying on colour alone.
- [ ] Buttons have large touch targets, predictable focus and clear selected states.
- [ ] Hardware keyboard and Switch Control workflows are tested where supported.
- [ ] Users can stop speech and clear a message without accidentally deleting saved vocabulary.
- [ ] Card locations stay stable during everyday use. Layout changes are deliberate and previewed.
- [ ] Essential vocabulary includes refusal, help, pain, consent and social communication, selected with users.
- [ ] A speech pathologist with AAC experience and intended users review vocabulary and interaction design.
- [ ] Silence, missing voices, Bluetooth routing, low volume, rapid taps and interruptions are handled visibly.
- [ ] A printable backup board or simple export is considered, subject to symbol export rights.

These are engineering recommendations, not a claim that each item is a separately mandated feature. Publish Apple Accessibility Nutrition Labels only for capabilities tested across common tasks. [Apple accessibility labels](https://developer.apple.com/help/app-store-connect/manage-app-accessibility/overview-of-accessibility-nutrition-labels/)

## 8. What to include on each page

The first three rows are the product you requested. The remaining rows map the controls and compliance surfaces discussed above; not every row needs a separate full-screen page.

| Page or location | Include | Status |
| --- | --- | --- |
| TapBoard | Licensed symbol cards, message bar, speak, backspace/clear and stop speech | Core product; symbol rights required |
| TapTalk | Keyboard, editable message, speak and save-to-QuickTalk | Core product |
| QuickTalk | Saved phrases; speak, add, edit and delete with appropriate confirmation | Core product |
| Settings → Speech | Available voice, preview, speed and speak-on-tap | Recommended |
| Settings → Display | Card size and readable text options | Recommended |
| Settings → Privacy | Privacy policy, data explanation and privacy contact | Apple policy access required; data obligations conditional |
| Settings → Data | Delete/reset local data, optional backup/export | Recommended; explain data loss and licence restrictions |
| Settings → Account | Delete account | Conditional on account creation |
| Settings → Purchases | Restore purchases; subscription management and disclosures where relevant | Conditional on payment model |
| Settings → About | Business identity, version, Symbols & Licences, software notices and applicable terms | Licence notices required where applicable; other details useful |
| Settings → Help | Support contact, audio troubleshooting and accessible complaint route | Supports review, consumer support and provider obligations |

**Recommended:** keep legal and purchase controls away from the main speaking surface. Protect destructive editing without preventing the communicator from expressing themselves. Use parental gates where Apple requires them; do not assume caregiver restrictions are appropriate for every adult user.

## 9. Your supporting website and documents

Use your own simple website for these pages. You do not need a separate “AAC certification website.”

| Page/document | Minimum useful content |
| --- | --- |
| Privacy Policy | Legal entity/contact; data collected and purpose; recipients; retention; deletion/access; relevant overseas processing and complaint procedure |
| Support | Contact method, supported devices, setup, speech troubleshooting and update information |
| Terms / licence information | Applicable EULA, scope of use, payment terms where relevant, third-party licence notices and consumer-rights wording |
| Symbols & Licences | Collection/creator, licence links, required notices and modification details |
| Product information | Accurate functionality, accessibility, compatibility, price and limitations |
| NDIS information, if marketed | Conditional funding explanation, purchasing route and factual documentation for assessment |
| Accessibility statement | Supported access methods, known limitations and feedback contact; recommended |

Do not publish a generic privacy template that says you collect nothing while an SDK sends data. Do not promise response times, lifetime support or offline functionality unless you can deliver them.

Australian Consumer Law applies to relevant software sales and consumer guarantees cannot simply be replaced with an “all sales final” policy. Describe remedies accurately and provide a support route. Apple’s refund process does not erase applicable Australian rights. [ACCC consumer remedies](https://www.accc.gov.au/consumers/problem-with-a-product-or-service-you-bought)

## 10. Adelaide business setup, children and taxes

- [ ] **Conditional:** Register a business name when trading under a name requiring registration. Check the app/business name before investing in branding. Business-name registration does not give trade mark exclusivity. [Australian business-name and trade mark guidance](https://business.gov.au/planning/protect-your-brand-idea-or-creation/difference-between-a-business-name-and-a-trade-mark)
- [ ] Establish the seller entity, ABN eligibility, bookkeeping, contracts and ownership of developer/illustrator work.
- [ ] **Conditional:** Check GST registration. The usual business threshold is AUD 75,000 GST turnover, assessed under the ATO rules. [ATO GST registration](https://www.ato.gov.au/businesses-and-organisations/gst-excise-and-indirect-taxes/gst/registering-for-gst)
- [ ] **Conditional:** Do not assume an NDIS purchase is GST-free. NDIS-specific GST treatment has conditions, including a relevant plan, qualifying support, written agreement and covered supply. Ask an accountant about your actual App Store/direct-sale arrangement. [ATO NDIS GST rules](https://www.ato.gov.au/businesses-and-organisations/gst-excise-and-indirect-taxes/gst/in-detail/your-industry/gst-and-health/national-disability-insurance-scheme)
- [ ] **Recommended:** Review suitable product/public liability, professional indemnity where services are supplied, and cyber cover with a broker. Registration or contracts may impose specific insurance requirements.
- [ ] **Conditional:** Before direct child testing, training or support work in SA, check WWCC requirements for each role, including business operators. Publishing an app and undertaking child-related work are different activities. [SA WWCC requirements](https://www.sa.gov.au/topics/rights-and-law/rights-and-responsibilities/screening-checks/screening-wwcc/for-organisations/who-needs-a-check)
- [ ] **Conditional:** Check whether your child-related services require child-safe policies and a compliance statement. Obtain appropriate research/testing consent and child assent where applicable. [SA Child Safe Environment Program](https://dhs.sa.gov.au/how-we-help/ngo-and-sector-support/child-safe-environment)

**Upcoming privacy change:** the OAIC says the Children’s Online Privacy Code must be finalised and registered by 10 December 2026. The published scope concerns specified online services and APP entities, with a health-service exclusion and potential additional designated entities. Do not present the draft as an already-final rule applying to all AAC apps. Review final scope and commencement before launching features used by children. [OAIC Children’s Online Privacy Code](https://www.oaic.gov.au/privacy/privacy-registers/privacy-codes/childrens-online-privacy-code)

## 11. Build and release sequence

1. **Define:** intended purpose, audience, territory, pricing and data map.
2. **Resolve rights and regulation:** choose licensed symbols; document TGA and privacy assessments.
3. **Build the core:** TapBoard, TapTalk, QuickTalk, Settings, reliable speech and local persistence.
4. **Add operational pages:** privacy, licences, support and applicable payment/account controls.
5. **Test with users:** accessible, consented testing with AAC users and relevant professionals; fix communication failures first.
6. **Prepare commercial operations:** seller identity, support, payments, tax and any NDIS supply process.
7. **Submit:** release build, genuine screenshots, declarations and reviewer notes.
8. **Maintain:** respond to issues, protect saved vocabulary, update policies and review changes to rules and licences.

### Release acceptance checklist

- [ ] Every production symbol and third-party dependency has documented distribution rights.
- [ ] Intended purpose and TGA position are documented; necessary permissions are obtained.
- [ ] Privacy policy, app disclosures and tested network behaviour agree.
- [ ] All three main workflows work on physical supported iPads.
- [ ] Saved phrases survive restart, update and interrupted saves.
- [ ] Speech works in the advertised offline conditions; unavailable voices have a clear fallback.
- [ ] Stop speech, reset/delete and data recovery behave as documented.
- [ ] Accessibility and user testing issues affecting communication are resolved.
- [ ] Purchases, restoration and account deletion are tested when applicable.
- [ ] Credits, support, legal links and reviewer information are complete.
- [ ] NDIS claims, invoices and any registration status are accurate.
- [ ] A support and incident process exists; the release can be maintained.

Keep evidence for these checks with the release: agreements, asset register, regulatory assessment, data map, policy versions, test results, known limitations and App Store submission materials.

## 12. Questions to resolve next

1. Will the app be paid once, permanently unlocked in-app, subscription-based or free?
2. Is the primary audience children, adults or both, and which access needs will version one support?
3. Will messages ever leave the device through sync, AI, diagnostics or support?
4. Will users add photos, recorded voices or exportable boards?
5. Will you sell only through Apple, or also supply directly through NDIS arrangements?
6. Will you provide assessments, training or ongoing disability support alongside the software?

**Next product idea:** trial a small, fully licensed vocabulary with Adelaide AAC users and a speech pathologist before buying a large symbol licence or adding cloud features. The most useful evidence is whether people can reliably say what they want with the app.

**Review limitation:** this guide covers the main issues identified for the described Australian app, not every law that could apply to an expanded business or overseas release. Recheck the linked official sources immediately before launch. No licence applications, provider registrations, legal filings or App Store submissions have been made by preparing this document.
