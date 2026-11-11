# Cream City Post — sample log (Claude)

**Rules live in `claude/sample-playbook.md`; read that first.** This file holds only status: the session handoff, the sample table and per-company notes.

**Source of truth for "already built / already handled":** the repo folders (TylerPed318/creamcitypost-samples) plus `Sample ready` / `Sample approved` emails in Gmail. This log can lag behind if a session dies. If the log disagrees with the repo or Gmail, trust those and fix the log. Re-read this file right before every write so you don't overwrite another session's lines.

## Session handoff (one line per session, newest at the bottom)
- Nov 11, ~12:10 PM CT: Playbook adopted. Brief rule in force.
- Nov 11, 12:20 PM CT: Audit. Log was stale: CCP-011/012/013 v1 had already been built and emailed (11:54–11:59 CT) by another session. Fixed below.
- Nov 11, 12:35 PM CT (interactive): done. CCP-114 v2 (0 credits), CCP-011 v2 (2 credits), CCP-014 v1 (4 credits) built and emailed. Next up for the 1:11 PM scheduled run: CCP-015 All City Mudjacking v1, then CCP-016 Bartz's Floor Covering v1. Tip: photo `img` tags need `height:auto` in CSS, or the width/height attributes stretch them.
- Nov 11, ~4:00 PM CT (interactive): The 3:00 PM scheduled run stopped because the Projects tool wasn't available. These docs now live in the repo under `claude/` and are read from the clone; `claude/scheduled-run-prompt.md` is the updated hourly prompt. Nothing built. Next up: CCP-015 All City Mudjacking v1, then CCP-016 Bartz's Floor Covering v1.
- Nov 11, ~4:50 PM CT (scheduled run, finished interactively): CCP-015 v1 done, live and emailed (2 credits). Tyler fixed the network policy and approved pushing straight to `main`; CLAUDE.md, the playbook and `scheduled-run-prompt.md` are updated. Next up: CCP-016 Bartz's Floor Covering v1, then CCP-023 A Service Beyond, CCP-024 Astro Auto Repair (oldest brief first).
- in progress — CCP-016 (Nov 11, 4:26 PM CT, scheduled run)

## Handled emails (don't reprocess)
CCP-005/007/008/009 revisions & approvals; CCP-018 approval; CCP-020 v1 revision (→v2) and v2 approval; CCP-021 v1 revision (→v2); CCP-112 v2 approval; CCP-012 v1 approval; CCP-011 v1 revision (→v2); CCP-114 v1 revision (→v2); CCP-011 v2 and CCP-114 v2 approvals (Nov 11).
Ignore the void early "Sample ready" emails that used wrong IDs (CCP-011 A Pest 2 Go, CCP-012 Hernia, CCP-013 Ingrilli, CCP-014 Sparks, CCP-015 Wood Floors Unlimited, CCP-022 Sunset Septic). The real IDs are in the table.

## Samples

| ID | Business | Trade / City | Source lead | Latest | Folder | Status |
|---|---|---|---|---|---|---|
| CCP-005 | Dale's Tree Service | Tree, Hartland | 10-20 #1 | v3 | dales/ | **Approved v3.** |
| CCP-006 | OnTime Handyman | Handyman, Sussex | 10-20 #2 | v1 | ontime-handyman/ | Awaiting review. |
| CCP-007 | Urban Loggers LLC | Tree, Pewaukee | 10-20 #3 | v3 | urban-loggers/ | **Approved v3.** |
| CCP-008 | Big Dog Landscaping | Landscaping, Waukesha | 10-20 #4 | v3 | big-dog-landscaping/ | **Approved v3.** |
| CCP-009 | Pinky's Locksmithing | Locksmith, Milwaukee | 10-20 #5 | v3 | pinkys-locksmithing/ | **Approved v3.** |
| CCP-010 | Wisconsin Wood Flooring | Flooring, Wauwatosa | 10-20 #6 | v2 | wisconsin-wood-flooring/ | Awaiting review. |
| CCP-011 | Gregg Heating & Air Conditioning | HVAC, New Berlin | brief | v2 | gregg-heating/ | **Approved v2.** |
| CCP-012 | Dnesco Electric Inc | Electrical, Milwaukee | brief | v1 | dnesco-electric/ | **Approved v1.** |
| CCP-013 | Big Jim's Small Engine Service | Small engine, Oconomowoc | brief | v1 | big-jims-small-engine/ | Awaiting review. |
| CCP-014 | TPC The Painting Company LLP | Painting, Muskego | brief | v1 | tpc-painting/ | v1 emailed Nov 11, 12:33 PM. 4 credits. |
| CCP-015 | All City Mudjacking | Mudjacking, Franklin | brief | v1 | all-city-mudjacking/ | v1 emailed Nov 11, ~4:50 PM. 2 credits. |
| CCP-016 | Bartz's Floor Covering | Flooring, Franklin | brief | — | — | Brief ready; not built. |
| CCP-017 | A Pest 2 Go | Pest control | 10-20 #7 | v1 | a-pest-2-go/ | Awaiting review. Photo-free. |
| CCP-018 | Hernia Movers Inc. | Movers, Milwaukee | 10-20 #8 | v1 | hernia-movers/ | **Approved v1.** |
| CCP-019 | Mike Ingrilli Plumbing | Plumbing, West Allis | 10-20 #9 | v1 | mike-ingrilli-plumbing/ | Awaiting review. |
| CCP-020 | SparksElectric.com LLC | Electrician, Milwaukee | 10-20 #10 | v2 | sparks-electric/ | **Approved v2.** |
| CCP-021 | Wood Floors Unlimited | Flooring, Nashotah | 10-20 B2 #1 | v2 | wood-floors-unlimited/ | Awaiting review. |
| CCP-112 | Sunset Septic Service | Septic, Waukesha | 10-20 B2 #2 | v2 | sunset-septic/ | **Approved v2.** |
| CCP-113 | Duffy's Professional Carpet Cleaning | Carpet, Milwaukee | 10-20 B2 #3 | — | — | **Skipped:** no website. |
| CCP-114 | P's Junk Removal & Demolition | Junk/demo, Milwaukee | 10-20 B2 #4 | v2 | ps-junk-removal/ | **Approved v2.** |

