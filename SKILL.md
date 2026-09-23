---
name: onboarding-pack
description: |
  Write and maintain the onboarding document a newcomer actually needs on
  day one: what the project is and who it serves, the exact commands that
  produce a working setup, a map of where things live with the authoritative
  source named, the unwritten rules insiders stop noticing, and who decides
  what — readable in ten minutes, updated as part of the change that
  invalidates it. Use when someone (a human, a new agent session, or the
  user themselves in three months) joins a project, when the user asks for
  a README/handover/onboarding doc, when the same questions keep being
  answered from memory, or when undocumented conventions keep tripping
  people up.
  触发词：上手文档 / 项目介绍 / 新人指南 / onboarding。
license: MIT
metadata:
  version: "0.1.0"
---

# Onboarding Pack: the month of asking around, prepaid

## When to use

Use when someone (or a new agent session) starts on a project: new hire, new contractor, new contributor, fresh assistant context. Use before taking leave. Not for HR paperwork or company-wide policy docs.

The expensive onboarding time is spent discovering unwritten rules, not
running install commands. This pack writes those rules down once, where the
next person will find them.

## Rules

1. **Write for day one.** Every section answers a question the newcomer has
   in their first hours; history and architecture debates stay out.
2. **Name the authoritative source for every contested area.** Most projects
   carry competing sources of truth (two configs, three trackers); the map
   section says which one wins, so the newcomer stops guessing.
3. **Unwritten rules are the payload.** The section lists the constraints
   that are obvious to insiders and invisible to newcomers — the script
   that must never run here, the check that always comes first, the thing
   that is deprecated but still load-bearing.
4. **Ten minutes, end to end.** If reading the pack takes longer, it has
   drifted into reference documentation; split or cut.
5. **Update is part of the change.** A change that invalidates the pack and
   leaves it stale is an incomplete change — the pack is updated in the
   same edit that breaks it.
6. **Dated.** The pack carries its last-review date so readers can judge
   staleness instead of trusting blindly.

## Steps

1. **Discover.** Survey the project as a newcomer would: entry documents,
   directory layout, scripts, configs, recent changes. Note every point
   where you had to guess.
   Done when: the guess list covers every stop a newcomer would hit.
2. **Draft the five sections.** What & why; run it (exact commands, in
   order); map (authoritative sources named); unwritten rules; who & where.
   Done when: all five sections exist and the unwritten-rules list names
   every guess from discovery.
3. **Verify by running.** Execute the run-it commands fresh; fix the pack
   where reality disagrees.
   Done when: the commands produce the claimed result in this run.
4. **Date and place.** Stamp the review date and put the pack where day-one
   eyes land (repo root or the project's obvious entry doc).
   Done when: the pack is reachable from the project's front door.

## Done when

A newcomer with zero context can run the project from the pack's commands,
name the authoritative source for every contested area, list the unwritten
rules, and find the owners — all within ten minutes of reading, and the
pack's date proves how current it is.

## Gotchas / 常见坑

- The pack's author knows too much to test it; run it against a fresh reader (human or agent) — untestable steps are where onboarding fails.
- Access items (repos, dashboards, keys) age fastest: date them and name their owner.
- 'Ask X if stuck' without X's availability or timezone is a dead end on day one.
