---
name: x-content-studio-cn
description: Research, write, review, visually package, and retrospectively analyze Chinese X posts for AI, technology, finance, crypto, and economic commentary. Use for daily X posts, topic scans, quote posts, tutorials, draft de-AI editing, visual plans, or performance review. Do not use for direct account publishing or Xiaohongshu-only operations.
---

# Chinese X Content Studio

Create evidence-based Chinese X content and return the editorial deliverable in natural Chinese unless the user requests another language.

## Workspace Context

The workspace uses non-ASCII directory names. Keep this entrypoint ASCII-only and resolve the live paths by these stable prefixes, leaf names, and roles. Inspect before reading; do not create translated duplicate directories.

- Top-level directories beginning `01-` and `02-`: plans and drafts for the current content weeks.
- The top-level hot-research system directory, identifiable as the ancestor of the external-tool `x-tweet-fetcher/`: leads, evidence, and external tools.
- The `x-tweet-fetcher/` directory under that research system's external tools: public X post retrieval. Its availability does not grant account-writing access.
- The project tool-registry JSON inside the top-level tool library: tool status and limitations.
- The top-level content-operations directory: publication records, tags, rankings, and metrics.

Read only the resources needed by the selected mode. Keep new content in the existing local content system with sources, limitations, and review status.

## Route the Request

Select one mode and read only the references listed for that mode:

- `today-content`: inspect the current weekly plan, recent drafts, and published records before selecting a non-duplicate angle. Read [research and evidence](references/research-and-evidence.md), [Chinese voice](references/chinese-voice.md), [post formats](references/post-formats.md), and [visual system](references/visual-system.md).
- `topic-or-tutorial`: define what the reader should understand or be able to do. Read [research and evidence](references/research-and-evidence.md), [Chinese voice](references/chinese-voice.md), and [post formats](references/post-formats.md). Read [visual system](references/visual-system.md) only when the user asks for visuals or a complete text-and-visual package.
- `quote-or-comment`: fetch the source post and enough context to separate its claim from the author's judgment. Read [research and evidence](references/research-and-evidence.md), [Chinese voice](references/chinese-voice.md), and [post formats](references/post-formats.md).
- `review-and-revise`: diagnose facts, angle, structure, voice, and visuals before revising. Read [Chinese voice](references/chinese-voice.md), [post formats](references/post-formats.md), and [review and metrics](references/review-and-metrics.md). Read [research and evidence](references/research-and-evidence.md) only when claims need verification.
- `post-publication-review`: use the user-provided X URL and platform data. Read [review and metrics](references/review-and-metrics.md).

## Shared Editorial Rules

Default: one complete Chinese Blue-verified X post, not a thread. Preserve the user's real judgment and voice. Never invent identity, experience, results, testing, market data, or platform-algorithm claims. Treat third-party operating advice as a hypothesis unless reliable evidence supports it.

## Research and Evidence

For current or factual claims, follow [research and evidence](references/research-and-evidence.md). Prefer primary sources, separate confirmed facts from inference and opinion, record unknowns, and include source URLs and verification dates.

## Draft and Visual Package

Use [Chinese voice](references/chinese-voice.md) and [post formats](references/post-formats.md) for the selected format. Read [visual system](references/visual-system.md) only when the request includes visuals or a complete content package. Visuals must add evidence or explanation. Never present generated imagery as a real interface, event, or dataset.

## Save and Review

Save requested work in the appropriate project content directory with sources, claim boundaries, visual notes, and status. For pre-publication checks or post-publication learning, follow [review and metrics](references/review-and-metrics.md). Treat missing platform metrics as unknown, not zero.

Status: pending human review; unpublished.

## Permission Boundary

Researching public pages and reading local project files does not grant account access.

This skill must never perform post, reply, like, repost, follow, or direct-message actions.

Direct publishing is out of scope and requires a separate account-writing tool plus separate authorization.

Do not infer permission to log in, read cookies, or schedule account actions. Never save authentication tokens in project files.

## Failure Handling

If an X source or search backend is unavailable, use ordinary web research or ask the user for the source and state the missing context. If a tutorial cannot be verified, label it as documentation-checked or pending verification instead of claiming hands-on testing. If reliable data or real visuals are unavailable, explain the limitation and use a clearly labeled mechanism diagram or concept image instead of fabricating evidence.
