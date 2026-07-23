# ToolBelt: Two Experiences, One Marketplace — Proposal PRD

**For:** Product, Engineering, Executive team, and the designers on the project
**From:** Andrew (Design) — drafted with Cowork
**Date:** 2026-07-22
**Status:** A proposal to share ideas and align. Not a locked spec. The prototypes and Figma files referenced here are idea-sharing artifacts; requirements and designs continue to evolve with the business and product teams and other designers.

## Links

- **Vision landing page:** https://toolbelt-vision.vercel.app
- **Individual experience prototype** (public-facing, social; + reference business suite): https://prototype-liart-seven.vercel.app
- **Business enterprise ERP prototype** (the Next prototype, emerging direction): https://toolbelt-next.vercel.app/
- **Product vision deck** (Google Slides): https://docs.google.com/presentation/d/1i5Zm7wcuGRVNKFOJFKSaANX_tPpPU197cFhoeJiNaxw/edit
- **FigJam — Journey Maps:** https://www.figma.com/board/ouaz6cnUkB7wauTlpbt8Tb
- **FigJam — User Flows** (web + mobile): https://www.figma.com/board/BjmEbUF8HvvV3y4qwESkcB
- **FigJam — Platform Map** (device strategy): https://www.figma.com/board/agvFb5s2g27SVAXBpU4n3Z
- **Figma — Consumer-First Save Sequence** (coachmarks, full chain): https://www.figma.com/board/TZvirnfukvXOkbb6jffjrk/Consumer-First-Save-Sequence-with-Coachmarks--full-chain-

---

## 0. What this document is for

