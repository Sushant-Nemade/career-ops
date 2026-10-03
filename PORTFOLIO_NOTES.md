# Portfolio Notes

## Project context

This repository is a personal portfolio fork of [career-ops](https://github.com/career-ops-hq/career-ops), an open-source, local-first AI job-search agent.

**Upstream:** https://github.com/career-ops-hq/career-ops  
**Fork owner:** Sushant-Nemade  
**Purpose:** preserve the upstream implementation while maintaining a clearly documented portfolio copy for experimentation, evaluation, and future contributions.

## Engineering focus

This project is valuable as an applied AI systems example because it combines:

- Human-in-the-loop agent workflows rather than autonomous application submission.
- Structured job evaluation and evidence-based profile matching.
- Local-first handling of candidate data.
- Document generation and validation pipelines.
- Multiple AI CLI backends and configurable workflows.
- Explicit safety boundaries around untrusted job-posting content.
- Operational tooling such as health checks, tracking, and pattern analysis.

## Architecture at a glance

```
Job URL / Job Description
          |
          v
   Retrieval + Validation
          |
          v
   Structured Evaluation
     /       |        \
  Fit      Risks    Evidence
    \       |        /
          v
   Human Review Gate
          |
     +----+----+
     |         |
     v         v
  Tailored   Interview /
  Documents  Follow-up
     |
     v
 Local application record
```

The human remains the final decision-maker. The system should be treated as an assistant that produces evidence, drafts, and structured recommendations—not as an autonomous applicant.

## Portfolio contribution policy

Changes made in this fork should favor:

1. Reproducibility and clear documentation.
2. Tests and validation before workflow changes.
3. Minimal exposure of personal candidate data.
4. Explicit attribution to upstream authors.
5. Small, reviewable commits.
6. No fabricated candidate experience or application claims.

The original MIT license and upstream copyright notice are retained.
