---
name: arknights-research
description: Query and synthesize Arknights operator information, character rankings, stage guides, farming advice, and operator development recommendations. Use when Codex needs current Arknights main-game facts, Chinese or Global operator data, tier-list context, material planning, stage strategies, or source routing for sites such as PRTS, BWiki, Penguin Stats, Ark Hypr, ArkDPS, Krooster, or Skland.
---

# Arknights Research

## Overview

Use this skill to answer questions about the main Arknights game only. Do not use it for Arknights: Endfield content.

Default to Chinese responses and CN-server context. Switch to English or Global-server sources when the user asks for Global, EN, JP/KR release timing, or English names.

## Query Workflow

1. Classify the request before searching:
   - Operator facts: profile, rarity, class, branch, skills, talents, modules, base skills, skins, voice, artist, lore.
   - Ranking or development advice: tier lists, whether to build, mastery/module priority, reroll/new-player value.
   - Farming or planning: promotion costs, mastery/module materials, best farming stages, shop efficiency.
   - Stage or mode guide: clear strategy, enemy/stage mechanics, MAA copilot jobs, IS/RA/CC mode advice.
   - Current game information: active events, banners, new operators, announcements.
   - Personal account or box advice: roster-specific plans, owned operators, depot materials.
2. Read `references/source-catalog.md` when you need source routing, login notes, or a reminder of which sites are appropriate.
3. Establish the user's requested time frame before searching. For relative wording such as "latest", "current", "today", "now", "this month", or "current patch", use the current absolute date from system context or a local `date` command.
4. Use live web lookup for current facts, rankings, banners, drop rates, and guides. Do not rely on memory for current Arknights data.
5. Prefer primary or stable factual sources for factual claims, then add evaluative/community sources for advice.
6. Separate factual information from subjective recommendations in the answer.
7. Include source names, links, and visible update dates or crawl/read dates when available.

## Time Alignment

Align source freshness with the user's requested time window. Do not answer a "latest" or "current" request from stale sources without explicitly saying that no fresh-enough source was found.

- For "today", "now", current banners, current events, or active shops, require an official date range that includes the current date or a source updated within 7 days.
- For "latest" rankings, strength lists, tier lists, cultivation recommendations, or meta summaries, prefer sources updated within 30 days of the current date. If none are available, use the newest credible source only as a fallback and state the exact age and limitation.
- For "this month" or a named month, keep sources within that calendar month unless the user accepts older context.
- For "current patch/version", prefer sources updated after that patch or sources that name the same event/operator set. Do not silently substitute the previous patch.
- For historical requests, match the requested date, month, season, or year instead of using newer sources.
- When sources disagree, prefer the freshest source only if it is also credible and aligned with the requested server; otherwise explain the tradeoff.

## Source Selection

For operator facts, prefer official pages, PRTS, BWiki, Arknights Terra Wiki, Ark Hypr, Aceship/Arkntools-style databases, then secondary guides.

For rankings, DPS, and cultivation advice, treat every source as contextual rather than definitive. Cross-check at least two sources when possible, especially for high-impact build recommendations. State the source's basis, such as DPS model, community tier list, usage survey, or author opinion.

For farming, combine material cost planners with drop-rate or efficiency sources. Prefer Penguin Stats and Yituliu for stage efficiency, and use ark-nights.com or Krooster-style planners for material totals.

For stage guides, prioritize current activity-specific guides and PRTS/BWiki mechanics pages. Use MAA/PRTS Plus only for automated "copilot" job discovery or when the user asks for "作业", "抄作业", "挂机", or MAA-compatible clears.

For current events or banners, check the official Arknights site first, then PRTS/Ark Hypr/community summaries if the official page lacks detail.

## Source Catalog Maintenance

When live research uncovers a useful Arknights source that is not already in `references/source-catalog.md`, decide whether it should become reusable skill knowledge.

Add or update the catalog only when the source is likely to be useful again, such as an official page, maintained database, recurring tier-list author, material planner, drop-rate tool, event guide hub, or account/roster tool. Do not add one-off low-quality reposts, expired event-only pages, search result pages, or sources that duplicate existing entries without adding clear value.

Save durable source updates in `references/source-catalog.md` inside this skill. Put public sources under `Public Sources`, and sources that require login, account binding, private profiles, cookies, tokens, or app-only access under `Login Or Account-Bound Sources`. Include the site name, canonical URL, best use case, login requirement, freshness signal, and a short caution about reliability or scope.

If the skill directory is not writable in the current environment, tell the user which source should be added and provide the exact row or note to insert. Do not store persistent source catalog updates in temporary files or only in the chat transcript.

## Answer Rules

- Do not present a single "强度榜" as objective truth. Explain scenario fit, account stage, mode, and investment cost.
- When recommending whether to build an operator, include at minimum: role/niche, general priority, mastery/module notes if relevant, and when to skip or delay.
- When answering personal box questions, ask the user to provide roster/depot text, screenshot, or an exported public profile. Do not request account passwords, cookies, tokens, SMS codes, or private API credentials.
- If a source requires login or account binding, say so and offer public alternatives.
- If sources conflict, summarize the conflict and explain which source is more suitable for the user's situation.
- Avoid copying large tables or long guide text. Summarize and link to the original page.

## Useful Search Patterns

- `干员名 PRTS 明日方舟 技能 模组`
- `干员名 明日方舟WIKI BWiki`
- `干员名 Arknights Terra Wiki operator`
- `干员名 明日方舟 值得练 专精 模组`
- `明日方舟 干员强度图 2026`
- `明日方舟 干员强度榜 2026年5月`
- `明日方舟 当前版本 干员强度榜`
- `site:bilibili.com 明日方舟 干员强度图`
- `site:bilibili.com 明日方舟 干员强度榜 2026年5月`
- `材料名 明日方舟 掉落 企鹅物流 一图流`
- `关卡名 明日方舟 攻略 MAA 作业`
- `明日方舟 官网 公告 活动 干员`
