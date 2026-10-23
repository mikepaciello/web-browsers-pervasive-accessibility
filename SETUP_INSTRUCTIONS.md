# How to publish this repo (for Mike)

Claude prepared these files; you create/update the repo and push. Nothing here has been
sent or published. **This folder is the current, correct version (v1.7)** — use it, not any
earlier copy.

---

## ✅ WHEN AUDIOEYE APPROVES — DO THIS (quick checklist)

Hold all of this until you have AudioEye's written sign-off. Then, in order:

1. [ ] **Get written AudioEye approval** (the one gate). Keep the reply on file.
2. [ ] **Create the repo** (if not already created) — Section A below. OR **replace the old
       files** (if you already uploaded an earlier version) — Section B below.
3. [ ] **Confirm `.nojekyll` is in the repo.** Finder hides dotfiles (press Cmd+Shift+period
       to see it). If it's missing from the repo's file list, add it: **Add file → Create new
       file → name it** `.nojekyll` **→ commit** (leave it empty).
4. [ ] **Turn on GitHub Pages** — Section C.
5. [ ] **Fill in the repo "About" panel** (gear icon, top-right of the repo) — Section D.
6. [ ] **Check the live page** at
       `https://mikepaciello.github.io/web-browsers-pervasive-accessibility/` and click a few
       links to confirm they work.
7. [ ] **(After peer review settles the content) Deposit on Zenodo** for the DOI — Section E —
       then paste the DOI into the README's "How to cite" and the paper.

---

## A. Create the repository (first time)

- github.com → **New repository**.
- Name: **web-browsers-pervasive-accessibility**
- Visibility: **Public**
- Do NOT initialize with a README (this folder already has one).
- Then add files: on the new empty repo page, click **"uploading an existing file"** and drag
  in **everything** from this unzipped folder:
  - index.html
  - README.md
  - LICENSE
  - ACCESSIBILITY.md
  - .nojekyll
  - SETUP_INSTRUCTIONS.md *(optional to include — it's just these notes)*
  - web-browsers-as-a-pervasive-accessibility-solution.pdf
  - web-browsers-as-a-pervasive-accessibility-solution.docx
  - Then **Commit changes**.

(Terminal alternative, run inside this folder:)
```
git init
git add .
git commit -m "Add Web Browsers as a Pervasive Accessibility Solution (review draft)"
git branch -M main
git remote add origin https://github.com/mikepaciello/web-browsers-pervasive-accessibility.git
git push -u origin main
```

## B. Replace the files (if you already uploaded an earlier version)

The earlier upload was an older version (no live links, no accessibility statement). To update:

- On the repo page: **Add file → Upload files**.
- Drag in **all** the files from this unzipped folder. Same filenames overwrite the old ones;
  new files (ACCESSIBILITY.md) are added.
- **Commit changes.**
- Confirm `.nojekyll` is present (see checklist step 3).

## C. Turn on GitHub Pages (the readable web version)

- In the repo: **Settings → Pages**.
- Under "Build and deployment", Source = **Deploy from a branch**.
- Branch = **main**, folder = **/ (root)**. **Save.**
- After a minute, the page is live at:
  **https://mikepaciello.github.io/web-browsers-pervasive-accessibility/**
- The README's "Read online" link and the HTML already point to that URL.

## D. Fill in the repo "About" panel (optional but recommended)

Click the **gear icon** next to "About" (top-right of the repo page):
- **Description:** A research paper by Michael G. Paciello on the browser as the layer for
  universal, personalized web accessibility.
- **Website:** `https://mikepaciello.github.io/web-browsers-pervasive-accessibility/`
  *(add this only after Pages is on; there's also a "Use your GitHub Pages website" checkbox)*
- **Topics:** accessibility, web-accessibility, a11y, browsers, web-standards, w3c,
  assistive-technology, wcag, research-paper

## E. (Last step, after peer review) Add the Zenodo DOI

- zenodo.org → log in (you can "Log in with GitHub"). Either:
  - **Connect the repo** (Settings → GitHub → toggle this repo ON), then create a GitHub
    **Release** — Zenodo auto-archives it and mints a DOI; or
  - **New upload** → drag in the PDF → fill the form (type = Working paper/Preprint; title;
    authors; paste the abstract; pick the license) → **Publish**.
- Zenodo publishing is **permanent** — do it only on the finished, approved paper.
- Paste the DOI into the README's "How to cite" section and the paper's front matter.

---

## Notes

- If your GitHub username is not **mikepaciello**, tell Claude and the one URL in the README,
  the HTML, and this file will be corrected.
- To update the paper later: replace index.html + the PDF + the DOCX and commit again.
- **Do not publish until AudioEye approves.** If approval doesn't come and you need to publish
  anyway, the fallback is to remove the "CAO, AudioEye" affiliation (the paper is written in a
  personal capacity and stands without it) — ask Claude to produce that version.
