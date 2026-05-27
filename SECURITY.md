# Säkerhet

NP-Monstret tar säkerhet på allvar. Det här dokumentet beskriver hur vi hanterar säkerhet på en övergripande nivå, och hur du kan rapportera sårbarheter.

## Rapportera en sårbarhet

Hittar du en sårbarhet i NP-Monstret? Skicka ett mejl till **hej@npmonstret.se** med ämnesrad "Säkerhet" så återkopplar vi inom 72 timmar.

Vi uppskattar ansvarsfull rapportering. Publicera inte detaljer om sårbarheten offentligt innan vi haft chans att åtgärda den.

## Vad du kan rapportera

- Tekniska sårbarheter (autentisering, datamapp, sessionshantering)
- Brister i hur personuppgifter hanteras
- Bypassar i betal- eller premiumflöden
- Felkonfigurerade tjänster eller exponerade endpoints

## Vad som inte räknas

- Spam, phishing eller social engineering mot anställda
- DoS- eller DDoS-attacker
- Brister i tredjepartstjänster vi använder (rapportera direkt till leverantören)

## Övergripande säkerhetsåtgärder

För transparens, utan tekniska detaljer:

- All trafik krypteras med TLS
- Lösenord lagras som saltade hashar, aldrig i klartext
- Autentisering hanteras av etablerad identitetsleverantör
- Data lagras inom EU (Frankfurt)
- Loggar och backuper raderas enligt GDPR-kompatibel retentionspolicy
- Inga elevpersonuppgifter delas med tredje part utöver de leverantörer som är nödvändiga för driften (alla med GDPR-anpassade avtal)

## Dataskydd och GDPR

Mer detaljerad information finns i [DATA-POLICY.md](DATA-POLICY.md).

## Ansvar

Ansvarig för säkerhet hos Lärinsikt AB är Alexander Johansson. Kontakt: hej@npmonstret.se.

---

*Senast uppdaterad: 2026-05-27*
