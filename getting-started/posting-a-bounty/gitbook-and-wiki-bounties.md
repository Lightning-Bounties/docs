---
description: How GitBook, wiki, and other Markdown documentation projects can post and solve bounties.
---

# GitBook and Wiki Bounties

GitBook, wiki, and other Markdown-based documentation projects can use Lightning Bounties when the work can be reviewed through a GitHub pull request. The core idea is simple: create a GitHub issue that describes the documentation change, attach a bounty to that issue, then review the contributor's pull request.

This works well for:

* Adding missing documentation pages or sections
* Improving unclear setup or troubleshooting guides
* Fixing broken links, outdated screenshots, or missing alt text
* Updating GitBook navigation in `SUMMARY.md`
* Editing Markdown pages that are mirrored from GitHub into a documentation site

## For bounty posters

### 1. Find the GitHub source file

Open the page that needs work and use its "Edit on GitHub" link when available. For GitBook projects, the public page usually maps to a Markdown file in the project's GitHub repository.

If the change needs a new page, identify the right folder and whether `SUMMARY.md` must be updated so the page appears in the GitBook navigation.

### 2. Create a focused GitHub issue

Write the issue so a contributor can complete the work without guessing. Include:

* The public documentation URL
* The GitHub file or folder that should change
* The expected outcome
* Any required screenshots, examples, or links
* The acceptance criteria for review

For example:

```markdown
Title: Add a troubleshooting section for wallet invoice failures

Please add a short troubleshooting section to:
getting-started/solving-a-bounty/withdraw-funds.md

The section should explain:
- what to check when an invoice is rejected
- how to retry with a new invoice
- when to contact support

Acceptance criteria:
- The wording is beginner-friendly
- The page keeps the existing heading structure
- Any new links are tested
```

### 3. Submit the issue to Lightning Bounties

After creating the GitHub issue, open [app.lightningbounties.com](https://app.lightningbounties.com/), submit the issue URL, choose the reward amount in sats, and set the bounty duration.

Use a reward that matches the scope. Small wording or link fixes should stay small; new pages, screenshots, and multi-page guides should be rewarded higher because they require more review and testing.

### 4. Review the pull request

When a contributor opens a PR, check that it:

* Changes the expected Markdown files only
* Updates `SUMMARY.md` if a new GitBook page was added
* Keeps headings and links consistent with the surrounding docs
* Includes `close #[issue-number]` in the PR description when required for reward claiming

Merge the PR only when the documentation change is complete and the bounty issue can be closed.

## For bounty solvers

### 1. Confirm the source and scope

Before editing, open the bounty issue and the current documentation page. Check whether the change is a small edit, a new section, or a new page.

For GitBook projects, also check `SUMMARY.md` when adding or moving pages.

### 2. Make the documentation change

Use the GitHub web editor for small changes, or fork and clone the repository for larger changes. Keep the PR focused on the bounty issue.

Good documentation PRs usually include:

* Clear Markdown formatting
* Tested internal and external links
* Descriptive image alt text when images are added or edited
* A short explanation of what changed and why

### 3. Open a pull request

In the PR description, explain the change and include `close #[issue-number]` if the bounty instructions require it. This links the PR to the GitHub issue and helps Lightning Bounties verify the completed work.

### 4. Claim the reward after merge

After the PR is merged, return to Lightning Bounties, open the bounty, choose "Claim Reward", and enter the merged pull request number. The platform checks the GitHub issue and pull request before releasing the sats.

## Quick checklist

For posters:

* The GitHub issue links to the exact docs page or file
* The bounty scope is clear and reviewable
* The reward amount matches the effort
* The acceptance criteria explain what "done" means

For solvers:

* The issue is still open before starting
* The PR changes only files needed for the bounty
* New GitBook pages are added to `SUMMARY.md`
* The PR description includes the required issue-closing syntax
