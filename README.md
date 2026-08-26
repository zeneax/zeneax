<h1 align="center">Zeneax Lab</h1>

<p align="center">
  <strong>A software studio.</strong><br>
  We build products that are considered in their design and rigorous in their engineering.
</p>

<p align="center">
  Founded by <a href="https://github.com/zeneax"><strong>Shahram Mazar</strong></a>
</p>

<p align="center">
  <a href="#what-we-do">What we do</a> ·
  <a href="#how-we-build">How we build</a> ·
  <a href="#work">Work</a> ·
  <a href="#contact">Contact</a>
</p>

---

## What we do

Zeneax Lab designs and builds software end to end — from working out what a product
actually needs to be, through interface design, to the engineering that makes it
dependable in daily use.

We take on work where the details matter. Most software fails not because the idea
was wrong but because the last twenty percent was never finished: the edge case
nobody tested, the error message that explains nothing, the state that gets lost when
the network drops. That last twenty percent is the part we care about.

**Design and engineering are not separate stages here.** A product that looks
considered but behaves unpredictably is not finished, and neither is one that works
correctly but is unpleasant to use.

---

## How we build

### Start from the real problem

Before writing code, understand what is actually being asked for — which is often not
what was first described. The right solution is frequently simpler than the one
requested, and occasionally quite different.

### Build for the failure cases

Software is judged on how it behaves when something goes wrong. Networks drop,
devices disconnect, permissions get revoked, APIs change under you. We design for
those paths deliberately: work in progress is never silently lost, failures are
retried when a retry can plausibly succeed, and errors are written in language the
person reading them can act on.

### Native where native matters

Using the platform properly — its conventions, its APIs, its performance
characteristics — rather than wrapping a generic layer and calling it cross-platform.
Users can tell the difference even when they cannot name it.

### Make the judgement calls configurable

Every decision that seemed obvious at design time turns out, eventually, to need
changing. Providers, models, thresholds, behaviour — these belong in configuration,
not compiled into assumptions.

### Document the reasoning

Code that looks wrong but is deliberately working around a platform behaviour is
worse than useless without the reason attached. We write down *why*, not just *what*.

---

## Work

### [FarsiTalkWrite](https://github.com/zeneax/Farsi-Talk-Write)

A macOS voice dictation utility. Press a key, speak, and the transcribed text is
inserted at the cursor in whatever application is in front — a browser, an editor, a
messaging app.

Built natively in Swift with no external dependencies. The interesting engineering is
in the parts users never see: Bluetooth audio devices that renegotiate their sample
rate mid-recording, system permissions bound to code signatures, complex text layout,
and a pipeline designed so that a failed network request never costs the user what
they just said.

`Swift` · `AppKit` · `CoreAudio` · Open source, GPL-3.0

### Shoppex

A complete e-commerce platform — not a storefront bolted onto a payment provider,
but the operational system a retail business actually runs on.

Most e-commerce products stop at the checkout and leave the operator to assemble
inventory, support and analytics from four other services. Shoppex was built the
other way round: the parts a business touches every day belong in one system, sharing
one source of truth.

**Commerce and inventory.** Full inventory management alongside the storefront —
stock, catalogue and fulfilment as one model rather than a shop with a spreadsheet
attached.

**CRM and customer communication.** Customer relationships are managed inside the
platform, including end-to-end messaging with customers. Conversations stay attached
to the customer record instead of being scattered across personal inboxes and phones.
Telegram and WhatsApp integrations exist for reach, though in practice the built-in
communication panel removes most of the need for them.

**Seller panel.** A dedicated surface for sellers to run their own catalogue, orders
and customers, separate from platform administration.

**Developer panel.** The part that makes the system operable rather than merely
functional: database tables can be inspected and queried directly from the panel,
backups are managed as a first-class process, and an error dashboard surfaces
failures where the operator can see them.

That last piece is the design argument for the whole product. Most platforms push
operators to a database client, a separate backup service and a third-party error
tracker — three tools, three logins, three places to look when something breaks.
Building them in means the person responsible for the system can actually diagnose it.

**Built solo.** Architecture, database design, interface and implementation — the
whole system, from the storefront through to the operational tooling behind it.

**Search.** Built on PostgreSQL with purpose-built indexing rather than a bolted-on
search service. Catalogue search is the feature customers judge a shop by — slow or
imprecise results cost sales directly — so it was treated as a first-class engineering
problem across every kind of query the platform serves.

`Next.js` · `TypeScript` · `PostgreSQL` · Solo build · Private

### DepoMotors

An inventory and ordering platform for automotive parts retail, built on the same
architecture as Shoppex and applied to a domain with its own demands.

The platform capabilities carry across — full inventory management, CRM with
in-platform customer messaging, and separate seller and developer panels, including
the same direct database inspection, managed backups and error dashboard. What
changes is the catalogue itself: parts retail lives or dies on whether a customer can
find the exact component that fits their vehicle, which makes precise, fast search
against a large and highly structured catalogue the central problem rather than a
supporting feature.

Built solo, end to end.

`Next.js` · `TypeScript` · `PostgreSQL` · Solo build · Private

<!--
  Further private / client work goes here, same shape.
  Check any confidentiality agreement before naming a client publicly.
-->

---

## Contact

<!-- Fill these in — a placeholder is better than a dead link. -->

- **GitHub** — [@zeneax](https://github.com/zeneax)
- **Email** — _add your contact address_
- **Web** — _add your site if you have one_

---

<p align="center">
  <sub><strong>Zeneax Lab</strong> · Founded by Shahram Mazar</sub>
</p>
