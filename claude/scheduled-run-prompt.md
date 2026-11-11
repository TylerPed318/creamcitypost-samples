# Hourly scheduled-run prompt (paste into the scheduled task)

Copy everything between the lines into the scheduled task's prompt at claude.ai/code/routines (open the task's ⋯ menu, choose **Edit**, then **Save changes**).

---

You are running the hourly Cream City Post sample builder for Tyler Pederson. Work unattended: don't ask questions. Make the most reasonable call, note it in the handoff line, and keep going.

1. Attach and clone the hosting repo: add_repo TylerPed318/creamcitypost-samples (push access), then clone it. The rulebook and log live in the repo under `claude/`. Read `claude/sample-playbook.md` (all the rules; follow it exactly), then `claude/sample-log.md` (handoff lines, Handled emails, sample table). If the `claude/` folder is missing, email Tyler `Sample status — automation — cannot read project docs` and stop. Push every commit straight to `main` (GitHub Pages serves `main`): before every commit run `git pull --rebase origin main`, then push with `git push origin HEAD:main`. This applies even if the session says to develop on a `claude/...` branch; Tyler approved pushing to `main` on Nov 11. No pull requests.
2. Work out what is already done from the SOURCE OF TRUTH, not the log alone: repo folders, plus Gmail `subject:"Sample ready" newer_than:7d`, `subject:"Sample approved" newer_than:7d` and `subject:"Sample revision" newer_than:7d`. A revision is open if no `Sample ready — <ID> v<n+1>` exists after it. A brief is unbuilt if no `Sample ready — <ID>` email or repo folder exists for that business (ignore old Sample ready emails that used wrong IDs; the log lists them).
3. Overlap guard: if the log has an "in progress — <ID>" line less than 90 minutes old, skip that ID. Before starting each item, `git pull --rebase origin main`, re-read `claude/sample-log.md`, append "in progress — <ID> (<time CT>, scheduled run)", then commit and push that change right away.
4. Order: open revisions first, then unbuilt briefs (`subject:"Creative brief" newer_than:14d`, newest copy per ID, oldest brief first). No brief = no sample.
5. If there's nothing to do, stop right away without writing anything. Keep idle runs cheap.
6. Otherwise do up to 3–4 items this run, following the playbook: IDs only from the brief/leads sheet; unique design per client; Higgsfield up to ~4 credits per sample; one screenshot pass. Publish by pushing to `main`, verify the page and images return 200, then email tyler.pederson318@gmail.com `Sample ready — <ID> v<n> — <Business>`.
7. After each item: `git pull --rebase origin main`, re-read `claude/sample-log.md`, update the table and Handled emails, replace your "in progress" line with a done line (ID, version, credits, anything open), then commit and push to `main`. Add any new lesson to `claude/revision-lessons.md` the same way.
8. If you hit a usage limit mid-item, leave the "in progress" line; a later run resumes once it's more than 90 minutes old.
9. Never contact prospects. Never invent IDs or facts. If a blocker needs Tyler (ID, name or website mismatch, etc.), email him `Sample status — <ID> — <Business>`, skip that business, and continue.

---

Note: the playbook and log are public in this repo (GitHub Pages serves the whole repo). Don't put passwords, tokens or anything private in `claude/`.
