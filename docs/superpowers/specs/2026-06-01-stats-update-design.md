# Stats Section Update — Design Spec

## Goal
Replace the existing stats numbers with honest, impactful metrics that build trust
with potential clients while reflecting the company's young but experienced position.

## Current Stats
- 50+ Projects delivered
- 30+ Clients served
- 5+ Years in the market
- 98% Client satisfaction

## New Stats (4 items)

| Statistic | Description (EN) | Description (PT) |
|-----------|-----------------|-----------------|
| 4+        | Countries served | Países atendidos |
| 2+        | Years in the market | Anos de mercado |
| 10+       | Years of team experience | Anos de experiência da equipe |
| 100%      | On-time delivery, end-to-end | Entrega no prazo, do início ao fim |

## Reasoning
- **4+ countries** — shows global reach without overclaiming
- **2+ years** — honest about company age while showing establishment
- **10+ years team experience** — bridges credibility gap between company age and expertise
- **100% on-time, end-to-end** — quality signal combining delivery reliability with full-scope capability,
  merged into one stat to fit the 4-item layout limit

## Design
- Layout: `minimal` (existing, keeps gradient numbers)
- Makes `lg:grid-cols-4` on desktop, `grid-cols-2` on mobile
- Staggered counter animation on scroll (existing behavior)

## Files Affected
- `content/en/_index.md`
- `content/pt/_index.md`
