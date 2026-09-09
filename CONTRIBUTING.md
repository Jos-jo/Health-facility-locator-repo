# Contributing (Freelancer Guide)

1. **Pick up an issue** from the Project board's `Ready` column — don't start
   work on anything still in `Backlog` without a go-ahead, and don't work two
   issues at once.
2. **Branch from `dev`**: `git checkout -b feature/<issue-number>-<slug>`.
3. **Commit small and often.** Reference the issue number in each commit,
   e.g. `git commit -m "#03 add current-location button"`.
4. **Open a PR into `dev`** as soon as the issue's acceptance criteria are
   met. Fill in the PR template — link the issue, list what changed, add a
   screen recording or screenshots for anything UI-facing.
5. **Move the card** on the board to `In Review` when the PR is open.
6. **Respond to review comments within 24h** on working days. Two rounds of
   review are included per issue at the agreed price; anything beyond that
   is scoped as a change request.
7. **Daily async update**: one line in the agreed Slack/WhatsApp channel —
   what shipped, what's blocked, what's next. This is separate from and
   shorter than the Google Sheet update (see `docs/PROJECT_BOARD.md`).

## Coding standards

- Match the existing repo's linter/formatter config (ESLint + Prettier) —
  run `npm run lint` before opening a PR.
- No API keys, tokens, or `.env` files committed. `.env.example` only.
- New dependencies must be justified in the PR description (why this
  package, bundle-size impact if relevant).

## Definition of done (applies to every issue)

- Acceptance criteria in the issue are all met.
- Code reviewed and merged into `dev`.
- No new console errors/warnings.
- Works on the two breakpoints specified in the issue (mobile + desktop).
- Sheet updated: status, actual hours/cost, notes.
