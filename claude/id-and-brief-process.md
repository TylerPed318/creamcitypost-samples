# Company IDs and creative briefs — standing process (from Tyler, Nov 11, 2026)

Follow this on every new sample (v1) and every revision. It sits on top of `claude/sample-log.md` and `claude/revision-lessons.md`.

## RULE: no brief, no sample (Tyler, Nov 11, 11:49 AM CT)
**Only build a sample if a "Creative brief — <ID> — <Business>" email exists for that business.** If there is no brief, don't build — skip the lead and move to the next one that has a brief. (This replaces the earlier "if there is no brief, build from the sheet and own site" fallback.) The lead-sheet "Top 10" order still sets priority among businesses that have briefs.

## Company IDs
- Every business has one permanent ID (CCP-001, CCP-002, …). Source of truth: the **"Trades leads with IDs — <date/batch>"** emails in Tyler's Gmail. Column 1 of each attached sheet is **Company ID** — the only ID allowed for that business. Backup lookup: "Cream City Post company ID master list" email (`cream-city-post-company-ids.csv`, 1,310 rows).
- Never invent, renumber or reuse an ID. Similar names → trust the ID column plus that row's phone and website (e.g. Frank Gillitzer Electric Co, Milwaukee ≠ Gillitzer Electric Services Inc, Menomonee Falls).
- If Tyler asks for a business that isn't in any "Trades leads with IDs" sheet: **stop and ask him for an ID.**

## Before building v1
1. Read the Company ID, business name and website from the leads sheet row.
2. Search Gmail for `subject:"Creative brief — <ID>"`. If several copies exist, use the newest. **None → stop; no sample.**
3. Read the whole brief before designing or writing anything.
4. Cross-check ID, business name and website between the sheet row and the brief. **If they disagree, stop and flag it to Tyler — don't build.**
5. Build from the brief, still using only facts from the business's own website (or facts the brief marks as verified from that site). No invented claims, review counts, years or job photos. Our revision lessons still apply (e.g. skip AI-looking photos even if the brief lists them, and say so).
6. Email `Sample ready — <ID> v1 — <Business>` with the public link.

## Revisions and approvals
- Same ID for every version. `Sample revision — <ID> v<n>` → rebuild as v<n+1> and send `Sample ready — <ID> v<n+1>`.
- `Sample approved — <ID> v<n>` → final; don't rebuild unless Tyler asks.

## Status of briefs (checked Nov 11, ~11:45 AM CT)
- Briefs exist only for **CCP-011 Gregg Heating & Air Conditioning, CCP-012 Dnesco Electric Inc, CCP-013 Big Jim's Small Engine Service, CCP-014 TPC The Painting Company LLP, CCP-015 All City Mudjacking, CCP-016 Bartz's Floor Covering** (each sent twice; the 17:22 UTC copies are the newest). All six are from the "Trades leads with IDs — 2026-11-10" sheet.
- No briefs for any sample built before this rule (CCP-005–010, 017–021, 112, 114) or for the Batch 2 queue (CCP-115–120) — those are on hold until briefs arrive.
- Sheets downloaded locally: /home/claude/leads/ids-2026-10-15-first30.xlsx (CCP-022–051), ids-2026-10-20-b2.xlsx (CCP-021, 112–160), company-ids.csv (master).
