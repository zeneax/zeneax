<h1 align="center">Shahram Mazar</h1>

<p align="center">
  I design and build software end to end — from working out what a product actually
  needs to be, through the interface, to the engineering that keeps it dependable in daily use.
</p>

<p align="center">
  <a href="https://mazarix.com"><strong>mazarix.com</strong></a> ·
  <a href="#work">Work</a> ·
  <a href="#how-i-build">How I build</a> ·
  <a href="#contact">Contact</a>
</p>

---

## Mazarix

[Mazarix](https://mazarix.com) is my studio: apps, automation and AI for businesses
that are losing hours to repetition — the same work done by hand because one system
never talked to the next. I listen to how the work is done today, map where it stalls,
build what removes the repetition, and hand it over in a form the business can run
without me. Where AI helps, I use it for what it does well — reading, sorting,
drafting, answering from a company's own documents — and I say plainly where it does
not. The studio's site is also its demo: a bilingual Persian and English site with an
assistant that answers from the studio's own material, a member area, and an owner
panel that runs the whole thing.

**Zeneax** is my lab — where the larger platform work lives before it has a name of its own.

---

## How I build

I start from the real problem, which is often not the one first described. I design
for the failure cases — dropped networks, revoked permissions, APIs that change
underneath — so work in progress is never silently lost and errors are written in
language the reader can act on. I use each platform natively rather than wrapping a
generic layer. Judgement calls — providers, models, thresholds — live in
configuration, not in assumptions. And I write down *why*, not just *what*.

---

## Work

### [Mazarix](https://mazarix.com)

The studio's own site and product. A bilingual marketing site, a member area, and an
owner panel driving an assistant that answers from the studio's documents; behind it,
a newsroom and blog pipeline, an error desk, a security desk, voice dictation, and a
meeting listener — all built and run solo.

`Next.js` · `TypeScript` · `Supabase` · `Postgres` · Solo build

### [FarsiTalkWrite](https://github.com/zeneax/Farsi-Talk-Write)

A macOS voice dictation utility. Press a key, speak, and the text lands at the cursor
in whatever application is in front. Native Swift, no dependencies; the interesting
engineering is in what users never see — Bluetooth devices that renegotiate sample
rate mid-recording, permissions bound to code signatures, and a pipeline where a
failed request never costs the user what they just said.

`Swift` · `AppKit` · `CoreAudio` · Open source, GPL-3.0

### Shoppex

A complete e-commerce platform — storefront, inventory, CRM with in-platform customer
messaging, a seller panel, and a developer panel with direct database inspection,
managed backups and an error dashboard. One system, one source of truth, built so
the person responsible for it can actually diagnose it. Catalogue search is built on
PostgreSQL with purpose-built indexing, because search is the feature a shop is
judged by.

`Next.js` · `TypeScript` · `PostgreSQL` · Solo build · Private

### DepoMotors

The same architecture applied to automotive parts retail, where the central problem
is precise, fast search against a large, highly structured catalogue — a customer has
to find the exact component that fits their vehicle.

`Next.js` · `TypeScript` · `PostgreSQL` · Solo build · Private

---

## Contact

- **Web** — [mazarix.com](https://mazarix.com)
- **GitHub** — [@zeneax](https://github.com/zeneax)

---

<p align="center">
  <sub>Shahram Mazar · Mazarix · Zeneax</sub>
</p>
