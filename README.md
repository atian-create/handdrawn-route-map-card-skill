# 小红书手绘路线图卡片 Skill

这是一个给小红书 / RedNote 图文创作者、旅行内容创作者、生活方式博主和 AI 作图使用者准备的开源轻量 Skill：它可以把一个城市、美食路线、旅行计划、徒步路线、生活清单或工作流，整理成一张“小红书风格手绘收藏地图卡”的生成 brief。

很多人想做手绘地图或清单图时，容易只写一句“帮我做一张好看的图”。结果出来的图经常有这些问题：

- 没有路线，只有装饰。
- 节点太多，画面拥挤。
- 标题、路线、侧边小图、提示框互相抢信息。
- AI 生成图看起来漂亮，但不是一张能收藏、能看懂、能发布的小红书图。

这个 Skill 解决的是“生图前的结构设计”：先把主题整理成标题、副标题、5-7 个节点、侧边元素、提示框、底部提醒和质量检查，再交给图像生成工具。

## 你下载后可以用它做什么

- 做城市美食地图，比如“长沙美食地图”“曼谷咖啡地图”。
- 做旅行路线图，比如“贵州 5 天游路线”“云南徒步路线”。
- 做生活清单图，比如“周末回血清单”“搬家准备清单”。
- 做工作流说明书图，比如“图文发布流程”“AI 内容复盘流程”。
- 生成一份可以直接交给 AI 作图工具的视觉 brief。
- 检查生成图是否标题可读、路线清楚、节点数量正确、没有虚假信息。

## 适合谁

- 想做小红书收藏型图文，但不会组织画面的人。
- 想用 AI 生成手绘地图、手绘清单、流程卡的人。
- 做旅行、美食、本地生活、学习计划、工作流内容的人。
- 想把复杂流程变成一张更容易保存的图的人。
- 给客户做图文视觉方案，希望先有稳定 brief 的设计/运营同学。

## 为什么这个 Skill 值得单独装

普通 AI 作图提示词往往只描述风格，比如“奶油纸、水彩、可爱”。但一张能用的小红书图，还需要清楚的信息结构。

这个 Skill 会固定输出：

1. 中文主标题。
2. 一句副标题。
3. 5-7 个路线节点或清单步骤。
4. 左侧/周围的物件拼贴。
5. 右侧提示框。
6. 底部收藏提醒。
7. 生成图质量检查。

它适合先把图“想清楚”，再去生图。

## 3 分钟上手

把这个仓库里的 `SKILL.md` 放到你的 Agent Skill 目录，然后这样问：

```text
用 handdrawn-route-map-card 做一张小红书手绘路线图。
主题：图文发布工作流地图
节点：收集灵感、判断选题、写大纲、做配图、发布检查、数据复盘
风格：奶油纸底、水彩路线图、手写标签
输出：先给我生图 brief 和质量检查表
```

## 你会拿到什么结果

默认输出会包括：

- 内容结构：标题、副标题、节点、侧边元素、提示框、底部提醒。
- 图像生成 brief。
- 硬性避免项，比如不要虚假价格、不要假导航、不要过多小字。
- 质量检查表。
- 如需要，还可以补一段小红书正文和标签。

## 公开版边界

这个开源版不验证实时门票、营业时间、交通、价格等信息。如果涉及真实旅行、餐厅或景点，它会提醒你这是“灵感图/路线草案”，不是精确导航。它不承诺图片生成一定完美，也不伪造官方信息。

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
