# Guide 2: Build

> Tell the AI what you want. Watch it build.

You're going to create a real Next.js project and tell Claude Code what to build, in plain English.

---

## Step 1 — Create your project folder

Open your Terminal and run these commands one at a time:

```
cd Desktop
```
*(This moves you to your Desktop — a good place to keep your projects)*

```
npx create-next-app@latest my-project --typescript --tailwind --eslint --app --no-src-dir --import-alias "@/*"
```

When it asks questions, press `Enter` to accept all the defaults.

This creates a folder called `my-project` on your Desktop with a working Next.js app inside.

> **Tip:** Replace `my-project` with whatever you want to call your project (no spaces — use dashes instead, like `my-landing-page`).

---

## Step 2 — Open your project in VS Code

```
cd my-project
code .
```

VS Code will open with your project files on the left. You don't need to understand them yet.

---

## Step 3 — Add the CLAUDE.md file

This file tells Claude Code important context about your project so it works better.

Copy the [template CLAUDE.md](../template/CLAUDE.md) file into the root of your project folder (the `my-project` folder, not inside any subfolders).

You can edit the `PROJECT_NAME` and `DESCRIPTION` fields to match your project.

---

## Step 4 — Start Claude Code

In your Terminal (make sure you're still inside your project folder), run:

```
claude
```

You'll see a prompt. This is your AI coding partner. You talk to it in plain English.

---

## Step 5 — Build something

Pick one of the [starter prompts](../prompts/) and paste it in. Or write your own.

**Example of a simple first prompt:**

```
Build me a clean landing page for my project. 

It should have:
- A headline that says "Coming Soon"
- A short description: "Something exciting is on the way."
- An email input field where people can sign up to be notified
- A submit button
- Clean, minimal design with a white background

Use the existing Next.js app structure.
```

Press Enter. Watch Claude write the code.

---

## Step 6 — Preview it in your browser

While Claude Code is open, open a **new Terminal window**, navigate to your project, and run:

```
npm run dev
```

Then open your browser and go to:

```
http://localhost:3000
```

You'll see your project live on your computer.

---

## Talking to Claude Code

You can keep chatting with Claude to refine what it built:

- *"Change the background color to light blue"*
- *"Make the headline bigger"*
- *"Add a section below with three feature bullet points"*
- *"The button doesn't look right, make it more prominent"*

It will make the changes and you can refresh your browser to see them instantly.

---

## When you're happy with it

Move to the next guide to save your work properly.

Next: [Guide 3 → Save your work](03-save.md)
