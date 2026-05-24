# Starter Prompt: Waitlist / Coming Soon Page

Copy and paste this into Claude Code to build a waitlist page that collects emails.

---

## The prompt

```
Build me a "coming soon" waitlist page. Here are the details:

PRODUCT NAME: [your product name]
HEADLINE: [what you're building, in one punchy line]
DESCRIPTION: [1-2 sentences about what it is and why people should care]
LAUNCH TIMEFRAME: [e.g. "Launching Summer 2025" or "Coming soon"]

The page should:
- Take up the full screen (one-page layout)
- Show the product name prominently
- Show the headline and description
- Have an email input field and a "Join the waitlist" button
- Show a success message after someone submits their email
- Look polished and modern — dark background preferred

For the email submission: just use a simple form that shows a "You're on the list!" message on submit. No backend needed for now.

Use the existing Next.js app structure. Put everything in app/page.tsx. Use Tailwind CSS for styling.
```

---

## How to fill it in

Replace everything in `[square brackets]`:

- `PRODUCT NAME: Pingo`
- `HEADLINE: The simplest way to track what matters`  
- `DESCRIPTION: A lightweight tool for indie founders who need focus, not complexity. No fluff, no feature bloat.`
- `LAUNCH TIMEFRAME: Coming Q3 2025`

---

## Adding real email collection later

Once you're ready to actually collect emails, ask Claude:

*"I want to collect emails for real. Integrate this form with [Mailchimp / ConvertKit / Resend] so submissions are saved."*

Claude will guide you through the integration.
