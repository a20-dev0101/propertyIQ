# Contributing to PropertyIQ

Thanks for your interest in improving PropertyIQ. Contributions of all kinds are welcome — bug fixes, better benchmarks, new features, or documentation improvements.

---

## What Can Be Improved

### Reference Data
The three files in `references/` are the most impactful place to contribute:

- **`cap-rate-benchmarks.md`** — Cap rate ranges need to stay current with market conditions. If you have data showing ranges are stale for a specific metro, open a PR with a source.
- **`defaults-by-property-type.md`** — Conservative defaults should reflect real lender requirements. If standards have shifted (e.g., down payment minimums, typical DSCR thresholds), update with a citation.
- **`insurance-benchmarks.md`** — Regional insurance costs change frequently, especially in disaster-prone states. Updates with sourced data are very welcome.

### SKILL.md Logic
If you find a category of property or deal type that PropertyIQ handles poorly, the instructions in `SKILL.md` can be extended. Common gaps:
- Mixed-use (residential + commercial)
- Mobile home parks
- Short-term rental (Airbnb/VRBO) income modeling
- International markets

### Bug Reports
If a listing URL produces incorrect output, wrong math, or a failed scrape with no fallback — open an issue with the URL and the output you received.

---

## How to Submit Changes

1. Fork the repo
2. Make your changes in a branch
3. Open a pull request with a clear description of what changed and why
4. For reference data changes, include a source (link, publication, date)

---

## Guidelines

- Keep `SKILL.md` under 500 lines — use `references/` for anything that doesn't need to be in context on every run
- Conservative defaults over optimistic ones — this tool is a feasibility screen, not a pitch deck
- Don't add dependencies — PropertyIQ works with zero setup and should stay that way
- One concern per PR — easier to review and merge

---

## Questions

Open an issue if you're unsure whether something is in scope. Happy to discuss before you spend time building it.
