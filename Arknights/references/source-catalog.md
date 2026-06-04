# Arknights Source Catalog

Use this catalog to choose sources for main-game Arknights research. Prefer live lookup because operator data, banners, events, tier lists, and farming efficiency change frequently. For "latest" or "current" requests, reject stale sources unless they are clearly labeled as background context.

## Public Sources

| Source | URL | Best for | Login | Notes |
| --- | --- | --- | --- | --- |
| 明日方舟官网 | https://ak.hypergryph.com/ | Official announcements, events, news, limited operator previews, selected operator/profile material | No | Treat as primary for CN official announcements. Some pages are visual/JS-heavy, so cross-check details with wiki mirrors if text is sparse. |
| PRTS Wiki | https://prts.wiki/ | CN operator facts, skills, talents, modules, stages, enemies, systems, lore, events | No for reading | Strong default factual source. Editing/account features require login, but reading pages is public. |
| PRTS 干员分类 | https://prts.wiki/w/%E5%88%86%E7%B1%BB:%E5%B9%B2%E5%91%98 | Operator index and navigation | No | Useful for finding exact Chinese operator page names, including alternate forms. |
| BWiki 明日方舟 | https://wiki.biligame.com/arknights/ | CN operator pages, skills, modules, events, supplementary wiki content | No for reading | Good cross-check for PRTS, especially when one wiki page is stale or hard to parse. |
| Arknights Terra Wiki | https://arknights.wiki.gg/wiki/Operator | English operator facts, Global/CN availability context, lists, terminology | No | Prefer for English or Global-server answers. Check server availability before applying CN advice to Global. |
| Ark Hypr | https://www.arkhypr.com/ | Fast English data atlas: operators, enemies, recruitment, skins, banners, tier list | No | Homepage exposes update timestamp and indexed counts. Useful for active banners and quick Global-facing data. |
| Aceship Operator Details | https://aceship.github.io/AN-EN-Tags/akhrchars.html | Operator details, recruitment tags, older EN/CN data tooling | No | Useful as a supplementary database, but verify freshness; community reports have noted stale periods. |
| Myrtle | https://myrtle.moe/ | Operator database, tier lists, recruitment calculator, DPS charts, public tooling | Partly | Public browsing is available; account sync/history/progress features require connecting an account. |
| 明日方舟一图流 | https://ark.yituliu.cn/ | Stage efficiency, shop value, pull calculator, operator development survey | No | Record attribution and license/redistribution caveats. Many views are JS-heavy; use linked text snippets or browser inspection when needed. |
| 干员练度调查 | https://ark.yituliu.cn/survey/operators | Operator ownership/build-rate survey and cultivation statistics | No | Treat as usage survey, not objective strength. |
| 企鹅物流数据统计 | https://penguin-stats.cn/ | Drop rates, stage/material statistics | No | SPA requires JavaScript. Use as statistical support for farming advice; pair with efficiency calculations. |
| ark-nights.com 干员培养表 | https://cn.ark-nights.com/?locale=zh_CN | Material planning, promotion/mastery/module cost tracking | No | Useful for cultivation totals and ArkPlanner/Penguin/MAA-style inventory import compatibility notes. |
| ArkDPS | https://ark-dps.com/ | DPS calculations and model-based strength comparison | No | SPA requires JavaScript. Treat as model output, not universal ranking. State assumptions when citing. |
| Bilibili UOEP 强度图 | https://www.bilibili.com/opus/1178985380546871297 | Recent CN community/model-based strength trends | Usually no for reading | Source is authored and subjective/model-based. Record edit date and author; avoid treating it as official. |
| MAA 自动战斗文档 | https://maa.plus/docs/zh-cn/manual/introduction/copilot.html | How to use MAA copilot/作业, supported workflows, JSON or code import behavior | No | Use for explaining MAA workflow; not a stage guide by itself. |
| PRTS Plus 作业站 | https://prts.plus/ | MAA-compatible copilot jobs/作业 | No for browsing basics | JS-heavy. Job availability and quality vary; advise users to inspect operator requirements and comments. |
| 明日方舟作业帮 | https://maliut.space/arknights/ | Community stage job search | No | Supplementary copilot/job source; verify stage and operator requirements. |
| TapTap / 游民星空 / 游侠 / 九游 / other guide portals | Varies | Stage guides, beginner guides, event summaries | Usually no | Quality varies. Use only as secondary/community guide sources and verify dates. |

## Login Or Account-Bound Sources

| Source | URL | Requires login/account binding for | Notes |
| --- | --- | --- | --- |
| 森空岛 | App / official community | Personal Arknights account data, owned operators, skins, resources, resource planning, official community account features | Requires Hypergryph account/phone login and likely game-account binding. Do not ask for passwords, SMS codes, cookies, or tokens. Ask the user for screenshots/exported text instead. |
| Krooster | https://www.krooster.com/ | Roster, Collection, Planner, Profile, Import | Public tools include Recruitment, Headhunting, Level Costs. Personal data features require login. Public profile links can be used if the user provides one. |
| Myrtle | https://myrtle.moe/ | Account sync, personal pull history, player profile/progress features | Public database/tools are usable; connected-account features need user action outside Codex. |
| ArkPRTS | https://arkprts.ashlen.top/about | Private account data fetching | Can fetch public and private Arknights data. Private use involves credentials/tokens; default to public data or user-provided exports only. |
| Bilibili / NGA / TapTap | Varies | Posting, commenting, following, full app search, some community content | Reading many pages is public, but complete access may require login. Treat community opinions as dated, subjective sources. |

## Routing Defaults

- Operator fact sheet: official site if relevant, then PRTS and BWiki; use Terra Wiki or Ark Hypr for English/Global.
- Build priority: PRTS/BWiki facts plus Bilibili UOEP, ArkDPS, Yituliu survey, Myrtle/Ark Hypr tier lists when available.
- Material farming: ark-nights.com or Krooster for needed totals, Penguin Stats and Yituliu for farming efficiency.
- Current banners/events: official site first, Ark Hypr/PRTS second.
- Stage clears: PRTS/BWiki mechanics first, then current community guides; use MAA/PRTS Plus for copilot jobs.
- Personal box planning: accept user-provided roster screenshots, text, Krooster public profiles, or exports; never request private login material.

## Freshness Defaults

- Current/today banners, events, shops, and farming rotations: use official sources or pages updated within 7 days.
- Latest rankings, tier lists, DPS summaries, and cultivation recommendations: prefer sources updated within 30 days; if the newest credible result is older, state the gap before summarizing.
- Current patch analysis: require sources published after the patch or explicitly covering the same new operators/modules/event.
- Named month/year requests: keep sources inside the requested month/year unless the user asks for broader context.

## Maintenance Notes

Store durable new Arknights source discoveries in this file, not in scratch notes or only in conversation. Use the existing public/login split:

- Add public, no-login resources to `Public Sources`.
- Add login-gated, account-bound, app-only, private-profile, cookie/token, or credential-adjacent resources to `Login Or Account-Bound Sources`.
- Prefer canonical home or hub URLs over transient search/result URLs.
- Include a freshness signal in `Notes` when useful, such as "updates monthly", "homepage shows last update", "Bilibili video series", or "verified YYYY-MM-DD".
- Skip one-off reposts, low-quality SEO pages, expired event-only articles, and sites that only mirror an existing source without extra value.
- If write access is unavailable, report the candidate row to the user so it can be added later.
