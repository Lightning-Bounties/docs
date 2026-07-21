# Posting and solving bounties for GitBook / Wikis

Many documentation sites (GitBook, MkDocs, Docusaurus, plain Markdown wikis) are **Git repositories** under the hood. Lightning Bounties works the same way as for application code: bounties attach to **GitHub Issues**, and solutions arrive as **Pull Requests** that update Markdown (or other content files).

This page explains how doc/wiki maintainers should post bounties, and how solvers should deliver changes.

## Why docs & wikis fit Lightning Bounties

| Docs workflow | Lightning Bounties mapping |
|---------------|----------------------------|
| Request a new page / fix typos / restructure SUMMARY | Open a **GitHub Issue** with clear acceptance criteria |
| Fund the work in sats | Post a **reward** on [app.lightningbounties.com](https://app.lightningbounties.com/) against that issue URL |
| Reviewer merges Markdown changes | Merge the solver’s **PR** (with `close #N` in the PR body) |
| Pay instantly after merge | Solver **claims** on the app; sats credit their LB balance |

You do **not** need a special “GitBook bounty mode.” If the docs live on GitHub and accept PRs, you can bounty them.

## For maintainers: posting a docs bounty

### 1. Keep docs in a GitHub repo

- Preferred: GitBook **Git sync** so the published site tracks a GitHub branch.
- Also works: any Markdown wiki, Docs-as-code site, or monorepo `docs/` folder with PRs enabled.

### 2. Open a specific GitHub issue

Good bounty issues for docs:

- Exact files or paths to change (e.g. `SUMMARY.md`, `getting-started/...`)
- Before/after expectations (screenshots for nav structure help)
- Links to existing pages that should be updated vs created
- Whether translations / locale folders are in scope

Avoid vague “improve the docs” issues without a definition of done.

### 3. Fund the issue on Lightning Bounties

1. Copy the GitHub issue URL.
2. On [app.lightningbounties.com](https://app.lightningbounties.com/), create a reward with that URL and amount in sats.
3. Choose a reasonable **lock time** so solvers can finish writing and get a review.

See also: [Create a GitHub issue and Submit a new reward](create-a-github-issue-and-submit-a-new-reward.md) and [Deposit Funds](deposit-funds.md).

### 4. Review like a docs PR

When reviewing:

- Check links, SUMMARY / sidebar entries, and spelling.
- Confirm the PR body includes `close #<issue-number>` so Lightning Bounties can attribute payment after merge.
- Merge to the branch GitBook (or your host) publishes from.

## For solvers: working on a docs bounty

### 1. Find open doc bounties

Browse [app.lightningbounties.com](https://app.lightningbounties.com/) or search GitHub issues that link Lightning Bounties. Prefer issues with clear file lists and no trophy/winner yet.

### 2. Fork, edit Markdown, open a PR

Typical flow (same as code):

```bash
git clone https://github.com/<org>/<docs-repo>.git
cd <docs-repo>
git checkout -b fix/docs-issue-123
# edit .md files, update SUMMARY.md / sidebar if needed
git add .
git commit -m "docs: describe change (closes #123)"
git push origin fix/docs-issue-123
```

Open a PR against the default docs branch. In the **PR description**, include:

```text
close #123
```

(Replace `123` with the issue number.)

### 3. GitBook-specific tips

- If the site uses GitBook Git Sync, mirror the repo’s folder structure; don’t invent paths outside SUMMARY.
- Add new pages to `SUMMARY.md` (or the project’s nav file) or they may not appear in the published TOC.
- Prefer relative links between docs pages.
- Keep screenshots under the repo’s asset folder (often `.gitbook/assets/`) and reference them with relative paths.

### 4. Claim after merge

Once the maintainer merges your PR and the issue is closed:

1. Log in to [app.lightningbounties.com](https://app.lightningbounties.com/) with GitHub.
2. Open the bounty → **Claim Reward** (PR must be merged into the default branch).
3. Withdraw sats via Lightning when ready: [Withdrawing Funds](../solving-a-bounty/withdraw-funds.md).

## Wiki platforms at a glance

| Platform | Host bounties via | Solver delivers |
|----------|-------------------|-----------------|
| GitBook (Git Sync) | GitHub Issues on synced repo | PR updating Markdown + SUMMARY |
| MkDocs / Material | GitHub Issues | PR to `docs/` |
| Docusaurus | GitHub Issues | PR to `docs/` or `blog/` |
| GitHub Wiki | Issues on main repo (wikis rarely take PRs) | Prefer moving content into a normal `docs/` folder for bounty-friendly PRs |
| Notion / Confluence only | Not Git-native | Export content to a GitHub docs repo first |

{% hint style="info" %}
**Tip:** If your wiki cannot accept pull requests, create a small GitHub `docs` mirror and treat that as the bounty surface. Publish from Git when reviews land.
{% endhint %}

## Related guides

- [Working on a Bounty](../solving-a-bounty/working-on-the-bounty.md)
- [Finding Bounties to Solve](../solving-a-bounty/looking-for-a-project-to-get-rewarded.md)
- [Claim Reward Criteria & Troubleshooting](../solving-a-bounty/claim-reward-criteria-and-troubleshooting-guide.md)
