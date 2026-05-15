# Team Submission

## Team

- Team name:
- Participants:
- Wiki / project name:

## Wiki Overview

One-paragraph description of what your LLM Wiki does and how it self-improves.

- Domain or data sources:
- Primary use case:
- What makes it stand out:

## The Three Operations

### Ingest

- What goes in (documents, conversations, runs, ...):
- How it is captured (`cognee.remember(...)`, custom pipeline, ...):
- Code entry point:

### Query + Self-improve

- How users query the wiki:
- Where feedback comes from (user rating, agent critic, eval, ...):
- How feedback updates the wiki (`SkillRunEntry`, edge re-weighting,
  graph rewrite, ...):
- Code entry point:

### Lint

- What "linting" means in your wiki (dedupe, conflict resolution, stale
  pruning, ...):
- How it runs (scheduled, on-write, on-demand):
- Code entry point:

## Self-Improvement Evidence

Show that the wiki actually got smarter. Concrete before/after beats prose.

### Baseline Run

- Query / task:
- Result:
- Score (your own metric, judge-readable):
- Recorded feedback:

```text
error_type:
error_message:
feedback:
success_score:
```

### Improved Run

- Query / task:
- Result:
- Score:
- What changed in the wiki between runs:

```text
Before:

After:
```

## Architecture

Short diagram or bullet list of components. Call out where Redis and Cognee
sit.

```text
[ingest source]  ->  [cognee.remember]  ->  [knowledge graph]
                                              |
                                              v
                                       [Redis cache / session]
                                              |
                                              v
                                       [recall / agent loop]
                                              |
                                              v
                                       [feedback -> improve]
```

## Agents / Skills (if any)

If you used skill packs or multi-agent roles:

```text
Skill path(s):
Roles:
  - Ingestor:
  - Querier:
  - Linter:
  - Critic:
```

## Reproduction

Commands to reproduce your demo:

```bash
# paste commands here
```

Environment variables required:

```text
LLM_API_KEY
REDIS_URL
# add anything else your wiki needs
```

## Demo

- Live demo link (Loom, YouTube, etc.) or local instructions:
- 3-minute pitch outline:

```text
1. Problem / idea
2. Ingest demo
3. Query demo (before improvement)
4. Self-improve step
5. Query demo (after improvement)
6. What is next
```

## Links

- Repo:
- Slides / writeup:
- Anything else:
