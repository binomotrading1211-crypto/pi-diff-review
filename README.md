# pi-diff-review

This is pure slop, see: https://pi.dev/session/#d4ce533cedbd60040f2622dc3db950e2

Native diff review window for pi, powered by Glimpse and Monaco.

## What it does

Adds a `/diff-review` command to pi.

The command:

1. collects the current git diff against `HEAD`
2. opens a native macOS review window
3. shows changed files in a Monaco diff editor
4. lets you draft comments on the original side, modified side, or whole file
5. inserts the resulting feedback prompt into the pi editor when you submit

## Requirements

- macOS
- Node.js 20+
- `pi` installed
- internet access for the Tailwind and Monaco CDNs used by the review window

## Install for a project

From the target project:

```bash
pi install -l ../pi-diff-review
```

Or run pi with the extension directly:

```bash
pi -e ../pi-diff-review
```

## Manual test

1. Start pi in a git repo with local changes.
2. Run:
   ```text
   /diff-review
   ```
3. In the review window:
   - switch between changed files on the left
   - select lines on the original or modified side
   - click one of the draft comment buttons
   - write the comment in the right panel and add it
   - optionally add overall feedback
4. Click `Put feedback in pi editor`.
5. The review window closes and the generated feedback prompt is inserted into pi's editor.
6. Edit it if needed and press Enter.

## Notes

- The review source is the entire worktree: tracked changes are taken from `git diff HEAD`, and untracked files are included via `git ls-files --others --exclude-standard`.
- Repositories without a `HEAD` still show untracked files.
- Binary files are not specially handled yet.
