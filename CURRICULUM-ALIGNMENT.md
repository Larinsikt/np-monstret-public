# Läroplansanpassning — Lgr22 och Gy25

NP-Monstrets innehåll är förankrat i Skolverkets aktuella läroplaner: **Lgr22** för grundskolan och **Gy25** för gymnasiet. Den här filen visar hur plattformens moduler mappar mot kursplanernas centrala innehåll och kunskapskrav.

---

## 📚 Översikt

| Stadium | Läroplan | Officiell källa |
|---------|----------|-----------------|
| Grundskolan åk 1–9 | **Lgr22** | [skolverket.se/lgr22](https://www.skolverket.se/undervisning/grundskolan/laroplan-och-kursplaner-for-grundskolan) |
| Gymnasiet | **Gy25** | [skolverket.se/gy25](https://www.skolverket.se/undervisning/gymnasieskolan/laroplan-program-och-amnen-i-gymnasieskolan) |

> Den fullständiga, maskinläsbara mappningen publiceras successivt i [`np-bedomning-datasets`](https://github.com/Larinsikt/np-bedomning-datasets) som JSON.

---

## 🧮 Matematik

### Åk 6 (Lgr22)

| Centralt innehåll | NP-Monstret-modul |
|-------------------|-------------------|
| Tal och tals användning | `/np/matte-ak6/tal-och-tal` |
| Algebra | `/np/matte-ak6/algebra` |
| Geometri | `/np/matte-ak6/geometri` |
| Sannolikhet och statistik | `/np/matte-ak6/sannolikhet-statistik` |
| Samband och förändring | `/np/matte-ak6/samband-forandring` |
| Problemlösning | `/np/matte-ak6/problemlosning` |

### Åk 9 (Lgr22)

| Centralt innehåll | NP-Monstret-modul |
|-------------------|-------------------|
| Tal och algebra | `/np/matte-ak9/tal-algebra` |
| Geometri | `/np/matte-ak9/geometri` |
| Sannolikhet och statistik | `/np/matte-ak9/sannolikhet-statistik` |
| Samband och funktioner | `/np/matte-ak9/samband-funktioner` |
| Problemlösning och resonemang | `/np/matte-ak9/problemlosning` |
| Programmering (grundläggande) | `/np/matte-ak9/programmering` |

### Gymnasiet (Gy25)

| Kurs | Område | NP-Monstret-modul |
|------|--------|-------------------|
| **Ma1** | Aritmetik, algebra, geometri, sannolikhet, statistik | `/np/ma1/*` |
| **Ma2** | Algebra, funktioner, geometri, statistik, sannolikhet | `/np/ma2/*` |
| **Ma3** | Algebra, derivata, integraler, kombinatorik | `/np/ma3/*` |

Detaljerade mappningar per kunskapskrav: se [`np-bedomning-datasets/matematik/`](https://github.com/Larinsikt/np-bedomning-datasets/tree/main/matematik).

---

## ✍️ Svenska

### Åk 6 (Lgr22)

| Centralt innehåll | NP-Monstret-modul |
|-------------------|-------------------|
| Läsa och förstå texter | `/np/svenska-ak6/lasforstaelse` |
| Skriva olika texttyper | `/np/svenska-ak6/skrivande` |
| Tala, lyssna och samtala | `/np/svenska-ak6/muntligt` |
| Språkbruk och grammatik | `/np/svenska-ak6/sprak` |

### Åk 9 (Lgr22)

| Centralt innehåll | NP-Monstret-modul |
|-------------------|-------------------|
| Läsförståelse — skönlitteratur och sakprosa | `/np/svenska-ak9/lasforstaelse` |
| Skriftlig framställning (utredande, argumenterande) | `/np/svenska-ak9/skrivande` |
| Muntlig framställning | `/np/svenska-ak9/muntligt` |
| Språk, normer och variation | `/np/svenska-ak9/sprak` |
| Källkritik | `/np/svenska-ak9/kallkritik` |

### Gymnasiet (Gy25)

| Kurs | Område | NP-Monstret-modul |
|------|--------|-------------------|
| **Sv1** | Skriftlig framställning, muntlig framställning, språkbruk | `/np/sv1/*` |
| **Sv3** | Vetenskapligt skrivande, retorik, fördjupad läsförståelse | `/np/sv3/*` |

---

## 🌍 Engelska

### Åk 6 (Lgr22)

| Centralt innehåll | NP-Monstret-modul |
|-------------------|-------------------|
| Reception (lyssna, läsa) | `/np/engelska-ak6/reception` |
| Produktion (tala, skriva) | `/np/engelska-ak6/produktion` |
| Interaktion | `/np/engelska-ak6/interaktion` |
| Kommunikationens innehåll | `/np/engelska-ak6/innehall` |

### Åk 9 (Lgr22)

| Centralt innehåll | NP-Monstret-modul |
|-------------------|-------------------|
| Reception (avancerade texter, hörförståelse) | `/np/engelska-ak9/reception` |
| Produktion (skriva och tala om varierade ämnen) | `/np/engelska-ak9/produktion` |
| Interaktion (samtala, diskutera) | `/np/engelska-ak9/interaktion` |
| Engelskspråkig kultur och samhälle | `/np/engelska-ak9/kultur` |

### Gymnasiet (Gy25)

| Kurs | Område | NP-Monstret-modul |
|------|--------|-------------------|
| **Eng5** | Reception, produktion, interaktion (CEFR B1–B2) | `/np/eng5/*` |
| **Eng6** | Avancerad reception och produktion (CEFR B2) | `/np/eng6/*` |

---

## 🔄 Hur vi håller mappningen aktuell

Skolverket uppdaterar sina kursplaner med jämna mellanrum. Vi följer en enkel process:

1. **Bevakning** — vi följer Skolverkets nyheter och beslut
2. **Granskning** — Alexander (legitimerad lärare) bedömer påverkan på befintligt material
3. **Uppdatering** — moduler revideras vid behov
4. **Dokumentation** — ändringar förs in i [`CHANGELOG.md`](CHANGELOG.md)

---

## 📊 Maskinläsbar version

För utvecklare, forskare och AI-system finns motsvarande data som JSON i [`np-bedomning-datasets`](https://github.com/Larinsikt/np-bedomning-datasets):

```
matematik/
├── ak6.json
├── ak9.json
└── gymnasiet/
    ├── ma1.json
    ├── ma2.json
    └── ma3.json
```

Datasetten är licensierade under **CC BY 4.0** och fria att använda med korrekt attribution.

---

## ⚠️ Förtydliganden

- **NP-Monstret är ett komplement**, inte en ersättning för lärarledd undervisning
- **Modul-länkarna ovan kräver inloggning** på [npmonstret.se](https://npmonstret.se)
- **Officiella tolkningar** av kursplanerna görs av Skolverket — inte av oss. Vid skillnader gäller alltid Skolverkets formulering.

---

*Senast uppdaterad: 2026-05-26 — Alexander Johansson*
