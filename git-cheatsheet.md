# Git Cheatsheet

## Workflow

1. Clone a repository

   ```bash
   git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
   ```

2. Review what changed:

   ```bash
   git status
   ```

3. Stage the changes:

   ```bash
   git add .
   ```

4. Create a snapshot:

   ```bash
   git commit -m "Describe your change"
   ```

5. Send the commits to GitHub:

   ```bash
   git push
   ```

> **Tip:** Run `git status` whenever you are unsure. It is safe and does not change your files.

## View commit history

```bash
git log
```

Displays commit history, with the newest commit first.

> Press `q` to leave the log viewer.

## The command pattern

Most Git commands follow this general pattern:

```text
git <command> [options] [destination]
```

| Part            | Meaning                               | Example                   |
| --------------- | ------------------------------------- | ------------------------- |
| `git`           | Program                               | Runs Git                  |
| `<command>`     | Action                                | `add`, `commit`, `status` |
| `[options]`     | Optional setting or flag              | `-m`                      |
| `[destination]` | File, branch, remote, or other target | `.`, `origin`, `main`     |

## Read commands from left to right

```text
git add .
git | add | .
```

```text
git commit -m "message"
git | commit | -m | "message"
```

```text
git status
git | status | (no destination)
```

---
