# SideBench — Privacy Policy
**Effective date:** August 17, 2025

> **TL;DR**
> - **No data leaves your browser.**
> - **We don’t collect, store, sell, or share personal data.**
> - **No analytics, no ads, no trackers, no external servers.**
> - Works **100% offline** with **no external dependencies/CDNs**.

---

## Table of Contents
- [What this covers](#what-this-covers)
- [Data we collect](#data-we-collect)
- [How processing works (local only)](#how-processing-works-local-only)
- [Storage on your device](#storage-on-your-device)
  - [Clear local data](#clear-local-data)
- [Permissions (and why)](#permissions-and-why)
- [Network activity](#network-activity)
- [Third-party services](#third-party-services)
- [Children’s privacy](#childrens-privacy)
- [Changes to this policy](#changes-to-this-policy)
- [Contact](#contact)

---

## What this covers
This policy applies to the **SideBench** Chrome extension and its built-in tools: Base64/Base64URL & URL encode/decode, hash & HMAC (incl. file hashing), cron helper, regex tester, UUID v4/v7, QR generator, color picker, JSON formatter, time/epoch converter, randomizer, and similar utilities added in future updates.

---

## Data we collect
**None.**  
SideBench does not collect, transmit, sell, or share any personal information or content. We do not use analytics or crash reporting.

---

## How processing works (local only)
- All operations run **inside your browser** using web platform APIs (e.g., Web Crypto).
- When you open a file (for hashing/Base64/etc.), it is read **in memory** and **not uploaded** anywhere.
- Outputs (hashes, HMACs, encodings, UUIDs, QR codes, etc.) are generated locally.

---

## Storage on your device
SideBench may store **non-content preferences** (e.g., theme, default tool order, expanded/collapsed state) in `chrome.storage.local`.

> We **do not** store the text or files you process with the tools.

### Clear local data
- Remove the extension, or  
- Visit `chrome://extensions` → SideBench → *Clear data* (if available), or remove & reinstall.

---

## Permissions (and why)
SideBench is designed with least-privilege access.

- **`sidePanel`** — Provides the toolbox UI in Chrome’s side panel.
- **`scripting`** *(optional feature)* — Used **only after a user action** (e.g., toolbar/context-menu click) to read the current page **selection** and prefill a tool or highlight it. Runs locally; no data leaves your device.
- **`activeTab`** — Grants **temporary**, user-initiated access to the current tab so a one-off script can run **without** broad site access. Ends when the tab navigates.
- **`host_permissions`** *(optional at runtime)* — **Not required by default.** If you opt in to deeper per-site integration, SideBench requests origin-scoped access with your consent. Even then, SideBench does **not** transmit data.

We do **not** read your browsing history, track pages you visit, or auto-run on sites without your explicit action or consent.

---

## Network activity
- SideBench performs **no network requests** during normal use.
- No analytics, no third-party calls, no telemetry.
- All libraries used by the tools are **bundled** and run locally.

---

## Third-party services
None. Any vendor code (e.g., a QR encoder) ships with the extension and does not contact external services.

---

## Children’s privacy
SideBench does not target children and does not collect personal information.

---

## Changes to this policy
If we make material changes, we’ll update the **Effective date** above and publish the new policy at the same location where this document is hosted.

---

## Contact
Questions about privacy? Reach us at **[dev@sidebench.cc]**.
