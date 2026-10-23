# Profile maintenance

## Contributions

- Keep the Open Source Highlights table in reverse chronological order, newest first.
- Include completed contributions only. Omit open proposals until the work merges or ships; reports
  and proposed fixes resolved by upstream work may be credited with accurate attribution.
- Verify completion from current upstream evidence before drafting an entry. An open, parked, draft,
  or approved PR alone is not a completed contribution; do not publish it with a proposed status.
- Verify dates from the linked sources. Use the merge date for merged work, the release date for
  work shipped without merging the submitted PR, and the confirmed transfer date for transferred
  projects. Use the latest completed contribution date when one row covers multiple contributions.
- Add contributions to the existing table. Preserve concise descriptions, source links, project
  icons, and accurate status labels. Use the same emphasis as the other rows.
- Write each description as a short, concrete story. Start with the observed problem or contribution
  and make its consequence clear, then explain the action and result in chronological order. Name
  who benefits and what becomes safer, easier, faster, or possible; briefly explain an unfamiliar
  project's purpose when readers need it to understand the benefit. Use familiar language and retain
  technical terms only when they explain what failed or changed. Omit implementation and validation
  details that readers can find in the linked sources.
- Vary openings to suit the evidence: lead with a failure users encountered, its trigger, the
  investigation, or the contribution. Avoid repeating the same lead-in across nearby entries.
- Ground impact in linked evidence. Explain the practical benefit of version or dependency changes
  instead of ending at "updated" or "fixed." Distinguish delivered outcomes from expected benefits;
  do not invent adoption, savings, prevented incidents, or vulnerability remediation.

## Delivery

- Keep upstream issue and PR evidence links in README entries for completed contributions. Do not
  put upstream issue or PR URLs, cross-repository references, or closing keywords in profile commit
  titles or bodies: GitHub can turn them into unwanted activity on upstream timelines. Describe the
  rationale in prose and point reviewers to the README evidence instead.
- Inspect the full commit message as well as the staged diff before publishing. Check contribution
  eligibility and unintended upstream references; removing a README entry later does not remove an
  existing timeline event.
- Publish requested profile updates after verification without another approval request. The user
  authorizes the task-owned commits and pushes for profile maintenance. Explicit instructions such
  as `local only` or `do not push` take precedence.
- Work on `main` and push to `origin/main`. Preserve unrelated changes, run applicable document
  checks, and read back the published README to verify delivery.
- Follow the shared
  [writing guide](https://github.com/Farmio-io/farmio-service/blob/master/WRITING.md),
  [commit guidance](https://github.com/Farmio-io/farmio-service/blob/master/AGENTS.md#commit-messages),
  and applicable
  [release workflow](https://github.com/Farmio-io/farmio-service/blob/master/GO_PROD.md). Use a
  local owner checkout when available.
