# Handdrawn Route Map Card Skill

Open Skill for turning a city, food, travel, hiking, life checklist, study plan, creator workflow, AI workflow, or SOP topic into a Xiaohongshu-style hand-drawn route-map card brief.

中文一句话：把城市、美食、旅行、生活清单或工作流，整理成小红书风格手绘收藏地图卡。

## Search Keywords

English keywords:

`handdrawn route map`, `Xiaohongshu map card`, `RedNote visual card`, `travel map brief`, `food map card`, `workflow map`, `life checklist card`, `watercolor route map`, `AI image prompt`.

中文关键词：

`手绘收藏地图`, `小红书手绘地图`, `手绘路线图`, `美食地图`, `旅游路线图`, `生活清单地图`, `工作流说明书地图`, `水彩地图卡`, `AI 作图提示词`.

## Why This Exists


A save-worthy map card is not a generic poster. It needs a clear route, 5-7 nodes, side collage, mini box, bottom note, and quality gate.
This Skill turns a topic into a structured generation brief or visual plan for a hand-drawn route-map card.

## What It Can Do

- content structure: title, subtitle, nodes, side box, bottom note
- image-generation brief
- quality checklist
- caption pattern when needed
- notes about verification if the map contains real places or current facts

## Best Inputs

- topic or route
- scene type: city food, travel itinerary, hiking, life checklist, or workflow manual
- 5-7 nodes, if known
- style preference
- whether the user wants image generation or just a brief

## Workflow

- Classify the topic into a map card type.
- Build a 5-7 node route or checklist.
- Create side collage subjects, mini box, and bottom note.
- Avoid fake precise navigation, prices, hours, or official claims.
- Return a generation brief and quality checklist.
- If image generation is available, generate and review the file; otherwise return the brief.

## Output Contract

Default output:

1. Scope and assumptions
2. Input reading
3. Main judgment
4. Structured table or checklist
5. Recommended next action
6. Boundary notes

For detailed rules, see `references/workflow-rules.md`.

## Example Prompt

```text
Use $handdrawn-route-map-card for this task:
做一张图文发布工作流地图。步骤：收集灵感、判断选题、写大纲、生成配图、发布检查、数据复盘。风格：奶油纸底水彩路线图。
```

## Example Output Shape

See `examples/sample-output.md` for a short sample.

## Open-Source Boundary

This standalone open version includes:

- reusable creator workflow instructions
- input and output contracts
- workflow rules
- example output
- Agent metadata
- MIT license

This standalone open version does not include:

- private platform credentials
- automatic publishing
- private analytics connectors
- scraping or monitoring
- guaranteed traffic, growth, sales, or viral outcomes
- copying another creator's content
- internal operating notes or private project context

## Repository Map

- `SKILL.md`: Agent entrypoint and workflow rules
- `agents/openai.yaml`: Agent display metadata
- `references/workflow-rules.md`: detailed workflow and quality rules
- `examples/sample-output.md`: sample input and output shape
- `LICENSE`: MIT license

## Recommended GitHub Description

> Open Skill for turning a city, food, travel, hiking, life checklist, study plan, creator workflow, AI workflow, or SOP topic into a Xiaohongshu-style hand-drawn route-map card brief.

## Suggested GitHub Topics

`handdrawn-map`, `route-map`, `xiaohongshu`, `rednote`, `visual-design`, `creator-tools`, `content-workflow`, `ai-image-prompt`, `open-source`

## License

MIT