**The ask: align on the individual experience layer.** The individual (consumer / job-seeker) experience is a **separate product** from the business suite. It is primarily a **mobile-native app** (the same shape as Indeed's job-seeker app) with a **desktop companion that mirrors the mobile UI**. Getting alignment on that layer is the point of this document and the companion site.

**For context (the emerging business direction): a full enterprise ERP suite, heading to the Next prototype.** The business side is a full enterprise ERP suite for the trades, similar to a CRM but with new vetting-style functionality plus forecasting and gap analysis. The emerging direction is the **Next prototype** (`toolbelt-next.vercel.app`) as the business app **shell and chrome**. We integrate the *qualified* items from our older PRDs, and the specific UI, micro-interactions, and page layouts we need **from Figma, into the Next shell** (not the Figma shell), plus the new features the team likes. The current tb v3 business suite in `prototype-liart-seven.vercel.app` is the earlier proposal and a reference for those qualified items, not the destination.

So: this PRD documents the whole two-experiences model, but the decision it seeks is **alignment on the individual layer**. The business direction is settled and described here so the two halves connect cleanly.

---

## 1. The proposal in one line

Two purpose-built ToolBelt products for two audiences with entirely different needs, kept separate, meeting at a shared Marketplace: a social, Indeed-style individual experience (mobile-native app + desktop companion) that acquires users, and an enterprise ERP business suite (the Next prototype) that posts and fills work.

---

## 2. Why now

- The business and product teams are converging on the Next prototype as the emerging business direction. The plan is to bring the qualified requirements and the right Figma UI into that shell.
- The Marketplace MVP work surfaced the growth engine (a connections and network layer) that lives on the individual side (see `Marketplace_MVP_PRD_Change_Proposal.md`).
- The individual experience is the piece still needing sign-off: is it a standalone mobile-native app (plus desktop companion), separate from the business suite? This proposal argues yes, and backs it with the proven Indeed model.

---

## 3. The experience model, and the proof (Indeed)

Individuals and businesses want completely different things. The proven pattern for this exact two-sided labor market is **Indeed**, and we are proposing the same model:

- **Indeed runs two separate products.** A job-seeker experience (search + apply) and a separate **Employer Dashboard** (post jobs, filter applicants, message, schedule, track, source). They are connected by search, matching, and recommendations, not merged into one app. [Indeed matching + hiring platform](https://www.indeed.com/hire/c/info/matching-and-hiring-platform), [Employer Dashboard](https://www.indeed.com/hire/resources/howtohub/employer-dashboard-frequently-asked-questions)
- **The job-seeker side is mobile-native and mobile-forward.** Indeed ships native iOS and Android apps ([App Store](https://apps.apple.com/us/app/indeed-job-search/id309735670)); the Android app alone has 100M+ downloads. "Apply from your phone" is a first-class flow. [Indeed mobile app](https://www.indeed.com/career-advice/finding-a-job/how-to-use-the-indeed-app)
- **The market is mobile.** Around two-thirds of job applications are submitted on mobile devices, and ~95% of global users reach the internet via smartphone. [Mobile vs desktop in job search, Appcast](https://www.appcast.io/mobile-versus-desktop-trends-in-job-search/)

**Our model mirrors Indeed:** a separate consumer product (mobile-native + desktop companion) and a separate business product (the enterprise ERP suite, the Next prototype), meeting at a marketplace with matching in the middle. We are not inventing a structure; we are adopting the one that already works at scale for labor.

---

## 4. The individual experience — THE alignment ask

**Who:** Individual workers and small one-operator companies ("Chuck in a truck").
**What it is:** A standalone consumer product, **separate from the business suite**. Primarily a **mobile-native app (iOS + Android)**, with a **desktop companion web app that mirrors the exact mobile UI**. Same model as Indeed's job-seeker app + desktop site.
**Why it is the core:** This is the acquisition and retention engine. Its viral networking loops grow the supply side of the marketplace, which is what makes the marketplace valuable to businesses.

**Positioning:** the public-facing, free social layer of the ToolBelt network. It behaves like a social app for the trades: users connect, share their work, refer, and prompt others to join. That is what fuels the activation funnels and viral loops. In practice this is the overdue upgrade to the mobile experience job-seekers are already forced into, modernized, with the features that fit where ToolBelt is going and a companion desktop app that mirrors it. The business suite sits behind a gated account upgrade (talk to sales, or self-serve when available), introduced with a pricing model and ToolBelt Pro; users upgrade into the business app when they need it.

**Design reference:** the recent Figma designs for the individual experience (the Indeed-style recommendations home, apply, notifications, applied/withdraw) plus the deliberate mobile-forward push. These become the native app UI; the desktop companion mirrors them.

**Requirements**

- **Discover and apply.** Recommended-work home (split-view on desktop, single-column on mobile), one-tap review-and-send apply (a review of the saved profile, not a re-entry form), tracking, revocable withdraw. (Prototyped; see `Phase_C_Indeed_Individual_Brief.md`.)
- **Public and social layer (the growth engine).** Free and public-facing, like a social app for the trades: connect, share work, refer, and invite others onto the ToolBelt network. This is what drives the activation funnels and viral loops, and the primary activation funnel with clear routes into the business suite lives here.
- **Networking and viral loops.** Worker profile ("available for work"), find and connect with workers/crews/orgs, request-and-accept connections, direct messages only after both accept, block and report. Two inboxes: application messages in Roster, connection messages separate. (From `Marketplace_MVP_PRD_Change_Proposal.md`.)
- **Contact management (simplified).** A contact and roster-style layer for the individual, the same idea as the business Roster but pared down for a one-person "Chuck in a truck" operation.
- **Post jobs (capped).** Individuals can also post work from the public app, with a cap. Heavy posting is a signal of hiring at scale and a natural upgrade path into the business ERP suite.
- **Mobile-native builds.** iOS + Android on the mobile-forward UI; the desktop companion mirrors it.
- **Notifications, My Jobs, My Posts, Network.**

**Alternative approach (the former path).** Rather than a standalone product, we could minify the business app (the Next prototype, formerly the Hardie route) into a streamlined, simplified experience for the individual user. This is the path we came from. It trades a purpose-built consumer app for reuse of the business shell, and it stays a viable option if we need it. The recommendation here is the separate mobile-native product; this alternative is captured so the team can weigh both.

**Open decisions to align on:** individual as a standalone mobile-native app + desktop companion (this proposal's recommendation); connections in the launch MVP vs fast-follow; worker-profile in MVP; ratings (facts only at launch); profile privacy (opt-in); trust-and-safety moderation owner; who owns the profile/connection data.

---

## 5. The business experience — the enterprise ERP suite (Next prototype route, emerging)

**What it is:** A full **enterprise ERP suite** for the trades, similar to a CRM but with new vetting-style functionality plus forecasting and gap analysis. It is the private, paid counterpart to the public individual app, reached through a gated account upgrade (talk to sales, or self-serve when available), introduced with a pricing model and ToolBelt Pro.

**Direction (emerging):** The **Next prototype** (`toolbelt-next.vercel.app`) is the emerging business app **shell and chrome**. It brings an auto-matching engine (auto-pairs candidates to open posts), a geographic view of jobs and pros, and a matches pipeline.

**The integration plan (this is the actual work):**

- **Shell/chrome = the Next prototype.** The Portal's navigation, layout, and chrome are the container. We do NOT carry over the Figma business shell.
- **Integrate the qualified items from our older PRDs into the Next shell.** Labor Requests (guided create + templates + request detail), Roster (CRM-style vetting of contacts, qualifications, status, the hiring pipeline), Org + Members + Permissions (ABAC-style scoped access), Billing, Account. These are qualified requirements from `Reflection_Spec_LRM.md`, `Reflection_Spec_Roster.md`, `Reflection_Spec_Org_Admin.md`, `Reflection_Spec_Account.md`, `Reflection_Spec_Portal.md`, `Business_Ecosystem_Build_Brief.md`, `Marketplace_Roster_Integration_Summary.md`.
- **Pull the specific UI, micro-interactions, and page layouts we need from Figma into that shell.** Not the Figma shell, only the qualified surfaces and interactions (for example the request-detail sections, the ABAC matrix, the Roster contact record, the address model and its micro-interactions).
- **Add the new features the team likes** from the Next direction (auto-matching, map, matches pipeline).

**Posture:** Desktop-first for the deep admin work; responsive so a mobile user can log in and handle essentials (verified on the current suite: Member Detail, Request Detail, Roster, Portal reflow to usable mobile).

**Open items:** the concrete migration path (which qualified surfaces port first), and design ownership of the Figma-into-Next integration.

---

## 6. The Marketplace — the flywheel

The shared surface and the only meeting point. Its own app at its own address, not hosted in the Portal; upgraded business accounts get a shortcut to it.

**The two-sided loop:** the individual experience acquires users via viral networking loops (supply); the business Portal posts labor requests (demand); workers discover and apply; applications route into the Roster; more users attract more businesses and more jobs attract more users. Matching connects the sides, the same mechanism Indeed uses.

**Requirements:** shared post/discovery model, application routing into Roster, saved jobs and saved-search alerts (in-app at launch), and the connections layer as the growth mechanism.

---

## 7. Delta vs the existing PRDs and briefs

| Area | Existing | This proposal |
|---|---|---|
| App model | Implicitly one suite + a marketplace | Two separate products + shared marketplace, made explicit (the Indeed model) |
| Individual | Profile/connections were "later" | Standalone mobile-native app + desktop companion; the alignment ask; connections proposed for MVP |
| Business | tb v3 business suite as the target | Enterprise ERP suite; the Next prototype is the shell; qualified PRD items + needed Figma UI integrate INTO it; not the Figma shell |
| Marketplace | MVP scope, connections TBD | Two-sided flywheel with connections as the engine; matching-driven like Indeed |
| Platform | Web-first | Individual mobile-native + desktop companion; business desktop-first + responsive |

Reconciled inputs: `Marketplace_MVP_PRD_Change_Proposal.md`, `Business_Ecosystem_Build_Brief.md`, `Individual_Experience_IA_Brief.md`, the `Reflection_Spec_*` set, `Prototype_Integration_Plan.md`.

---

## 8. Pricing and packaging (proposal)

**Model: plan tiers plus a credit economy. No seat pricing.** Seats are unlimited on every paid tier; we charge for marketplace demand and outcomes, not logins. This anticipates AI agents doing more of the per-seat work, and it matches how the two-sided comparables actually monetize (Indeed sponsorship budgets, Thumbtack lead spend, LinkedIn and Upwork credits).

- **Individual: free, public, capped posting.** 2 active posts, 5 per month. The cap is the upgrade trigger: posting past it means hiring at scale. Individuals can buy small visibility boosts, but money never raises the cap.
- **ToolBelt Pro (business): tiered plans bundling monthly credits.** Credits are spent on marketplace actions: job posts, boosts (promoted placement), and match unlocks. Top-up packs are available on every tier; rollover is generous and expiry is loud, never silent; a published, USD-denominated rate card keeps spend transparent. The exact credit definition and rate card are being finalized in the dedicated pricing engagement.
- **Three tiers.** Two self-serve tiers with trial (entry and growth, the growth tier adding forecasting and gap analysis), then Enterprise through sales with committed credit volume plus API, SSO, and integrations. Sales-assisted only at Enterprise.
- **No pay-to-win (binding).** Credits buy visibility and volume, never verdicts: boosts never override match-quality scores, vetting status, or ratings, and unlocks auto-refund when a worker never responds. Marketplace quality is the asset the pricing must protect.

Anchor dollar amounts, the rate card, and tier names live in the internal pricing docs (`ToolBelt_Pricing_Plan.md` plus the dedicated Toolbelt Pricing Strategy engagement, which owns the verified research and the packaging PRD) and stay off public artifacts until validated with the business team. The vision site carries a qualitative teaser only.

---

## 9. Infrastructure implications

- **Two products, two codebases.** Individual (mobile-native iOS/Android + desktop companion web) and business (the enterprise ERP suite, the Next prototype). Production splits them; the current prototype only co-hosts them behind a persona switch for demo.
- **Native app builds** for the individual experience, on the mobile-forward UI. New pipeline, app-store presence, push.
- **Business builds on the Next codebase/shell**, with qualified surfaces and Figma-sourced UI ported in.
- **Shared marketplace backend.** Posts, applications, connections, messaging, profiles, matching, Roster. Single owner and data model required.
- **One design system** (tb v3 tokens, Geist) applied across both products and the Next shell so the brand stays coherent.
- **Trust and safety.** Connections/messaging brings a moderation queue and block/report; needs an operational owner.

---

## 10. Phasing (proposed, to size with Eng)

- **Phase 1 — Marketplace + individual core.** Discovery, apply, track/withdraw, saved jobs/searches; business posts into it. (Largely prototyped.)
- **Phase 2 — Connections/network (the growth engine).** Worker profile, connections, DMs, block/report. The viral loop turns on.
- **Phase 3 — Native individual apps.** Ship iOS/Android on the mobile-forward UI; desktop companion mirrors.
- **Phase 4 — Business on the Next prototype.** Stand up the Next shell, port the qualified PRD surfaces + Figma UI, add auto-matching / map / matches.

Phases 1–2 build the flywheel; 3 scales the consumer side; 4 delivers the business direction.

---

## 11. Risks and the driving question

- **The separation must hold.** If the individual and business bleed into one app, both degrade and the flywheel gets muddy. Guard it in the architecture.
- **Native build capacity and timeline** for the individual apps.
- **Figma-into-Next integration** needs clear design ownership so qualified surfaces port faithfully without recreating the Figma shell.
- **Connections roughly doubles Marketplace scope** and reintroduces trust-and-safety work; worth it for the growth bet.
- **Shared backend + profile/connection data ownership.** Product + Engineering.

**The question that drives the rest:** Do we align on the individual experience as a standalone, mobile-native product (plus desktop companion), separate from the enterprise ERP business suite, meeting at one marketplace, with connections as the launch growth engine? The business direction (the Next prototype) is the emerging path; this is the call we need.

---

*Companion artifacts: the vision landing page, the three FigJam boards (Journey Maps, User Flows, Platform Map with the Venn/flywheel), the individual + reference-business prototype (`prototype-liart-seven.vercel.app`), and the Next business Portal prototype (`toolbelt-next.vercel.app`).*

*Sources for the Indeed model: [Matching + hiring platform](https://www.indeed.com/hire/c/info/matching-and-hiring-platform) · [Employer Dashboard](https://www.indeed.com/hire/resources/howtohub/employer-dashboard-frequently-asked-questions) · [Indeed mobile app](https://www.indeed.com/career-advice/finding-a-job/how-to-use-the-indeed-app) · [App Store listing](https://apps.apple.com/us/app/indeed-job-search/id309735670) · [Mobile vs desktop job-search trends, Appcast](https://www.appcast.io/mobile-versus-desktop-trends-in-job-search/)*
