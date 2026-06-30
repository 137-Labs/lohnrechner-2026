# Stundenlohn & Reverse Netto Rechner

🔗 **[Live App öffnen](https://137-labs.github.io/lohnrechner-2026/)**

Single-file web tool for German hourly wages and net pay.

## What it does

- **Forward mode:** enter a gross hourly wage → see net pay per hour, day, week, month, year.
- **Reverse mode:** enter a target monthly net income → calculates the gross hourly wage required to hit it.
- Accounts for Steuerklasse (1–6), Lohnsteuer, Solidaritätszuschlag, optional Kirchensteuer, Rentenversicherung, Arbeitslosenversicherung, Krankenversicherung (incl. Zusatzbeitrag), Pflegeversicherung, and contribution caps (Beitragsbemessungsgrenzen).

## Stack

Single `index.html`. No build step, no backend, no dependencies. Deploy to GitHub Pages or Vercel as-is.

## Tax data

All yearly constants (brackets, caps, allowances) live in one `TAX_YEAR` object near the top of the script, so they can be updated each January without touching the calculation logic.

*Note: figures are estimates and may not match official German wage tax tables exactly — double-check before relying on them for major decisions.*

## License

Personal/portfolio project, 137-labs.
