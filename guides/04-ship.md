# Guide 4: Ship

> Put it live at a real URL. Share it with anyone.

Deploying used to be complicated. Vercel makes it a one-time setup, then automatic forever after. Once connected, every `git push` you do will automatically update your live site.

---

## How this works

```
You push code to GitHub → Vercel detects the push → Vercel builds and deploys automatically
```

You set this up once. After that, shipping is just `git push`.

---

## Step 1 — Make sure your code is on GitHub

Before connecting Vercel, your project needs to be pushed to GitHub. If you haven't done that yet, go back to [Guide 3](03-save.md) and complete the GitHub connection section.

Check that your code is on GitHub by visiting `github.com/yourusername/my-project` in your browser. You should see your project files there.

---

## Step 2 — Connect Vercel to GitHub

1. Go to [vercel.com](https://vercel.com) and log in
2. Click **Add New → Project**
3. Click **Import** next to your GitHub repo (`my-project`)
4. Leave all the settings as-is — Vercel auto-detects Next.js
5. Click **Deploy**

Vercel will build your project. This takes about 60 seconds the first time.

---

## Step 3 — Get your live URL

When the build finishes, Vercel gives you a URL like:

```
https://my-project-abc123.vercel.app
```

Your project is live. Share the link with anyone.

---

## Step 4 — Every push is now a deploy

From this point on, your workflow is:

```
git add .
git commit -m "what I changed"
git push
```

Vercel will detect the push and automatically update your live site in about 60 seconds.

No manual deploys, no extra commands. Push and you're done.

---

## Optional: Add a custom domain

If you want a proper domain (like `myproject.com` instead of the Vercel URL):

1. Buy a domain from [Namecheap](https://namecheap.com) or [Cloudflare](https://cloudflare.com/products/registrar/) (~$10–15/year)
2. In Vercel, go to your project → **Settings → Domains**
3. Add your domain and follow the DNS instructions

Vercel handles HTTPS automatically. Your site is secure by default.

---

## You've shipped something

That's the full loop:

1. ✅ **Setup** — tools installed
2. ✅ **Build** — AI wrote your project
3. ✅ **Save** — code is on GitHub
4. ✅ **Ship** — live at a real URL

---

## What's next

Keep building. The loop is the same every time:

1. Open your project: `cd my-project && claude`
2. Describe what you want to change or add
3. Preview at `localhost:3000`
4. Commit and push when it looks right

Every project you build from here uses the same four steps. You get faster each time.

---

## Stuck on something?

- Check the [starter prompts](../prompts/) for ideas on what to build next
- Open an issue on this repo if a guide is unclear
- Ask Claude Code directly — it can explain anything about your own project
