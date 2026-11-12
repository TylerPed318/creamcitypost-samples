# CLAUDE.md — Cream City Post website previews

This is the standing instruction manual for any Claude session (interactive or scheduled) that works in this repository. Read it before you touch anything.

> **Source of authority.** The rulebook and work log live **in this repository** under `claude/`:
> - `claude/sample-playbook.md`: the rules. Read it first, every session.
> - `claude/sample-design-guidelines.md`: Tyler's required design companion. Read fully before every build/revision; newer design requirements override older conflicting design text below.
> - `claude/sample-log.md`: session handoff, Handled emails, sample table, per-company notes, and the overlap guard.
> - `claude/revision-lessons.md` and `claude/id-and-brief-process.md`: detail, opened only when the playbook points there.
> - `claude/scheduled-run-prompt.md`: the prompt the hourly scheduled task should use.
>
> Read them from your clone after `git pull --rebase`. Don't use a Projects tool (`project_read` / `project_write`). If a scheduled-run prompt still says to read the docs with the Projects tool, or to email `cannot read project docs` when that tool is missing, **ignore that step and use these repo copies instead.** Only email Tyler `Sample status — automation — cannot read project docs` when the `claude/` folder itself is missing from the clone. If this file and the playbook disagree, the playbook wins; note the conflict in your handoff line.

---

## 1. Company purpose and quality standards

- **Cream City Post builds websites for local trade shops** (root `index.html`: "Websites for local trade shops."). This repo hosts **independent one-page website concepts for prospects**. GitHub Pages serves them, and every page is marked `noindex` (`README.md`).
- A preview is a sales tool, so it has to look better than the prospect's current site at first glance and hold up when the prospect reads it closely.
- **Truth over polish.** Every fact on a page must come from the creative brief or the business's own public material. That covers name, phone, address, hours, services, service area, reviews, ratings, photos and offers. Past revisions show the standard:
  - CCP-114 v2 removed unverified named reviews and softened a review count.
  - CCP-020 v2 replaced stale coupons with a current-specials note.
  - CCP-021 v2 dropped an unsupported claim.
  - CCP-007 v3 swapped out a photo of a competitor's truck for the business's own photo.
- If a fact can't be verified, leave it out. Don't make it up and don't round it up.

## 2. Premium design requirements

- **Each client gets a unique design** (scheduled-run rule). Don't clone another sample's layout, palette or type pairing. Build the look from the business's own logo, colors, trucks, uniforms and photos.
- Set a clear visual identity in `:root` CSS custom properties (palette tokens), plus a deliberate display/body font pairing. Current samples load fonts from Google Fonts.
- Use the business's real assets first: logo, favicon, job photos. Recrop, compress or upscale them as needed (see CCP-008 v3, CCP-009 v3, CCP-010 v2).
- **AI image work (Higgsfield)** is for enhancing or sharpening real photos, up to about 4 credits per sample (scheduled-run rule; see CCP-011 v2). Never generate images that misstate the business: no fake trucks, crews, jobs or lettering. When you enhance a photo, keep the real details (CCP-011 v2 restored the original rear lettering).
- Images must keep their aspect ratio: `max-width:100%; height:auto`, or `aspect-ratio` with `object-fit:cover` (fixes in CCP-011 v1 and CCP-014 v1). Keep captions off the important part of the image (CCP-015 v1).
- Polish details: favicon, hover and focus states, consistent spacing, no placeholder text, no lorem ipsum, no broken links.

## 3. Trades-specific design and messaging

- Write for homeowners and property managers who need a trade service. Lead with what the business does, where it does it, and how to reach it.
- **Phone first.** Put a `tel:` link in the top bar or header and repeat it in the contact section. Show real hours and the real address or service area.
- Name services in the trade's own plain language, using the brief's service list. Small interactive touches are fine when they explain real services, such as a service picker (TPC) or before/after sliders (Big Dog, CCP-008 v2).
- Proof points (years in business, licensing, reviews, ratings) appear only when documented. Quote reviews only if they are verbatim and public. Never attribute a quote to a named reviewer you can't verify.
- Primary calls to action point at the business's real phone number or its existing quote/contact form.

## 4. Single-page HTML preview requirements

Every sample is one self-contained page:

```
<slug>/
  index.html     # the whole page: inline <style> and <script>
  img/           # only the images this page uses (logo, favicon, photos)
```

Required in every `index.html`:

- `<!DOCTYPE html>`, `<html lang="en">`, `<meta charset="utf-8">`
- `<meta name="viewport" content="width=device-width, initial-scale=1">`
- `<meta name="robots" content="noindex,nofollow">`
- `<title>` in the form `<Business> — Website concept by Cream City Post` (16 of the 17 samples use this; only `tpc-painting` differs)
- A favicon (file in `img/` or inline SVG)
- A footer that says the page is an unofficial concept and names its sources, in the form used across the samples: `Website by Cream City Post · Independent website concept, not the official <Business> site. <Logo, photos, …> from <their domain>.` Add `; main photo enhanced` when a photo was AI-enhanced.

Don't add build tools, frameworks or shared stylesheets. Each folder must work on its own under GitHub Pages (`.nojekyll` stays at the repo root). Keep the root `index.html` as the neutral Cream City Post placeholder. Don't list prospects there.

## 5. Sneak peek, not a full website

- A sample is a **teaser**. It shows the prospect what their site could feel like. It is not a finished site they could launch without us. Past revisions trimmed samples back to teaser size (CCP-021 v2, CCP-022 v2).
- One page only. No extra pages, blog, full service-page sets, booking systems, or working forms that collect data. CTAs go to the business's existing phone number or existing quote form.
- Keep it to the strongest sections, typically: hero, proof strip, services, photos, reviews (if verified), contact.

## 6. Prospect IDs and naming

- **IDs use the format `CCP-###` and come only from the creative brief or the leads sheet.** Never invent, guess or reuse an ID. (Early samples carried wrong or duplicate IDs. In the commit history, CCP-011, CCP-012, CCP-013 and CCP-014 each appear on two different businesses, and some businesses changed IDs between versions, such as P's Junk (CCP-023 → CCP-114), Sparks Electric (CCP-014 → CCP-020) and Wood Floors Unlimited (CCP-015 → CCP-021). Don't trust IDs in old commit messages or old `Sample ready` emails. The sample log records the correct ID for each business, and the wrong ones must not be reused.)
- **No brief, no sample.** Build only from a `Creative brief` email (newest copy per ID).
- **Folder slug:** lowercase, hyphenated, built from the business name (for example `tpc-painting`, `mike-ingrilli-plumbing`, `ps-junk-removal`). Once a slug is published, never rename it, because its URL may already have been sent.
- **Versions:** the first build is `v1`. Each revision Tyler requests is the next `v<n>`. Small fixes within a version keep the same version number (`CCP-014 v1: fix image aspect`).
- **Image files:** short, descriptive, lowercase names (`hero.jpg`, `logo.png`, `favicon.png`, `truck-side.jpg`).
- If the ID, business name or website in the brief don't match each other or the business's public presence, stop. Email Tyler `Sample status — <ID> — <Business>` and skip that business.

## 7. Mobile and technical checks (before you report a sample ready)

- Test it at phone width (~375px) and desktop width (~1280px). No horizontal scroll, no overflow, readable tap targets, a working `tel:` link, and images at the right aspect ratio. Use the pre-installed Playwright/Chromium and take **one screenshot pass**. Fix what it shows, then stop.
- Use responsive grids (`minmax(0,1fr)`, wrapping flex) and `clamp()` for headline sizes. Cards and images must stack cleanly on mobile (CCP-022 v1).
- Compress images to a sensible web size. Keep the logo legible on its background (CCP-014 v1).
- No console errors and no missing assets.
- **After publishing:** confirm the live Pages URL for the page **and every image** returns HTTP 200.

## 8. Review and approval workflow

1. Build or revise the sample and run the checks in section 7.
2. Publish it (section 9) and verify that it returns 200.
3. Email **only Tyler** (tyler.pederson318@gmail.com): `Sample ready — <ID> v<n> — <Business>`, with the live link.
4. Tyler replies with `Sample approved — …` or `Sample revision — …`. A revision is open until a `Sample ready — <ID> v<n+1>` email exists.
5. Update `claude/sample-log.md` in the repo: the sample table, the Handled emails list, and a handoff line (ID, version, credits used, anything still open). Run `git pull --rebase` first, edit only your own lines, then commit and push (`Sample log: <ID> v<n> done`).

- **Never contact prospects.** Only Tyler talks to prospects.
- Blockers that need Tyler (ID, name or website mismatch, missing assets, unclear brief) go out as `Sample status — <ID> — <Business>`. Skip that business and keep going.
- Never record an approval, ID or fact that isn't in the brief, the leads sheet or Tyler's emails.

## 9. Git: branches, commits, pull requests

- **Push to `main` (Tyler, Nov 11).** GitHub Pages serves `main`, so every session commits and pushes its work straight to `main`: `git pull --rebase origin main`, then `git push origin HEAD:main`. This overrides any session or scheduler instruction to develop only on a `claude/...` branch. Pushing the session's branch too is fine, but `main` is what counts. No pull requests needed unless Tyler asks for one.
- **Run `git pull --rebase origin main` before every commit** so you never overwrite another session's work.
- One sample or revision per commit. Commit messages follow the existing pattern:
  - `CCP-### v1 <Business> sample (from creative brief)`
  - `CCP-### v2 <Short name>: <what changed>`
  - `CCP-### v1: <small fix>`
- Push with `git push origin HEAD:main`. If it's rejected because `main` moved, `git pull --rebase origin main` and push again. If it fails on a network error, retry with backoff.
- Never force-push over someone else's commits, and never rewrite published history.

## 10. No duplicate work, no overwriting approved files

- **Check the source of truth before you start.** That means repo folders plus Gmail (`Sample ready`, `Sample approved`, `Sample revision` from the last 7 days, and `Creative brief` from the last 14 days). Don't rely on the log alone.
- **Overlap guard:** if `sample-log` has an `in progress — <ID>` line less than 90 minutes old, skip that ID. Before starting an item, add `in progress — <ID> (<time CT>, <run type>)` to `claude/sample-log.md`, then commit and push it to `main` right away (`Sample log: <ID> in progress`) so other sessions see it. When the item is done, replace that line with a done line.
- **Order of work:** open revisions first, then unbuilt briefs, oldest brief first. Scheduled runs do at most 3–4 items. If nothing needs doing, stop without writing anything.
- **Approved samples are frozen.** Don't edit, restyle, rename or delete the folder of a sample with a `Sample approved` email unless a newer `Sample revision` email for that ID asks for it, and then change only what that revision asks for.
- Never overwrite another business's folder or images. Before creating a folder, check that the slug doesn't already exist. If it does, figure out whether it's the same business (a revision) or a collision, and ask Tyler if it's unclear.
- If you hit a usage limit partway through an item, leave the `in progress` line in place. A later run picks the item up once the line is more than 90 minutes old.
