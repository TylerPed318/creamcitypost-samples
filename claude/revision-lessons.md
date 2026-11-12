# Cream City Post — lessons from revision requests (read before every new sample)

Kept by Claude. Every "Sample revision" email gets distilled into rules here so the next sample doesn't need the same fix. **Step zero for every v1: follow `claude/id-and-brief-process.md`** (Company ID from the "Trades leads with IDs" sheet, then find and read the "Creative brief — <ID> — <Business>" email). Then run the pre-send checklist at the bottom before the Sample ready email.

## Where these came from

| Revision | What was asked | Root cause |
|---|---|---|
| CCP-007 v1 → v2, Urban Loggers (Design Review) | Add the 4.9★ (30+ reviews) rating and a 2nd review; 2–3 more real gallery photos; compress the 132 KB logo; add a favicon | v1 was **thinner** than their already-modern site: fewer photos, less social proof. Heavy logo, no favicon. |
| CCP-009 v1 → v2, Pinky's (Design Review) | Remove "24/7" and show the posted hours; use the real key logo and favicon instead of a script wordmark; 2 more job photos | v1 turned one "24 hours for emergency lockouts" line into a blanket 24/7 claim that contradicts their hours table; a redrawn wordmark; too few photos. |
| CCP-008 v1 → v2, Big Dog (**Tyler, from his iPhone**) | "I love the slider idea, let's do more of this," but both slider photos are blurry; spend a few more Higgsfield credits to sharpen them | Low-resolution source photos shown large without enhancement. **Tyler likes interactive pieces (before/after slider).** |
| CCP-007 v2 → v3, Urban Loggers (Design Review) | Replace the gallery photo showing **another company's branded truck** with their real sawmill photo, cropped so a background trailer's lettering isn't legible | I didn't **read the text inside the photo**. The prospect's own gallery contained a competitor's truck. |
| CCP-009 v2 → v3, Pinky's (Design Review) | Upscale the key-cutter photo: 545px file shown at 483px CSS (1.13×), soft on desktop and phones | **Sharpness is now a revision trigger.** The largest photo on the page failed the 1.5× / retina math. |
| CCP-010 v1 → v2, Wisconsin Wood Flooring (Design Review) | Replace all 3 photos with the official 4K gallery originals; add "Bona Certified Craftsmen" from their About page | I used the 720–768px gallery thumbnails/slideshow captures when **4160px originals existed** on the same Wix gallery. I also missed a trust line on their About page. |
| CCP-008 v2 → v3, Big Dog (Design Review) | Recrop the front-yard "before" photo: a strip of the collage's tan mat/logo frame was still visible at the top-right | Cropping cells out of a 2×2 collage left a few pixels of frame. **Check every crop edge.** |
| (self-caught) CCP-018 Hernia Movers, before sending | — | The Higgsfield 4K upscale **garbled small painted lettering** on their truck ("Busirers", "Coneral Delivery", a misspelled web address). Fixed by blending the original photo's pixels back over the lettered areas. |
| (self-caught) CCP-020 Sparks Electric, before sending | — | I put ★★★★★ on review cards, but their site shows testimonials with **no star ratings**. Stars imply a rating they never published. Replaced with quote marks. |
| CCP-020 v1 → v2, Sparks Electric (Design Review) | Remove the four dollar coupons ($25 off, $149 consult, etc.). Replace with "Specials & discounts / Ask about current specials when you call." | The coupons came from a **2011 "limited time" graphic** with no expiry. Publishing stale prices in a first-touch intro is a risk: a prospect could quote an offer that no longer applies. |
| CCP-021 v1 → v2, Wood Floors Unlimited (Design Review) | (1) Drop the NBA patent lead: their History page credits **GJ Baseman**, not the company, and "60 years" conflicts with it. (2) **Shorten to a teaser**: cut the stain sampler, pet band and commercial block to single lines; keep hero, one interactive, a 3-photo row, 1–2 reviews and the closer. Drop the NWFA/NARI badges (logo files only, not confirmed in copy). | I led with the flashiest homepage claim without checking the History page, and I stacked too many sections. **Page length is now an explicit revise trigger: "Tyler prefers a short teaser."** |
| Review bot ID notes + Tyler's ID instructions (Nov 11) | Hernia re-IDed CCP-012 → CCP-018; Sparks CCP-014 → CCP-020; Sunset Septic is CCP-112 (not 022). Tyler: use only the Company ID column of the "Trades leads with IDs" sheets, and read the creative brief before building. | I was numbering samples myself. **Every business already has a permanent ID; look it up, never assign one.** |

Approved as final so far: CCP-005 v3, CCP-007 v3, CCP-008 v3, CCP-009 v3, CCP-018 v1 (Hernia Movers).

