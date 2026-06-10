# CLAUDE.md — Yuldopunk 2040

## Identity

Yuldopunk 2040 is a playable web simulation game.

Product title: `율도펑크2040`  
Product subtitle: `서울 밖 50인의 AI 자급자존 생존 시뮬레이션`

The first playable episode is `첫 겨울까지 180일`: outside Seoul, in 2040, a small AI-assisted community of 50 people or fewer must prepare a viable settlement before winter.

## First Principle

Build playable systems, not pitch material.

The first milestone must be something Minho can open in a browser and play. Do not let the project collapse into a deck, landing page, static dashboard, or CAD-like drawing tool.

## Communication

- Speak Korean to the user.
- Write system files, agent instructions, code comments, commit messages, and technical planning in English.
- All product-facing UI copy must be Korean.
- Preserve these Korean terms exactly unless the user changes them:
  - `율도펑크2040`
  - `서울 밖 50인의 AI 자급자존 생존 시뮬레이션`
  - `첫 겨울까지 180일`
  - `AI 이장 보고서`

## Phase 1 Scope

The current phase is founding/construction, not long-term town operation.

The player is trying to prepare a 50-person AI-assisted settlement before the first winter arrives. Gameplay must center on time, budget, construction progress, winter survivability, infrastructure, and social agreement.

### Required Play Loop

1. Review settlement status.
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

## Capabilities

Follow the superpowers discipline for development work:

```text
brainstorming -> writing-plans -> executing-plans -> verification-before-completion
```

Use product-design workflows before UI/prototype implementation when available. Use frontend-design guidance for frontend builds. Use verification-before-completion before any completion claim.

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

## Product Design Rules

- First screen: playable game screen, not a marketing landing page.
- Feel: board-game-like simulation.
- Tone: Korean, near-future, realistic, practical, tense, slightly absurd.
- Avoid generic dark sci-fi dashboards.
- Avoid decorative-only village building.
- Emotional core: "Could we actually live like this, and what breaks first?"

## Engineering Rules

- Prefer a simple static or frontend-only deployment until a backend is justified.
- Use structured data for scenarios, modules, events, scores, and rules.
- Keep simulation rules readable and easy to tune.
- Store snapshots locally in Phase 1.
- Add import/export or copyable snapshot JSON if practical.
- Never hard-code secrets.
- Verify the actual browser play loop before claiming done.

## Reference Context

- Knowledge sketch: `SK-007-AI-Native-Village-Lab`
- Collaboration proposal: `SK-007-AI-Native-Village-Lab-공동프로젝트-제안`
- Beomseok reference repository: `https://github.com/bumjaa/village_project`

