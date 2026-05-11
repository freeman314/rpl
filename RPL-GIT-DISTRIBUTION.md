# RPL Git Distribution Plan

How to package RPL Harness so it can be shared with other people without exposing any private user instance.

## Distribution Principle

RPL should be distributed as two things:

1. **Public Harness** — reusable system files, skills, templates, rituals, and examples without personal data.
2. **Private User Save** — one person's memory, profile, quests, evidence, financial models, images, and session history.

The public Git repository must contain the Harness. It must not contain any real user's save unless that user explicitly publishes an anonymized example.

## Public Repository Contents

Recommended public structure:

```text
rpl-harness/
  README.md
  RPL-CONCEPT.md
  RPL-HARNESS.md
  RPL-DATA-BOUNDARIES.md
  RPL-ONBOARDING-RITUALS.md
  RPL-LIFE-COMPASS.md
  RPL-HUMAN-JOURNEY.md
  RPL-GIT-DISTRIBUTION.md
  skills/
    rpl-onboarding/
    rpl-current-mirror/
    rpl-future-mirror/
    rpl-life-compass/
    rpl-quest-designer/
    rpl-weekly-mirror/
    rpl-season-review/
    rpl-freedom-number/
    rpl-independent-offer/
    rpl-memory-curator/
  templates/
    USER-MEMORY.template.md
    USER-PROFILE.template.md
    USER-QUESTS.template.md
    USER-EVIDENCE-LOG.template.md
```

## Private Files To Exclude

These files are private by default:

- `USER/`
- `RPL-MEMORY.md`
- `{USER}-*.md`
- `users/`
- `assets/`
- photos, generated personal images, financial calculations, session histories

This working folder uses `.gitignore` to protect the current private pilot instance.

## How People Use It

1. Clone the public Harness repository.
2. Create a private user save outside the public repo or inside ignored `USER/`.
3. Run one skill at a time through an agent or manually from the `skills/` folder.
4. Save personal outputs only in the private user save.
5. If a new reusable pattern appears, move only the anonymized rule back into the Harness.

## Publication Checklist

Before pushing to a public Git remote:

- scan `RPL-*.md` for personal names, locations, employers, photos, money amounts, health data, and private links;
- keep only system rules, rituals, formats, and anonymized examples;
- verify `.gitignore` excludes user saves and assets;
- create template files instead of publishing real profiles;
- check that a new person can understand how to start without reading a private pilot instance.

## North Star

The repository should feel like a small operating system for honest life reflection, not a productivity template pack.