## Rules (apply to every sample)

### Shape: a short teaser (most important — Nov 11)
0. **Keep it to about 5 blocks:** header with logo + tap-to-call → hero (headline + one framed real photo) → slim proof strip (3–4 items) → **one** interactive built from real data → a 3-photo row → 1–2 short reviews + contact/closer card → "first look" closer and footer. Fold everything else (extra services, pets, commercial, do's/don'ts, badges) into **one line of copy** inside those blocks. Never two interactives. If a section doesn't earn its place in a 30-second scroll, cut it.

### Facts and claims
1. **Hours and availability must match their posted schedule exactly.** Never write "24/7", "24 hours" or "always open" unless their hours table says so. If they word it with a caveat (e.g. "*24/7 emergency rates may be higher"), keep their wording and caveat.
2. Every number or claim (years, %, ratings, review counts, response times, licenses, certifications, "family owned") must be quoted from their own site (or marked in the creative brief as verified from that site). Lead spreadsheets and directories are not sources.
3. **Read their About AND History pages too**, not just the homepage. Certifications and trust lines (e.g. "Bona Certified Craftsmen") often live there. **Homepage claims can be looser than the History page** — when they conflict, follow the History page, and never credit a founder's, parent's or predecessor's achievement (patents, awards) to the current company. Don't lead with a high-risk claim.
4. Reviews: short excerpts from reviews published on their own site, credited the way they credit them. **No star icons unless their site publishes a star rating** for that review or overall.
5. Captions describe only what the photo visibly shows. Use neutral labels ("From our gallery") when unsure.
6. **No dollar amounts or coupon terms from old specials pages.** If a specials page exists, use: "Specials & discounts / Ask about current specials when you call. / Offers change, so we don't list dollar amounts here. Mention this note and we'll tell you what's current." plus a tap-to-call button.
7. Membership/association badges (NWFA, NARI, BBB, etc.) only when the site's **copy** states the membership — a logo file in the media library isn't enough.
8. Skip placeholder content on their site (e.g. template team names like "John Smith, Position/Title").

### Photos: get the best original, then inspect it
9. **Always find the original full-resolution file**, never a thumbnail, slideshow screenshot or CSS-sized render.
   - Wix: `static.wixstatic.com/media/<id>~mv2.jpg` with no `/v1/fill/...` suffix returns the original (often 4000px+).
   - Squarespace: `images.squarespace-cdn.com/...` with `?format=2500w`.
   - GoDaddy: `img1.wsimg.com/isteam/ip/<site>/<file>` without the `/:/rs=...` suffix. Note: `isteam/stock/...` files are GoDaddy **stock** — never use them.
   - WordPress: the `wp-content/uploads/...` file without the `-1024x683` or `-scaled` suffix (e.g. `IMG_1036-scaled.jpeg` → `IMG_1036.jpeg` is 4032px).
   - Hostinger/others: the `storage.googleapis.com/...` source URL.
10. **Sharpness math (Design Review's standard):**
   - The image's real width must be **≥ 1.5× its CSS display width on desktop** and **≥ ~3× its CSS width on a 390px phone** (DPR 3).
   - In practice: hero/feature images ≥ ~1800px on the long side (≥1400 acceptable for a framed ~560px card); half-width or pair images ≥ ~1600px; a ~480px CSS card ≥ 1200px. Small originals (≤600px) only as small tiles (≤240px CSS, 2-up on phones).
   - If the best original is smaller than that, upscale it with Higgsfield (2 credits; keep the same crop and scene) or show it smaller.
11. **After any upscale, zoom in on all text in the photo** (truck lettering, signs, logos, phone numbers). Upscalers invent wrong letters in small text. If text is garbled, blend the original's (softer but correct) pixels back over just those areas, or crop the text out. Never ship AI-invented lettering on a prospect's brand.
12. **Read any lettering in the photo.** If it names another company, don't use it or crop it unreadable.
13. Skip photos that look stock, CGI, composited or AI-generated, even on the prospect's own site (WWF's stock CGI hero; Urban Loggers' AI-looking milling.jpg; Hernia Movers' room/box shots; all of A Pest 2 Go's GoDaddy stock; Sparks Electric's stock-model/composite-van banner; Wood Floors Unlimited's Unsplash/Pixabay images; P's Junk team/truck renders).
14. **If a company has no real job photos at all** (A Pest 2 Go, Sparks Electric), build a photo-free design around their logo, real data (hours, services, service areas) and an interactive element. Say so in the Sample ready email and suggest getting their photos for the full build. Don't fill the gap with stock or generated "job" photos.
15. **Cropping collages:** crop well inside each cell and check all four edges at full size for any flat mat/border strip. After cropping, check for black fill (crop box past the image edge).
16. Use 3 real job photos in the teaser's photo row when they have them.
17. **Don't invent before/after pairs.** Only build a slider when the site has a matching before AND after of the same job.
18. Skip family/kid photos and photos of work that may be a partner's (e.g. remodel shots), even if they're on the site.

