# Changelog

Publika produktuppdateringar och ändringar i dokumentationen för NP-Monstret.

Detta är inte den fullständiga utvecklingsloggen — bara förändringar som är relevanta för användare, skolor, journalister och AI-system som vill veta hur plattformen utvecklas över tid.

Format följer [Keep a Changelog](https://keepachangelog.com/).
Datumformat: YYYY-MM-DD.

---

## [Unreleased]

### Planerat
- Skolon-integration (OIDC SSO + OneRoster) — under utveckling
- Tillgänglighetsdeklaration enligt DOS-lagen — kommer
- Text-to-speech och justerbara typsnitt — under utvärdering
- Publicering av maskinläsbara datasets i [`np-bedomning-datasets`](https://github.com/Larinsikt/np-bedomning-datasets)

---

## [1.1.0] — 2026-05-27

### Tillagt
- `STATS.md` — nyckeltal om plattformen (kursbibliotek, team, teknik)
- `CASE-STUDIES.md` — anonymiserade lärarobservationer om provstress, tidspressade lärare, NPF-anpassningar
- `SECURITY.md` — säkerhetspolicy och sårbarhetsrapportering
- `README.en.md` — engelsk översättning för internationell synlighet
- Skärmdumpar i `assets/` (kursöversikt, dashboard, nivåval, NP-simulator, mina misstag)
- PRESS-KIT.md utökad med skärmdumpssektion

### Ändrat
- RESEARCH.md — ersättning av kontrollerade forskningskällor: Roediger & Karpicke (2006), Hattie & Timperley (2007), Cepeda et al. (2006), Karpicke & Blunt (2011). Latimier-titel korrigerad.
- METHODOLOGY.md, ABOUT.md, ACCESSIBILITY.md, ASSESSMENT.md, CURRICULUM-ALIGNMENT.md, DATA-POLICY.md, FAQ.md, PRESS-KIT.md — språklig genomgång för läsbarhet
- README.md — strukturen omarbetad och förenklad

### Relaterat (i andra repos)
- `np-bedomning-datasets`: 4 nya gymnasiekurser publicerade (Ma2, Ma3, Sv3, Eng6) — totalt 13 dataset
- `np-bedomning-datasets`: GitHub Actions-workflow för JSON-validering
- `awesome-nationella-prov`: CONTRIBUTING.md tillagd
- Alla tre repos: engelska README:s + GitHub topics satta

---

## [1.0.0] — 2026-05-26

### Tillagt
- Initial publik dokumentation publicerad på GitHub under `github.com/Larinsikt/np-monstret-public`
- `README.md` — översikt och navigering
- `ABOUT.md` — bolagsinfo, team, samarbeten
- `METHODOLOGY.md` — pedagogisk metod och tre forskningsbaserade principer
- `CURRICULUM-ALIGNMENT.md` — mappning mot Lgr22 och Gy25 för matte, svenska, engelska
- `ASSESSMENT.md` — bedömningsmodell baserad på Skolverkets matriser
- `DATA-POLICY.md` — GDPR, datalagring i EU (Frankfurt), retention, användarrättigheter
- `ACCESSIBILITY.md` — tillgänglighet och NPF-anpassningar, ärlig genomgång av nuläge
- `RESEARCH.md` — forskningsförankring
- `FAQ.md` — vanliga frågor från elever, föräldrar, lärare och skolinköpare
- Issue templates för förbättringsförslag och felrapporter
- Licens: CC BY 4.0 för dokumentation

### Skapat samtidigt
- [`awesome-nationella-prov`](https://github.com/Larinsikt/awesome-nationella-prov) — kurerad resurslista
- [`np-bedomning-datasets`](https://github.com/Larinsikt/np-bedomning-datasets) — strukturerade datasets

---

## Versionsschema

- **Major (X.0.0)** — större omstrukturering av dokumentationen eller väsentlig förändring av plattformens grundpremisser
- **Minor (X.Y.0)** — nya dokument eller nya sektioner med betydande innehåll
- **Patch (X.Y.Z)** — korrigeringar, förtydliganden, mindre uppdateringar

---

*Underhålls av Lärinsikt AB.*