**On hold, no brief yet:** CCP-115 Friendly Junk, 116 Royal Chimney, 117 Sun Lake Cleaning, 118 Klink's Karpets, 119 A&L Appliance, 120 Duct Works. New briefs from Design Research get built in the order they arrive.

### Notes per company
- **CCP-005 Dale's:** 30+ years, free estimates, fully insured, residential & commercial; 550 North Avenue, Hartland; (262) 951-8635.
- **CCP-007 Urban Loggers:** use (414) 240-4626, not (414) 514-0750. Gallery-19 shows "A New Leaf Tree Service" truck; never use it.
- **CCP-009 Pinky's:** hours "Normal hours: Sun–Fri 9am–3pm. Emergency: Sun–Thu 24 hours, Fri 12am–3pm. Closed Saturday." Never say 24/7.
- **CCP-010 Wisconsin Wood Flooring:** since 1926, three generations, Bona Certified Craftsmen; 560 N. 108th Place, Wauwatosa; 414-882-0101.
- **CCP-011 Gregg:** hero van is a Higgsfield upscale of the official about-img.webp; the rear-door small lettering was blended back from the original (the upscaler garbled it).
- **CCP-015 All City Mudjacking:** founded 1984 only (never "29 years"); 7095 S. Ballpark Dr., Suite 320, Franklin, WI 53132 only (no West Allis); Mon–Sat 6:00am–6:00pm, Sun closed; 414-543-2400; no email. Portfolio photos carry a VisualLightBox.com watermark at the bottom; crop it. Their SSL chain is missing its intermediate, so fetch with the ZeroSSL intermediate added (don't disable verification).
- **CCP-014 TPC:** hero cropped to hide the yard sign's 262-751-6135 (don't print that number). Sunday hours on their site read "9:00AM–5:00AM"; omitted. Only phone: 262-818-0960. No email.
- **CCP-019 Mike Ingrilli Plumbing:** est. 2007; plumber since 1985, Master Plumber since 1989, third generation; Anya = Operations Manager; "We respond 24/7" is on their site. 237 S. Curtis Road, West Allis; 414-213-9617.
- **CCP-020 Sparks:** 414-536-8500; never publish the 2011 coupon amounts; "*24/7 emergency rates may be higher".
- **CCP-021 Wood Floors Unlimited:** never use the NBA patent line; BonaKemi's Atomic DCS; NWFA/NARI not confirmed; showroom Mon–Fri 9–4:30; (262) 367-8896.
- **CCP-112 Sunset Septic:** over 30 years; licensed, insured & bonded drivers; WI 3-year pump/inspect rule; (262) 968-9812; skip the About page's placeholder team names.
- **CCP-114 P's Junk:** owner Vanessa; 6001 W Capitol Dr, Milwaukee; 414-240-4332; contact@psjunkremovalwi.com; use only real job photos (IMG_2927, IMG_2894, IMG_2832, BE11FC62, 42B1A82A). No named review quotes; no exact review count; "5.0 on Google" only.
