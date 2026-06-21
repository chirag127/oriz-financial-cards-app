# Oriz Tabs — Cards

> India card intelligence — credit, debit, and prepaid card profiles for every major Indian issuer, with a static catalog and comparison UI.

**Live at**: <https://cards.oriz.in> · **Status**: production

## What this is

A free, searchable directory of cards issued in India — Amex, Axis, AU SFB, Bandhan, BoB, BoM, Canara, CUB, DCB, Dhanlaxmi, ESAF, Federal, HDFC, HSBC, ICICI, IDBI, IDFC, Indian Bank, IndusInd, IOB, J&K Bank, Karnataka Bank, Kotak, KVB, PNB, PSB, RBL, Saraswat, SBI, SIB, StanChart, TMB, UCO, Union, Yes Bank. Card data lives as JSON under `data/cards/{credit,debit,prepaid}/<bank>/`.

## Per-feature inventory

| Feature | Status |
| --- | --- |
| Card directory + detail pages (`credit/[issuer]/[slug]`) | ✅ live |
| `cards.json` data endpoint | ✅ live |
| Account / sign-in (shared) | ✅ live |
| Legal pages (privacy, terms, cookies, disclaimer, grievance) | ✅ live |
| Debit + prepaid detail routes | 🚧 WIP |
| Side-by-side card comparison | 📜 planned |

## App-specific env vars

None beyond the family-wide set at `templates/.env.example`.

## Local dev

```bash
# from the workspace root (c:/D/oriz)
pnpm -F @chirag127/oriz-cards dev
```

## Knowledge

See [`./knowledge/`](./knowledge/) for app-specific decisions, runbooks, and services. Family rules / decisions / architecture live at the master repo's [`knowledge/`](../../../../knowledge/).

## License

Source-available, all rights reserved. See master [`LICENSE`](../../../../LICENSE) — same terms across the family.
