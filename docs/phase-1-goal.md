# Phase 1 Goal — First Playable Yuldopunk 2040

## Objective

Create and publish the first directly playable web version of `율도펑크2040`.

The first milestone is not a pitch deck, design mockup, or vague MVP. It is a coherent browser-playable experience that Minho can play himself and later share with Beomseok.

## Product Identity

- **Title**: `율도펑크2040`
- **Subtitle**: `서울 밖 50인의 AI 자급자존 생존 시뮬레이션`
- **Genre**: realistic near-future Korean community survival simulation
- **Setting**: South Korea outside Seoul, year 2040
- **Scale**: AI-assisted community of 50 people or fewer

## Critical Scope Decision

The first playable version focuses on Episode 1: `첫 겨울까지 180일`.

The player is not operating a completed town yet. The player is not only selecting a site. The player is the founding/planning/build team trying to prepare a 50-person AI-assisted settlement before the first winter arrives.

## Core Episode Premise

`이미 후보지는 정해졌다. 50명이 들어오기로 했다. 겨울 전까지 최소 생존 가능한 마을을 만들어야 한다. 돈, 시간, 인허가, 전기, 난방, 사람의 합의가 모두 부족하다.`

## Primary Player Goal

Prepare a settlement that can pass the first winter survival test within 180 days.

## Required Play Loop

1. Review the current settlement situation.
2. Choose and place build modules on a village board.
3. Spend budget, days, labor, and infrastructure capacity.
4. Watch readiness, winter survivability, budget, build progress, and social consent change immediately.
5. Trigger construction-phase events.
6. Adapt the plan.
7. Save snapshots and compare alternative settlement plans.
8. Reach day 180 and see whether the community survives the first winter test.

## Required Primary Scores

- `입주 준비도`
- `겨울 생존성`
- `예산 건전성`
- `공사 진행률`
- `사회 합의`

## Required Secondary Indicators

- `인허가 리스크`
- `전력 안정성`
- `난방 안정성`
- `통신 안정성`
- `AI 의존도`
- `시공 복잡도`
- `지역 민원 위험`
- `현실성 레벨`

## Required Playable Content

- One complete scenario: `강원 산기슭 10가구, 첫 겨울까지 180일`
- A visible village board or planning map
- At least 10 buildable modules
- At least 8 construction/founding events
- Immediate score changes when modules are added, removed, or changed
- A day, budget, and progress system
- Snapshot save and comparison
- A final day-180 winter readiness result
- A Korean `AI 이장 보고서` that summarizes current risks and next actions

## Example Modules

- `주거 블록`
- `단열 업그레이드`
- `공용 식당`
- `작업실`
- `서버실`
- `태양광`
- `배터리`
- `히트펌프`
- `보일러 백업`
- `도로/동선`
- `창고`
- `통신 타워`
- `방풍림/녹지`

## Example Construction Events

- `폭설 예보가 앞당겨짐`
- `공사비 15% 상승`
- `인허가 보완 요청`
- `전력 인입 공사 지연`
- `배터리 납기 지연`
- `지역 주민 민원`
- `공용시설 우선순위 갈등`
- `AI 운영 시스템 장애`
- `난방 설계 재검토`
- `예산 후원 조건 변경`

## Design Direction

- The first screen should be the playable game screen, not a marketing landing page.
- The interface should feel like a board-game-like simulation, not a CAD tool and not a static dashboard.
- It should be realistic but playful.
- It should feel Korean, near-future, practical, slightly tense, and a little absurd.
- Avoid generic sci-fi dashboards.
- Avoid making it only a pretty village builder.
- The central emotional loop is: "Could we actually live like this, and what breaks first?"

## Out of Scope

- Long-term post-completion town management
- Real architectural, legal, or engineering claims
- Login or account systems
- Paid API dependencies
- Real-time multiplayer
- Pitch deck or presentation page as the main result
- Static calculator with no play loop
- Wireframe-only milestone

## Deployment Goal

The final Phase 1 result must have a public URL.

Choose the simplest appropriate deploy path:

- GitHub Pages if the app can remain static.
- Vercel if a React, Next, or Vite app is more appropriate.

If deployment authentication is unavailable, create the complete local playable app and clearly state the exact deployment blocker and next required user action.

## Definition of Done

- Minho can open a URL and play a complete run.
- The game has a clear objective: prepare for the first winter within 180 days.
- The player can make meaningful tradeoffs between budget, time, survival, infrastructure, and social consent.
- The product has enough interaction that Minho can play for at least 10 minutes and naturally think, "I want to try a different plan."
- The experience is clearly `율도펑크2040`, not a generic town planner.

