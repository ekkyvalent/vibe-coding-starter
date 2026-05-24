# Guide 1: Setup

> One-time setup. Never again.

This guide gets your computer ready to build. It takes about 20–30 minutes. After this, you can start any new project in under a minute.

---

## What you're installing

| Tool | What it is | Why you need it |
|---|---|---|
| Node.js | The engine that runs JavaScript on your computer | Next.js (your building tool) needs it |
| Git | A save system for code | Tracks every version of your project |
| Claude Code | Your AI coding partner | The thing that writes the code |
| VS Code | A text editor built for code | Where you'll review and manage files |

---

## Step 1 — Install Node.js

1. Go to [nodejs.org](https://nodejs.org)
2. Download the **LTS** version (the one labeled "Recommended For Most Users")
3. Run the installer, click through all the defaults

To confirm it worked, open your Terminal (Mac: press `Cmd + Space`, type "Terminal", press Enter) and type:

```
node --version
```

You should see something like `v20.11.0`. If you see a number, you're good.

---

## Step 2 — Install Git

**Mac:** Git usually comes pre-installed. Check by running:

```
git --version
```

If you see a number, skip to Step 3. If you see an error, download Git from [git-scm.com](https://git-scm.com) and install it.

**Windows:** Download from [git-scm.com](https://git-scm.com) and install.

---

## Step 3 — Install VS Code

1. Go to [code.visualstudio.com](https://code.visualstudio.com)
2. Download and install

This is where you'll look at your files, review what the AI built, and occasionally make small edits.

---

## Step 4 — Install Claude Code

Claude Code is the AI that will build your project. It runs inside your Terminal.

1. In your Terminal, run:

```
npm install -g @anthropic-ai/claude-code
```

2. Then run:

```
claude
```

3. It will ask you to log in with your Anthropic account. Follow the prompts.

If you don't have an Anthropic account, create one at [claude.ai](https://claude.ai) first.

---

## Step 5 — Create a free Vercel account

Vercel is where your project will live on the internet. It's free for personal projects.

1. Go to [vercel.com](https://vercel.com)
2. Sign up with your GitHub account (if you don't have GitHub, create one at [github.com](https://github.com) first)

You won't need to do anything in Vercel yet. Have the account ready.

---

## You're done with setup

Your computer can now build and ship real web projects.

Next: [Guide 2 → Build your first project](02-build.md)