### Brand
19. **Use their real logo file**, never a redrawn or typed wordmark. If the logo is part of a wide banner, crop to the wordmark. White-text logos go on a dark brand-colored header.
20. **Always ship a favicon** made from their logo or site icon. Crop to the icon element (e.g. the ant, the water drop, the sun) so it reads at 16px; an inline SVG of their brand symbol (e.g. a lightning bolt in their colors) is fine when the logo has no clean icon.
21. Keep asset weight down: logo ≤ ~20–25 KB (PIL `quantize(colors=128, method=FASTOCTREE)` keeps RGBA logos clean at ~10 KB), photos ~100–300 KB each (JPEG q≈72–80), the whole page well under 1 MB.

### Content depth
22. Still never thinner than their current site on **proof**: bring the best social proof they publish (Google rating with review count if shown, 1–2 short reviews, one trust line). But depth comes from quality, not section count (see rule 0).
23. If their site is already modern, the sample must be a **clear upgrade**: more polish and personality. Lean into whatever is distinctive about them (e.g. Hernia's "Potentate of Totin' Freight" since 1975).
24. Lead sheets go stale. Check the live site before building: Hernia Movers had been fully rebuilt since the lead was logged. Note it in the email.

### Design (Tyler's taste)
25. Don't mirror their current hero (same lead photo full-screen with text over it).
26. **Tyler likes interactive touches, like the before/after slider on Big Dog — "do more of this."** Use exactly one: a drag slider where real before/after pairs exist; otherwise a small interactive built from real data (live "Open now" hours card, move-type picker, "pick the problem" service picker, flip-a-breaker panel, 3-year pump-due checker, dust-containment switch, text-a-quote builder).
27. Mobile: photo rows stack or scroll at ≤560px; nothing overflows at 390px; sliders and tabs work with touch.
28. **Do the overflow/screenshot check on the live URL in the Higgsfield sandbox**, not locally: the local workspace can't load Google Fonts, so fallback fonts give false overflow results. Use `minmax(0,1fr)` grid columns so long words can't push a column wider than the screen.

### Higgsfield budget
29. Default: at most 2 credits per sample (one 4K upscale on the main/largest photo), and only if the best original fails the sharpness math.
30. Tyler or Design Review may approve more for a specific revision ("Use Higgsfield: yes …"). Follow exactly what the email allows.

### IDs and briefs
31. **Never assign an ID.** Take it from column 1 ("Company ID") of the business's row in the "Trades leads with IDs" sheet (backup: the master ID list CSV). Similar names → trust that row's phone and website. Business not in any sheet → ask Tyler for an ID.
32. **Before v1, search Gmail for `Creative brief — <ID>`** and read it fully. Cross-check ID, name and website against the sheet; if they disagree, stop and flag it to Tyler. Build from the brief (own-site facts only). If no brief exists, say so in the Sample ready email: "No creative brief found for this ID; built from the lead sheet and the business's own site only."

## Fast photo pipeline (Claude, Nov 11)
- Claude's own workspace can't reach most image hosts, but the **Higgsfield sandbox** (`sandbox_exec`) has full internet, PIL, and headless Chromium via Node Playwright (`require` from `$(npm root -g)/noop.js`; use `waitUntil:'load'` plus a short wait, not `networkidle`). There: curl originals and upscale results, render JS-heavy pages (galleries, hours widgets), crop/resize/compress with PIL, then return finished JPEG/PNG files via `image_paths` (≤512 KiB total per call). They land byte-for-byte in `/tmp/claude-tool-results/…/mcp-Higgsfield-blob-*` and can be copied straight into the repo.
- If `media_import_url` is refused (e.g. SiteGround returns HTML to bots), upload from the sandbox: `media_upload` → `curl -X PUT -H "Content-Type: image/jpeg" -H "If-None-Match: *" --data-binary @file '<upload_url>'` → `media_confirm` → `upscale_image`.
- Use Tyler's Chrome only when he's at his computer (not available from the mobile app).

## Build lessons (scheduled run, Nov 11 PM)
- Manufacturer promo banners (e.g., Bartz's 2000×680) often have text and buttons baked into one side. Crop to the clean side before using one as a hero.
- Shop-sign photos usually show extra phone numbers or mascots. Crop to the part you can publish (bay, logo half) instead of editing pixels.
- Fetching the Higgsfield sandbox isn't needed now: the session network reaches image hosts directly (Wagtail cms_images, GoDaddy wsimg, lh3.googleusercontent `=s0`, graph.facebook.com profile pictures). Local Playwright is enough for the screenshot pass.

## Pre-send checklist (tick every item before emailing Sample ready)
- [ ] **ID taken from the "Trades leads with IDs" sheet; creative brief searched, read and cross-checked** (or "no brief found" stated in the email)
- [ ] **Teaser shape: ~5 blocks, one interactive, 3-photo row, 1–2 reviews, closer** — nothing else
- [ ] Hours match their posted hours table (or no hours/availability claims at all)
- [ ] Every number/claim found verbatim on their site (homepage, About AND History); nothing credited to a predecessor; no stale dollar offers; no unconfirmed badges; no stars unless they publish ratings
- [ ] Every photo is the **original full-res file**, passes the sharpness math, and is inspected at full size: no other company's name legible, no stock/CGI/AI look, no collage frame or black fill on any edge, **no garbled lettering after upscaling**
- [ ] Their real logo (not redrawn), ≤ ~25 KB, plus a favicon
- [ ] Real job photos used (or a deliberate photo-free design, flagged in the email)
- [ ] Clear upgrade over their current site; hero composition differs from theirs
- [ ] Live-URL check in the sandbox at 1440 and 390 (real fonts), no overflow; page and all images return 200

- **Nov 11, CCP-023 v2 / CCP-024 v2 (review copy):** Never quote a named Google review unless you've copied it word for word from the live listing during the build. Directory snapshots and aggregates don't count. If the live listing can't be opened, show only a stable rating line ("4.9 on Google"), with no review count and no date, plus a link to the listing. Review themes ("Fair pricing") are fine as long as they aren't attributed to anyone.
- **Nov 11, CCP-024 v2 (full-bleed hero):** A full-bleed hero renders at the full viewport width, so it needs about 2900px to stay sharp at 1920. Upscale at 4K and save at about 2900px, q70 (~450 KB). The ByteDance upscaler garbles small lettering on doors. Blend that strip back from a Lanczos-resized original with a feathered mask.
- **Nov 11, CCP-030/032/022 (scheduled run):** Brief photo lists can name the same photo twice under different file hashes (4EG: 5f49… = 3aab…). Montage the candidates once before choosing the photo row. Facebook-only briefs with Google review quotes still follow the live-listing rule: use review themes instead of named quotes unless the listing is opened during the build. Own-site testimonials (Canva/WordPress) can be quoted verbatim.
- **Nov 11, CCP-040 (scheduled run):** `git add -A` for a log commit also sweeps in a half-built sample's `img/` folder, so the images go live before the page. Stage only `claude/` on log commits (`git add claude/`).

- Nov 11, Tyler chat / CCP-055 v2: Use a draggable slider whenever presenting real before-and-after comparisons, rather than toggle buttons. Preserve keyboard/touch operation and original photo geometry; disclose different camera angles. This is Tyler's standing preference for future samples.
- **Nov 11, CCP-056 (scheduled run):** To hide readable certificates behind a person, don't blur hard rectangles (`-region` leaves blocky patches). Composite a blurred copy through a feathered mask (person polygon black, blur the mask ~18px), which reads as natural depth of field. Also: don't show five full stars beside a non-5.0 rating; use one star.

- Nov 11, Tyler chat / CCP-055 v3 and CCP-060 v2: Following verified facts is insufficient. Follow the brief's strongest visual direction, with a modern, company-specific composition and confident scale. AKL: make the real comparison the centerpiece, not a small card; upscale the real pair when needed. Whitlow: use the genuine team/key wall and history as distinctive visual material. Preserve original brand, short homepage scope and one interactive.
- **Nov 12, CCP-033 v2 / CCP-034 v2:** (1) Phone DPR-3 math applies to every lead photo. A 900px photo stacked full-width at 358px is only 0.84×. Make the hero typographic and move the photo into a small grid tile (2×2 on phones, about 167px). (2) On a thin or polarized Google listing (for example 3.9 from 7), don't show positive review themes, even true ones, because they overclaim. Use neutral "Find them on Facebook / Read the reviews on Google" links and let the services and process carry the page.

- Nov 12 (CCP-070 v1, scheduled run): a decorative `::after` on a card that is `position:sticky` on desktop escapes to the page when a media query sets it `position:static`, causing mobile overflow. Use `position:relative; top:auto` in the mobile override instead. Also: when upscaling a before/after pair, check the small lettering in BOTH frames; the tool sat in a different spot in each frame, so each needed its own blend-back box.
