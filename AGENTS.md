# AGENTS.md — Yuldopunk 2040

## Identity

Yuldopunk 2040 is a playable web simulation game.

Product title: `율도펑크2040`  
Product subtitle: `서울 밖 50인의 AI 자급자존 생존 시뮬레이션`

The project explores a near-future Korean founding scenario: outside Seoul, in 2040, a small AI-assisted community of 50 people or fewer tries to prepare a settlement before the first winter arrives.

## First Principle

Build playable systems, not pitch material.

The first milestone is not a deck, landing page, static mockup, CAD tool, or generic town planner. It must become a browser-playable product that Minho can open, play, and share with Beomseok.

## Current Stage

- **Phase**: Phase 1 — playable founding/construction episode
- **Episode**: `첫 겨울까지 180일`
- **Maturity**: Level 0 harness initialized; implementation not started
- **Primary goal**: prepare a 50-person AI-assisted settlement before winter within 180 in-game days

## Communication

- Speak Korean to the user.
- Write system files, agent instructions, code comments, commit messages, and technical planning in English.
- All product-facing UI copy must be Korean.
- Preserve the Korean product terms exactly unless the user changes them:
  - `율도펑크2040`
  - `서울 밖 50인의 AI 자급자존 생존 시뮬레이션`
  - `첫 겨울까지 180일`
  - `AI 이장 보고서`

## Phase 1 Scope

Phase 1 focuses only on the founding/construction phase.

The player is not operating a completed town yet. The player is not only selecting a site. The player is trying to make a partially planned settlement ready before winter.

### Required Play Loop

1. Review the current settlement situation.
2. Place or adjust build modules on a village board.
3. Spend budget, days, labor, and infrastructure capacity.
4. See scores change immediately.
5. Trigger founding/construction events.
6. Adapt the plan.
7. Save snapshots and compare alternatives.
8. Reach day 180 and receive a winter readiness result.

### Required Primary Scores

- `입주 준비도`
- `겨울 생존성`
- `예산 건전성`
- `공사 진행률`
- `사회 합의`

### Required Secondary Indicators

- `인허가 리스크`
- `전력 안정성`
- `난방 안정성`
- `통신 안정성`
- `AI 의존도`
- `시공 복잡도`
- `지역 민원 위험`
- `현실성 레벨`

### Out of Scope for Phase 1

- Long-term post-completion town management
- Real architectural, legal, or engineering claims
- Login or account systems
- Paid API dependencies
- Real-time multiplayer
- A presentation page as the main result
- A static calculator with no play loop
- CAD-level modeling

## Product Design Rules

- The first screen should be the playable game screen, not a marketing landing page.
- The interface should feel like a board-game-like simulation.
- The tone should be realistic, Korean, near-future, practical, tense, and slightly absurd.
- Avoid generic dark sci-fi dashboards.
- Avoid making it only a decorative village builder.
- The emotional core is: "Could we actually live like this, and what breaks first?"

## Engineering Rules

- Prefer a simple static or frontend-only deployment unless a backend becomes necessary.
- Use structured data for scenarios, modules, events, scores, and simulation rules.
- Keep simulation rules readable and easy to tune.
- Use local persistence for snapshots in Phase 1.
- Add import/export or copyable snapshot JSON if practical.
- Do not hard-code secrets. API keys and tokens must only live in ignored environment files.
- Before claiming completion, run the app locally and verify the actual play loop in a browser.

## Workflow Triggers

| Trigger | Action |
|---|---|
| Session start | Read `progress.md`, then `docs/phase-1-goal.md`. |
| Before implementation | Confirm the task serves Phase 1 and does not drift into post-completion town operations. |
| Significant design or architecture decision | Record it in `docs/decisions.md`. |
| User expresses opinion or judgment | Run Evidence / Redundancy / Independence checks visibly before responding. |
| Bug or unexpected behavior | Use systematic debugging before proposing fixes. |
| Before claiming done | Run verification against the actual playable loop. |
| Session wrap-up | Update `progress.md` and `CHANGELOG.md`. |

## Project Structure

```text
yuldopunk-2040/
├── AGENTS.md
├── CLAUDE.md
├── README.md
├── CHANGELOG.md
├── progress.md
├── docs/
│   ├── phase-1-goal.md
│   └── decisions.md
├── src/              # future app source
├── public/           # future static assets
└── data/             # future scenario/module/event data
```

## Reference Context

- Knowledge sketch: `SK-007-AI-Native-Village-Lab`
- Collaboration proposal: `SK-007-AI-Native-Village-Lab-공동프로젝트-제안`
- Beomseok reference repository: `https://github.com/bumjaa/village_project`

