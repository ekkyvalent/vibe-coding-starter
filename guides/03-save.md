# Guide 3: Save

> Commit your work. Like saving a document, but smarter.

Git is a version control system. Think of it like Google Docs version history — but for your entire project. Every "save" (called a **commit**) is a snapshot you can go back to at any time.

You only need three commands. That's it.

---

## First-time Git setup

If this is your first time using Git on this computer, run these two commands once to tell Git who you are:

```
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Use the same email as your GitHub account.

---

## Setting up your project with Git

In your Terminal, inside your project folder, run:

```
git init
```

This turns your project folder into a Git-tracked project. One time, per project.

Then:

```
git add .
```

This stages all your files — telling Git "I want to include everything in my next save."

Then:

```
git commit -m "first commit"
```

This creates your first snapshot. The message in quotes is just a note to your future self about what changed.

---

## The three commands you'll use forever

Every time you want to save your progress:

```
git add .
git commit -m "describe what you changed"
git push
```

**What each does:**

| Command | Plain English |
|---|---|
| `git add .` | "Select everything that changed" |
| `git commit -m "..."` | "Take a snapshot and label it" |
| `git push` | "Send it to GitHub so it's backed up online" |

---

## Connecting to GitHub (one time per project)

To use `git push`, you need to connect your project to GitHub first.

1. Go to [github.com](https://github.com) and click **New repository**
2. Name it the same as your project folder (e.g. `my-project`)
3. Leave it public, don't add any files
4. Click **Create repository**
5. GitHub will show you a page with commands. Copy and run the ones under **"…or push an existing repository from the command line"**

It looks like this:

```
git remote add origin https://github.com/yourusername/my-project.git
git branch -M main
git push -u origin main
```

After this, `git push` is all you need every time.

---

## Good commit message habits

Write commit messages that describe **what changed**, not what you did:

| Instead of... | Write... |
|---|---|
| `"update"` | `"add email signup section"` |
| `"fix stuff"` | `"fix button color on mobile"` |
| `"changes"` | `"change headline copy"` |

Future you will thank you.

---

## When to commit

A good rule of thumb: commit whenever you finish something that's working. After you add a new section, fix something, or get a feature working the way you want — commit it.

You can't "over-commit." More saves = more safety net.

---

Next: [Guide 4 → Ship it live](04-ship.md)
