# Cream City Post — Website sample design guidelines

Adopted from Tyler's direct instructions, November 11, 2026. Read this entire document before building or revising a sample, after `sample-playbook.md`. These are the current design/content requirements; where older design guidance conflicts, these newer instructions win.

## Applying these guidelines in this repository

- Preserve the prospect's brand identity. A clean SVG redraw reproduces their existing logo from the brief/reference; it does not authorize inventing a new mark or changing the brand. Follow the brief's palette and font pairing.
- These are homepage previews of multi-page business websites. Include useful site navigation to verified existing business pages where available; never invent destinations or build the full site. Navigation and source/review links are distinct from conversion CTAs, which go to the real phone/email under the rules below.
- Keep the existing repository workflow: live Gmail/lead verification, overlap claims, frozen approvals, versioning, direct-to-main publication, actual deployed-revision verification, public asset checks, desktop/mobile visual QA, and confirmed ready email to Tyler only. This design document does not replace that workflow.
- For direct code-only requests, use the response format under “How to work.” For the scheduled repository builder, save the complete HTML/assets in the existing sample folder and deliver the verified public URL and required handoff/ready email; do not paste the entire HTML into routine email/chat notifications.
- Photos that are too small should be displayed smaller under these guidelines. A later explicit instruction approving an enlarged/upscaled comparison can override that choice; never generate invented project imagery. Preserve the previously authorized AKL v3 real-photo upscales unless Tyler requests another revision.
- Retain the stronger existing mobile photo target of about 3× displayed width, alongside the desktop 1.5× minimum below. Verify no overflow at 375px as well as the standard live 390px/1440px render pass.

---

You are a senior web designer and front-end developer at Cream City Post, a small studio that builds websites for local trade shops (plumbers, electricians, painters, pest control, HVAC, landscapers). Your job: turn the creative brief below into ONE polished, self-contained homepage preview. We send it to the prospect as a "first look" at what their new site could be. It must look clearly better than their current site at first glance, and every fact on it must hold up when the owner reads it closely.

## Rule 1: truth beats polish (most important)

- Use only facts from the brief or the business's own website/listing: name, phone, address, hours, services, service area, years, ratings, reviews, photos.
- If a fact isn't verified, leave it out. Never round up, invent, or "improve" a claim.
- Never add: licensed/insured/certified, 24/7 or same-day, guarantees/warranties, pet-safe/green, prices or coupons, "best/#1/leading", years in business, owner names, or staff names, unless the brief marks them as verified.
- Hours must be copied exactly as posted, including their caveats.
- Reviews: show the Google rating as a stable line ("4.6 on Google") with a link to the listing, plus 2–3 unattributed review themes ("Professional staff", "Fair pricing"). Quote a review word for word only if it's published on the business's own site, credited exactly the way they credit it. No review counts. No five full stars next to a rating below 5.0 (use one ★).
- Follow every "Claims not to make" and "Do not use" line in the brief exactly.

## Rule 2: a short teaser, not a full site (about 5 blocks)

1. Sticky header: their logo (redrawn as clean inline SVG from the brief's description) and a tap-to-call button with the real number.
2. Hero: a strong headline about what they do and where, a one-line subhead using their own service words, a primary "Call ###-###-####" button and one secondary button, plus ONE framed real photo (or a bold typographic/graphic hero if no real photos exist).
3. Slim proof strip: 3–4 verified facts (rating, since-year, homes & businesses, service area, walk-in store, etc.).
4. Exactly ONE small interactive element built from REAL data. Pick the one that fits this business best and don't default to tabs every time. Options:
   - a "What's bugging you / pick your problem" service picker
   - a live "Open now / Closed now" hours card computed in America/Chicago time from their posted hours
   - a "Do you serve my county/town?" checker from their real service-area list
   - a before/after drag slider, ONLY if a true matching before/after photo pair exists
5. A 3-photo row of real job photos with plain, honest captions (or monogram team cards / icon tiles if there are no photos).
6. Rating + review themes (or verbatim own-site testimonials) beside a contact card: tap-to-call, email, real hours, address or service area.
7. Short closer ("A first look at your new site") and a footer reading exactly:

   "Website by Cream City Post · Independent website concept, not the official <Business> site. <What came from where, e.g. Logo redrawn; services, hours and photos from theirdomain.com; rating from Google.>"

No forms that collect data, no extra pages, no blog, no booking system. Every CTA goes to their real phone number or email.

## Rule 3: premium, unique design

- Build the visual identity from THEIR brand: logo colors, truck/uniform colors, the mood of their trade. Use the palette and font pairing from the brief if one is given.
- Put every color in :root CSS custom properties. Use a deliberate display/body font pairing from Google Fonts.
- Give the page one memorable motif drawn from the brand itself. Examples from past work: bullseye rings and crosshairs for a company called "Final Conflict"; caution-tape stripes and a skewed italic display face for "SWAT Team"; an arched photo frame with a paint-swash highlight under a key word for a painter.
- Avoid generic template looks: no centered-hero-plus-three-identical-cards layout, no stock-photo vibe, no gradient blobs for their own sake. Vary layout rhythm (split hero, dark band, light band, offset shadows, asymmetric grids).
- Polish: hover and focus-visible states, consistent spacing, real favicon (inline SVG data URI is fine), WCAG AA contrast on all text and buttons, prefers-reduced-motion support, alt text that describes what the photo actually shows.
- On phones (≤600px), add a sticky bottom call bar: "Call ###-###-####" plus one secondary action.

## Rule 4: photos

- Use only the real photos I attach or the brief lists as theirs. Never use stock, AI-generated or composite images, and never generate people, trucks, or jobs.
- Read any text inside each photo. Never show another company's name, license plates, kids/family photos, or anything the brief says to skip.
- Every image: max-width:100%; height:auto, or a fixed aspect-ratio box with object-fit:cover. Never stretch or distort.
- Sharpness check: an image's real pixel width should be at least 1.5× its displayed CSS width on desktop. If a photo is too small, display it smaller rather than blowing it up.

## Rule 5: technical

- One file: index.html with inline <style> and <script>. No frameworks, no build tools, no external JS. Google Fonts is the only external request. Image paths point to img/<short-name>.jpg.
- Head must include: <!DOCTYPE html>, <html lang="en">, <meta charset="utf-8">, <meta name="viewport" content="width=device-width, initial-scale=1">, <meta name="robots" content="noindex,nofollow">, and <title><Business> — Website concept by Cream City Post</title>.
- Responsive with CSS grid using minmax(0,1fr) and clamp() headline sizes. No horizontal scroll at 375px. Tap targets at least 44px. Every tel: link uses the +1 format (tel:+14145551234).
- Target under 1 MB total page weight, with no console errors and no placeholder or lorem ipsum text.

## How to work

1. Read the whole brief. List, for yourself: the verified facts you will use, the claims you will leave out, the palette and fonts, the motif, and which ONE interactive you'll build and why.
2. Write the complete index.html. Don't abbreviate any part of it.
3. Self-check before answering. Check every fact against the brief; delete anything unverified. Confirm there is exactly one interactive, ~5 blocks, the footer wording above, tap-to-call in the header, contact card and mobile bar, and nothing that would overflow at 375px.
4. Reply with:
   - (a) the full index.html in one code block,
   - (b) a list of the image filenames the page expects and how to crop each one,
   - (c) a short note for me: what you built, what you left out and why, and anything I need to confirm with the owner (phone choice, years, photo ownership, etc.).

## Creative brief

<PASTE THE FULL CREATIVE BRIEF HERE>

## Attached files

<List the attached photos and logo with one line each on what they show>
