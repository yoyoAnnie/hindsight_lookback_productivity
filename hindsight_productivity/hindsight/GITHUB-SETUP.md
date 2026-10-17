# GitHub Setup — Create the Private Repository

Do this once. About five minutes.

## 1. Create the repo

1. On github.com, choose **New repository**.
2. Name: `hindsight`. Description (private, fine to keep plain):
   `Scrapbook journal for ideas — one stream: Hand holds, Brain directs, Eye shows.`
3. Visibility: **Private** — this is the IP rule in `docs/08-privacy-and-ip.md`.
   Do not change this later without a decision record.
4. Do **not** tick "Add a README / .gitignore / licence" — this folder already
   contains them. Importing these files into an empty repo avoids conflicts.

## 2. Push this folder

From inside this folder:

```bash
git init
git add .
git commit -m "document hindsight concept, workflow, and design system"
git branch -M main
git remote add origin https://github.com/<your-username>/hindsight.git
git push -u origin main
```

## 3. Check after the push

- [ ] The repo badge/visibility says **Private**.
- [ ] `README.md` renders with the documentation map and all links open.
- [ ] `.github/ISSUE_TEMPLATE/` offers the two issue forms on "New issue".
- [ ] No file from a `private/` or `uploads/` folder was committed
      (`.gitignore` should have prevented it — verify anyway).

## 4. Working rhythm from here

- One branch per task, one PR per change (`CONTRIBUTING.md`).
- Every session: a log in `sessions/` the same day.
- Every structural choice: a record in `decisions/`.
- This setup file can be deleted from the repo after the push is verified,
  or kept — it does no harm.
