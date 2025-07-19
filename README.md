# Web5 Purple Vibes – Privacy Policy

> **Status:** Prototype / Concept Extension  
> **Last Updated:** 2025-07-19  
> **Contact:** iknowyoullremember@gmail.com  
> **Applies To:** Chrome extension “Web5 Purple Vibes – LinkedIn Enhancer (Concept)”

**Not affiliated with, endorsed by, or officially connected to LinkedIn Corporation.**

---

## 1. Summary
We do **not** collect, transmit, sell, rent, analyze, monetize, or otherwise share any personal data. All processing (metrics, scoring heuristics, notes, visualizations) happens locally in your browser. Uninstalling (or using the purge function) removes stored data.

## 2. Data Stored *Locally Only*
| Category | Examples | Purpose | Scope |
|----------|----------|---------|-------|
| Notes | Your free‑form text (context or URL bound) | Personal memory / annotation | Stays on device |
| Preferences | Theme colors, feature toggles, update interval, targets list | Customize UI & behavior | Local storage |
| Lightweight Metrics | Post counts, scroll velocity, follower snapshot numbers, ephemeral scoring buffers | Real‑time panel metrics & visuals | Ephemeral / local |
| Version Flags | Last seen / onboarded version markers | One‑time info display, migration | Local storage |

## 3. Data *Not* Collected
- No account credentials or session tokens  
- No raw LinkedIn feed export or bulk duplication  
- No external analytics, telemetry, tracking pixels or fingerprinting  
- No third‑party advertising networks  

## 4. Network Activity
The extension itself makes **no external network requests** beyond the normal LinkedIn page traffic already initiated by your browser. All computations occur in the content script context.

## 5. Permissions & Justification
| Permission | Why It’s Needed |
|------------|-----------------|
| `storage`  | Persist local notes & user preferences |
| Host access: `https://www.linkedin.com/*` | Inject UI, read DOM to compute per‑page metrics and visual overlays |

No additional capabilities (clipboard, downloads, cookies, etc.) are requested in the prototype.

## 6. Notes & Scoring
- Notes: Plain text you explicitly enter.  
- Scoring / “resonance” metrics: Derived at runtime from visible content fragments (e.g., counts, novelty ratios).  
- These are not transmitted; only minimal numeric summaries are kept locally for sparkline history (capped length).

## 7. Data Retention & Deletion
- All stored objects reside in Chrome’s extension storage (`chrome.storage.local` / `sync` for prefs).  
- Use the in‑extension **Purge** (if provided) or uninstall the extension to remove data.  
- No remote backups exist; we cannot restore purged data.

## 8. Third Parties
No external frameworks fetch or process data. (UI relies solely on built‑in Web APIs; no remote scripts.)

## 9. Children’s Privacy
The prototype is not directed to children and does not knowingly store information about minors.

## 10. Security Considerations
- Runs with least privileges (only LinkedIn host + storage).  
- No dynamic code execution via `eval`.  
- User-entered note text is HTML‑escaped before display to mitigate XSS injection into injected panels.

## 11. Affiliation Disclaimer
“Web5 Purple Vibes” is an independent prototype and is **not affiliated with LinkedIn**. Logos or trademarks of LinkedIn are not used inside shipped assets.

## 12. Changes to This Policy
If the scope expands (e.g., optional export or semantic features), this document will be updated and the extension version number incremented. Because no server component exists, changes typically concern added local features or clarifications.

## 13. Contact
Questions, concerns, or deletion confirmation requests (though all data is local) can be sent to:  
**Email:** <iknowyoullremember@gmail.com>

---

*Version: 2025-07-19 · Prototype Phase*
