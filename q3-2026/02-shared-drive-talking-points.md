# Talking Points — Shared Drive Restructure

---

## The why

The next thing on our roadmap is standardizing the file naming and folder structure across SharePoint. I want to start with why this matters.

Most of the automations we've been talking about — things people have brought up to me — require software to be able to programmatically look up where a document is. That means surfacing the right document to you when you need it. It means automatically extracting data from a document and loading it into SiteTracker when it's dropped in a precise location with the right name. It means automatically assembling document packages for you once all the required documents are present in the right location and follow a naming convention.

Reorganizing our filesystem opens the door to a very large number of opportunities that will be helpful to everyone.

---

## The problem

That said, it won't be easy, and I can't do it alone — but I can do a very large chunk of it.

Right now we have 54,000 files, none of which follow a standard naming convention. We have dates formatted different ways, different ways to track versions. There are roughly 385 different names for what should be about 14 folder types. We have "Budgets & Invoices", "Budget and Invoices", "Budgets and Invoices" — three variations of the same folder, and dozens more like that.

The bottom line: if I asked a computer to find a specific document for a specific site, it would not be able to run that query reliably.

---

## The approach

Here's the plan. I've designed it to require as little effort from everyone as possible.

**Tier 1 — Automated (~65% of files).** For about two-thirds of our files, moving and renaming is obvious. I don't need to ask anyone. The system will rename them automatically based on where they live and what's already in the filename.

**Tier 2 — AI-assisted (~25% of files).** For another quarter of the files, it's less clear. Maybe the filename is just "Final.pdf" or a vendor-generated name. For these, I'm using AI to analyze the context — the folder it's in, the files around it, the file type — and propose a name. This is still fully automated, no effort needed from you.

**Tier 3 — PM review (~10% of files).** For the last 10%, where AI can't be confident — like a file named "(2).pdf" with no context — I'll drop them in a review dashboard. You'll see the original name, the original location, and a proposed new name. You approve it, tweak it, or flag it — that's it. If you approve or tweak it, the system will automatically move and rename the file in the shared drive to reflect that.

Combined, the first two tiers should handle about 90% of the work with no effort from you all. The 10% that needs your eyes is genuinely the stuff only you could answer, and it's my goal to give you all the information up front and make that task as easy as possible.

---

## Timeline

In the next couple of weeks, I'll finish building the classification system. Then I'll roll out migrations in phases. I'll start with a small test — one site in one market — and then do the rest of the migrations on weekends, market by market.

Once a market is migrated, you'll see your dashboard populated with the files I could not resolve. Your total involvement is reviewing maybe 5–10% of files in a simple approve/modify interface over the next month. Everything else is automated.

---

## Reassurances

A couple of important points.

The files themselves are never opened or edited. I am not copying or moving data, so there is no risk of file corruption — I'm just updating SharePoint metadata.

Because of the approach I'm taking, all version history is preserved. And every change made to any file is logged in a database and reversible. If anything looks wrong or you're unable to find a file, I can undo any individual change.
