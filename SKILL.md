---
name: handdrawn-route-map-card
description: "Open Skill for turning a city, food, travel, hiking, life checklist, study plan, creator workflow, AI workflow, or SOP topic into a Xiaohongshu-style hand-drawn route-map card brief. Use when the user asks for handdrawn route map, Xiaohongshu map card, RedNote visual card, travel map brief, 手绘收藏地图, 小红书手绘地图, 手绘路线图, 美食地图. This Skill uses user-provided material and public-safe reasoning only; it does not publish automatically, scrape private data, copy creators, or promise growth."
---

# Handdrawn Route Map Card

## Purpose

把城市、美食、旅行、生活清单或工作流，整理成小红书风格手绘收藏地图卡。

This is a lightweight standalone open Skill. It turns a repeated creator task
into a clear Agent workflow with inputs, checks, output shape, and boundaries.

## Use This For

- content structure: title, subtitle, nodes, side box, bottom note
- image-generation brief
- quality checklist
- caption pattern when needed
- notes about verification if the map contains real places or current facts

## Do Not Use This For

- automatic publishing
- private account login
- private data extraction
- guaranteed traffic, growth, sales, or viral outcomes
- copying another creator's exact wording, identity, images, or claims
- making claims that the user's material does not support

## Inputs

- topic or route
- scene type: city food, travel itinerary, hiking, life checklist, or workflow manual
- 5-7 nodes, if known
- style preference
- whether the user wants image generation or just a brief

If the input is incomplete, proceed with a first-pass version and mark
assumptions. Ask only the smallest necessary follow-up when the missing detail
would materially change the result.

## Workflow

Read `references/workflow-rules.md` when the task needs the full rule set.

- Classify the topic into a map card type.
- Build a 5-7 node route or checklist.
- Create side collage subjects, mini box, and bottom note.
- Avoid fake precise navigation, prices, hours, or official claims.
- Return a generation brief and quality checklist.
- If image generation is available, generate and review the file; otherwise return the brief.

## Output Contract

```markdown
## 1. Scope And Assumptions

## 2. Input Reading

## 3. Main Judgment

## 4. Working Table Or Checklist

## 5. Recommended Next Action

## 6. Boundaries
```

## Quality Bar

- Be specific and operational.
- Prefer a small usable output over a broad lecture.
- Explain why each recommendation fits the user's material.
- Mark weak evidence instead of pretending certainty.
- Do not promise results.
- Do not copy another creator's protected expression or personal story.

## Tone

Write in the user's language. For Chinese creator tasks, default to clear,
practical Chinese.

## Public Boundary

Keep examples generic. Do not include internal thread IDs, private file paths,
unpublished customer material, private account data, or internal product notes.
