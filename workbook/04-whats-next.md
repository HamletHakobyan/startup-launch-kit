# 4. What's next

**Goal:** know how to take your prototype further, and share what you built.

You now have a full-stack AI app running on Cloudflare: website, API, database and AI. Your prototype is your production: you can keep growing this exact project, with no rewrite and no migration. Here is where to go from here.

## The demo you just saw: AI agents and MCP

The presenter showed how the same Worker can become:

- **An MCP server.** MCP (Model Context Protocol) is a standard way for AI assistants such as Claude or ChatGPT to use tools. Your menu, waitlist and orders could become tools that an AI assistant calls directly ("order 3 portions for the office", "add this person to my waitlist").
- **An AI agent.** With the Cloudflare **Agents SDK**, an agent can remember conversations, run tasks on a schedule, and call your APIs, all running on Workers.

Learn more:

- Agents: https://developers.cloudflare.com/agents/
- Build a remote MCP server: https://developers.cloudflare.com/agents/guides/remote-mcp-server/

## Ideas to continue on your own

- **Use your own domain** (for example `yourstartup.uz`). Add your domain to Cloudflare, then in your Worker go to **Settings** → **Domains & Routes** → **Add** → **Custom domain**. Guide: https://developers.cloudflare.com/workers/configuration/routing/custom-domains/
- **Get notified about new signups**, for example by sending yourself an email or a Telegram message from the Worker.
- **Change the design.** Your brand colour is `accentColor` in `src/config.ts`; other colours and fonts are in `src/styles/global.css`.
- **Write blog posts.** Add Markdown files to `src/content/blog/` (see the Level 1 bonus). Delete the two sample posts when you have your own.
- **Try a different look.** Any static theme from https://astro.build/themes can be deployed the same way, on Workers static assets.
- **Give your assistant more knowledge (RAG).** Right now it knows only `src/config.ts`. For bigger content (docs, a product catalogue, PDFs), Cloudflare **AI Search** indexes your content and lets the assistant find the right passage before answering: https://developers.cloudflare.com/ai-search/
- **Try another AI model.** Change the `AI_MODEL` line in `worker/index.ts`. Model list: https://developers.cloudflare.com/workers-ai/models/
- **Work like a developer.** Open your repo in GitHub Codespaces, or install Node.js and run `npx wrangler dev` to preview changes on your computer before you publish.

## Cloudflare for Startups

**Bootstrapped or raised under $1M?** You may qualify for **$10,000 in Cloudflare credits** through the Cloudflare for Startups program (the program offers up to $350,000 at its highest tier). Requirements include a live website (you now have one!), a business email on your domain, a public LinkedIn/X/GitHub presence, and being founded within the last 10 years. See the full eligibility list on the page. Credits are valid for one year.

Apply at **cloudflare.com/forstartups** (terms may change, so check the page for the current details):

https://www.cloudflare.com/forstartups/

## Talk to us

- **Want a Cloudflare solutions engineer to review your architecture?** Leave your details here: <SE_REVIEW_FORM_LINK>
- **Questions after the workshop?** Join our Telegram community for help from the team and other founders: <TELEGRAM_GROUP_LINK>

## LinkedIn giveaway 🎧

Post about the workshop on LinkedIn and you can enter the prize draw for **AirPods**.

**How to enter:**

1. Publish a LinkedIn post about today's workshop **within 48 hours** after it ends.
2. **Tag Cloudflare** (type `@Cloudflare` and choose the company page) **and the presenter** (type `@<PRESENTER_NAME>` and choose their profile).
3. Include the hashtag `<#WORKSHOP_HASHTAG>`.
4. Make the post **public** so we can see it.

Subject to official rules: <RULES_LINK>. Winner announced <WINNER_DATE> on LinkedIn. One entry per person. Cloudflare employees are not eligible. No purchase necessary.

A screenshot of your site or your favourite AI assistant answer makes the post stand out.

**Copy-paste template** (replace `<STARTUP NAME>` and `<YOUR LIVE URL>`):

```text
Today I built and launched a website for my startup <STARTUP NAME> in under 2 hours, for free, at the Cloudflare Developer Platform workshop for startups in Uzbekistan 🇺🇿

✅ Landing page running on Cloudflare's network in 330+ cities
✅ Waitlist with a real database
✅ AI assistant that answers customers in their own language

From a GitHub commit to live in about a minute. No servers to manage, no code written from scratch, and my prototype is already production-ready.

Check it out and join the waitlist: <YOUR LIVE URL>

Thanks @Cloudflare and @<PRESENTER_NAME>!

<#WORKSHOP_HASHTAG> #Cloudflare #startups #Uzbekistan
```

**Kept Plovify?** Use this one instead (replace `<YOUR LIVE URL>`):

```text
Today I launched Plovify — Plov as a Service 🍚 (a fictional startup, a very real stack) at the Cloudflare Developer Platform workshop for startups in Uzbekistan 🇺🇿

✅ Landing page served from Cloudflare's network in 330+ cities (zero cold starts, unlike cold plov)
✅ Waitlist with a real database
✅ AI assistant that answers in English, Russian, Uzbek and more

From a GitHub commit to live in about a minute, in under 2 hours, for free. No servers to manage, and the prototype is already production-ready.

Ask my AI assistant about plov: <YOUR LIVE URL>

Next: my own startup on the same stack.

Thanks @Cloudflare and @<PRESENTER_NAME>!

<#WORKSHOP_HASHTAG> #Cloudflare #startups #Uzbekistan
```

## Feedback

Please tell us how it went. It takes 2 minutes and helps us improve the next workshop:

<FEEDBACK_SURVEY_LINK>

Thank you for building with us! 🚀
