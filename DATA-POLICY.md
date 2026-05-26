# Datapolicy

Hur NP-Monstret hanterar elev- och användardata. Den här filen beskriver principer på hög nivå — fullständiga juridiska villkor finns i användaravtal och personuppgiftsbiträdesavtal (PuB-avtal) som signeras med skolor och organisationer.

---

## 🇪🇺 Var data lagras

All användardata för NP-Monstret lagras i **Europeiska Unionen**.

| Detalj | Värde |
|--------|-------|
| **Region** | Frankfurt, Tyskland |
| **Cloud-leverantör** | AWS (eu-central-1) |
| **Databas** | Supabase (Postgres) |
| **Hosting** | Vercel (EU-region för svensk trafik) |

**Inga personuppgifter förs ut ur EU.** Det innebär att GDPR Art. 44–49 (överföringar till tredje land) inte är aktuell — vi har valt arkitektur så att frågan inte uppstår.

---

## 📜 Juridisk grund

NP-Monstret hanterar personuppgifter enligt **Dataskyddsförordningen (GDPR)** och svensk dataskyddslag.

### För elever via skola

När en skola eller kommun upphandlar NP-Monstret är **skolan/kommunen personuppgiftsansvarig** och **Lärinsikt AB är personuppgiftsbiträde**. Förhållandet regleras genom ett personuppgiftsbiträdesavtal (PuB-avtal) enligt GDPR Art. 28.

### För privatkunder

När en privatperson köper NP-Monstret direkt är **Lärinsikt AB personuppgiftsansvarig**. Användaren samtycker till behandlingen genom att skapa konto och godkänna användarvillkoren.

---

## 🔐 Vad vi samlar in

Vi tillämpar **dataminimering** — vi sparar bara det som faktiskt behövs för att tjänsten ska fungera.

### Alltid

- E-postadress (för inloggning och kommunikation)
- Namn (för personalisering)
- Vald årskurs eller kurs (för att visa rätt innehåll)
- Genomförda uppgifter och resultat (för progress)
- Tekniska loggar (för felsökning och säkerhet)

### Vid skolintegration

- Skolans namn och organisations-ID
- Klasstillhörighet
- Lärarens roll (lärare/elev/admin)

### Aldrig

- ❌ Personnummer
- ❌ Politiska åsikter, religion, hälsa eller annan känslig data (GDPR Art. 9)
- ❌ Innehåll i privata meddelanden eller anteckningar utöver det som är relevant för uppgifter
- ❌ Platsdata (GPS)
- ❌ Information från andra appar eller tjänster

---

## ⏱️ Hur länge data sparas (retention)

| Typ av data | Retention |
|-------------|-----------|
| Aktivt användarkonto | Så länge kontot är aktivt |
| Inaktivt konto (ingen inloggning) | Raderas automatiskt efter 24 månader |
| Genomförda uppgifter | Bevaras under kontots livslängd, raderas med kontot |
| Tekniska loggar (felsökning) | 90 dagar |
| Säkerhetsloggar | 12 månader |
| Ekonomiska underlag (fakturor) | 7 år (bokföringslagen) |
| Skoldata efter avtalsslut | Raderas inom 30 dagar efter avtalets upphörande |

---

## 🛡️ Skydd av data

På hög nivå:

- **Kryptering i transit:** TLS för all kommunikation mellan användare och plattform
- **Kryptering at rest:** All data krypterad på lagringsnivå hos cloud-leverantören
- **Behörighetsstyrning:** Användare ser bara sin egen data; lärare ser bara sina egna klassers data
- **Loggning:** Säkerhetsrelevanta händelser loggas automatiskt
- **Incidentplan:** Incidenter rapporteras enligt GDPR Art. 33–34 (inom 72 timmar till tillsynsmyndighet, vid hög risk även till påverkade personer)

För skolinköpare som behöver mer detaljer kring säkerhetsarkitektur — kontakta oss för en NDA-skyddad genomgång.

---

## 👤 Dina rättigheter (GDPR)

Användare i NP-Monstret har följande rättigheter:

| Rätt | Vad det betyder | Hur du utövar den |
|------|-----------------|-------------------|
| **Tillgång** (Art. 15) | Få veta vilka uppgifter vi har om dig | Begär utdrag via mejl |
| **Rättelse** (Art. 16) | Få felaktiga uppgifter korrigerade | Ändra själv eller kontakta oss |
| **Radering** (Art. 17) | Få ditt konto och all data raderad | Använd "Ta bort konto" eller mejla oss |
| **Begränsning** (Art. 18) | Pausa behandlingen | Mejla oss |
| **Dataportabilitet** (Art. 20) | Få ut din data i maskinläsbart format | Begär export via mejl |
| **Invändning** (Art. 21) | Invända mot viss behandling | Mejla oss |
| **Klaga** | Lämna in klagomål till tillsynsmyndighet | [imy.se](https://www.imy.se) |

**Svarstid:** Vi svarar inom 30 dagar (GDPR Art. 12.3).

---

## 🤖 Tredjepartstjänster

NP-Monstret använder ett begränsat antal noga utvalda tredjepartstjänster. Listan är medvetet kort.

| Tjänst | Funktion | Datalokalisering |
|--------|----------|------------------|
| Supabase | Databas och autentisering | EU (Frankfurt) |
| Vercel | Webbhotell | EU för EU-trafik |
| Stripe | Betalningar (privatkunder) | EU (DPA tecknat) |
| Google OAuth | Inloggning (om användaren väljer det) | Användarens val |
| Skolon | Distributionsplattform (vid integration) | EU |

Inga tredjepartstjänster används för annonsering eller spårning av minderåriga.

---

## 🍪 Cookies och spårning

NP-Monstret använder enbart **funktionella cookies** som krävs för att tjänsten ska fungera (inloggning, sessioner, preferenser).

- ❌ Inga marknadsföringscookies
- ❌ Inga tredjepartscookies för annonser
- ❌ Ingen försäljning av data till annonsörer
- ✅ Anonymiserad analys för att förbättra plattformen (frivillig)

Se [npmonstret.se/integritetspolicy](https://npmonstret.se/integritetspolicy) för fullständig cookie-information.

---

## 👶 Barn och minderåriga

NP-Monstret riktar sig delvis till elever under 16 år. Vi följer extra strikta principer för minderåriga:

- **Inget marknadsföringsmaterial** riktas direkt till barn
- **Inga annonser** visas i plattformen
- **Föräldrasamtycke** krävs för privatkonton för elever under 13 år
- **Skolkonton** hanteras enligt skolans rutiner — skolan är personuppgiftsansvarig

---

## 📬 Kontakt i datafrågor

För frågor om personuppgifter, dataskydd eller utövande av dina rättigheter:

- **E-post:** [hej@npmonstret.se](mailto:hej@npmonstret.se)
- **Post:** Lärinsikt AB *(adress läggs till)*
- **Tillsynsmyndighet:** [Integritetsskyddsmyndigheten (IMY)](https://www.imy.se)

---

## 🔄 Ändringar i policyn

När vi uppdaterar denna policy:

1. Den nya versionen publiceras här
2. Ändringen dokumenteras i [`CHANGELOG.md`](CHANGELOG.md)
3. Vid betydande ändringar informerar vi alla aktiva användare via e-post

---

*Senast uppdaterad: 2026-05-26 — Lärinsikt AB*

> Den fullständiga juridiska integritetspolicyn finns på [npmonstret.se/integritetspolicy](https://npmonstret.se/integritetspolicy). Vid skillnader mellan denna fil och den juridiska policyn på hemsidan gäller hemsidan.
