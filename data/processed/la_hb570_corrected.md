# Louisiana HB-570 — Corrected Bill Data

**Date corrected:** 2026-03-12
**Anomaly reference:** C3 in `output/reports/anomaly_report.md`
**Problem:** The LegiScan API returned a property tax millage rate bill instead of the age verification bill. The scraper queried the wrong legislative session. The correct bill is from the **2025 Regular Session** (session code `25RS` on legis.la.gov, but the bill info page at `BillInfo.aspx?i=248616` is the canonical entry point).

---

## Bill Identification

| Field              | Incorrect (Old Data)                                  | Correct (2025 Regular Session)                              |
|--------------------|-------------------------------------------------------|-------------------------------------------------------------|
| **Bill**           | LA HB-570                                             | LA HB-570                                                   |
| **Session**        | Wrong session (returned property tax bill)            | 2025 Regular Session                                        |
| **Title**          | "Authorizes a taxing authority to adjust a millage rate..." | Provides relative to minors' use of applications            |
| **Short title**    | N/A                                                   | The App Store Accountability Act                            |
| **Act number**     | N/A                                                   | Act No. 481 of 2025                                         |
| **Author**         | Unknown                                               | Rep. Kim Carver (R-Bossier City)                            |
| **Status**         | Unknown                                               | Enacted — signed by Governor Jeff Landry on June 30, 2025   |
| **Effective date** | N/A                                                   | July 1, 2026                                                |

---

## Sponsors and Co-Sponsors

**Author:** Rep. Kim Carver

**House Co-Sponsors:** Representatives Adams, Amedee, Bacala, Bamburg, Bayham, Beaullieu, Berault, Billings, Boyd, Boyer, Brass, Braud, Bryant, Butler, Wilford Carter, Chassion, Chenevert, Coates, Cox, Deshotel, Dewitt, Dickerson, Domangue, Edmonston, Egan, Emerson, Firment, Fisher, Fontenot, Freiberg, Glorioso, Henry, Jackson, Mike Johnson, Lafleur, Mack, Melerine, Moore, Owen, Riser, Romero, Schamerhorn, Schlegel, Spell, Ventrella, Villio, Wilder, Wiley, and Wyble.

---

## Legislative History and Votes

| Date       | Action                                       | Vote          |
|------------|----------------------------------------------|---------------|
| 2025-05-12 | Passed House (Final Passage)                 | 99-0 (5 absent) |
| 2025-06-02 | Passed Senate (Final Passage)                | 39-0          |
| 2025-06-04 | House rejects Senate amendments              | 93-0 (12 absent) |
| 2025-06-12 | Conference Committee Report adopted (House)  | 98-0 (7 absent) |
| 2025-06-12 | Conference Committee Report adopted (Senate) | 38-0 (1 absent) |
| 2025-06-30 | Signed by Governor Jeff Landry               | —             |

**Not one "NO" vote was cast against passage of the bill at any stage.**

**Conference Committee Members:**
- House: Carver, Hebert, Schlegel (originally Carver, Deshotel, Schlegel)
- Senate: Cathey, Mizell, Morris

---

## Key Provisions

### Age Categories
The Act defines four age categories with distinct requirements:
- **Child** (under 13)
- **Younger teenager** (13-15)
- **Older teenager** (16-17)
- **Adult** (18+)

### Application Store Provider Requirements
- Must request age information when users create accounts
- Must verify ages using commercially reasonable or approved methods (including real-time age verification systems authorized by the Commissioner of the Office of Motor Vehicles)
- Must require that minor accounts be affiliated with a verified parent account
- Must obtain verifiable parental consent before allowing minors to download or purchase applications
- Must provide accurate age ratings on applications
- Must disclose data collection practices, content ratings, and significant application changes to parents

### Developer Requirements
- Must verify user ages
- Must obtain verifiable parental consent before allowing minors to download apps or make in-app purchases
- Parental consent must be renewed upon significant changes to app terms, privacy policies, or monetization features

### Data Minimization
- Collection and processing of personal data is limited strictly to what is necessary for age verification, parental consent, and compliance records
- Age verification or parental consent requests limited to once every 12 months unless reasonable cause exists for more frequent verification

### Prohibited Practices
- Developers and application stores may not enforce contracts against minors without parental consent
- Misrepresentation of information is prohibited

### Connected Devices
The conference committee report added a definition of "connected device" and expanded the bill's scope accordingly.

---

## Meta Drafted the Bill (Confirmed)

**UPDATE (2026-03-13):** Investigative reporting confirmed that **a Meta lobbyist "brought legislative language" directly to sponsor Rep. Kim Carver** for HB-570. Carver confirmed this publicly. The original bill as written placed age verification burden exclusively on app stores, not on platforms — directly serving Meta's commercial interests.

Three lobbying firms confirmed representing Meta in Louisiana:
1. **Pelican State Partners, LLC** (Koch, Rhodes, Kirkpatrick, Satpathi, Albrecht)
2. **Adams and Reese LLP** (Wilkerson, Brooks — #1 ranked LA gov affairs firm)
3. **State Capitol Solutions / State GR** (Borill)

Total: 12 lobbyists across 9 firms, at least **$324,992** ("very conservative estimate").

See `five_threads_investigation.md` and `ncose_forgood_fec_investigation.md` for complete analysis.

---

## Committee Hearing Testimony

### House Commerce Committee (approx. May 2025)
The House Commerce Committee passed HB-570 with support from multiple witnesses:

- **Brinkley Bennett** (junior, St. Joseph's Academy, Baton Rouge): Testified in support, calling HB-570 "a digital seatbelt."
- **Chris Masters** (internet crimes investigator, Louisiana Attorney General's Office): Testified in favor, noting that stores selling alcohol and cigarettes are required to check identification, and Louisiana should require the same of multi-billion-dollar tech companies.

### Senate Commerce Committee (late May 2025)
The Senate Commerce Committee passed HB-570 amid contentious debate. This hearing featured the notable exchange between Sen. Jay Morris and Casey Stefanski of the Digital Childhood Alliance.

**Tech company positions at Senate Commerce:**
- **Apple and Google:** Filed in opposition but did not send company representatives to testify.
- **Meta:** Nicole Lopez, Meta's Director of Global Litigation Strategy for Youth, testified in support, calling HB-570 a "privacy-protective solution" that streamlines parental control without overburdening app developers.
- **ACT | The App Association** (largely funded by Apple): Testified in opposition.
- **NetChoice** (members include Meta, Google, and X): Testified in opposition.
- **Chamber of Progress:** Opposed the bill on privacy and First Amendment grounds.

---

## The Morris / Stefanski Exchange (Senate Commerce Committee)

During the Senate Commerce Committee hearing, **Sen. Jay Morris (R-West Monroe)** pressed **Casey Stefanski**, Executive Director of the **Digital Childhood Alliance (DCA)**, about the organization's funding sources and tech industry ties. This exchange is significant because DCA supported HB-570 and had a paid lobbyist (Koch) registered in Louisiana.

### Key points of the exchange:

1. **Funding question:** Morris asked Stefanski to disclose which tech companies fund the Digital Childhood Alliance. Stefanski initially said she "didn't feel comfortable answering" questions about funding sources.

2. **Yes-or-no demand:** Morris pressed for a direct yes-or-no answer on whether tech companies provide funding to DCA. Stefanski eventually confirmed that tech companies **do** fund the organization but refused to name them.

3. **Largest donor:** Stefanski identified the father of DCA's founder as the organization's largest donor.

4. **Meta connection:** Stefanski acknowledged that Meta supports the legislation DCA is promoting. She said the organization is "happy" that Meta supports the bill.

5. **Model legislation:** Stefanski testified that DCA paid attorneys to draft model legislation (the App Store Accountability Act template) and has met with companies like Google in pursuit of broader industry support.

6. **501(c)(4) status:** When Morris asked whether DCA is a 501(c)(3) or 501(c)(4) organization, Stefanski confirmed it is a **501(c)(4)** — a nonprofit classification that permits political advocacy without requiring public disclosure of donors. This is significant because it means DCA's tech industry funders cannot be identified through standard nonprofit filings.

### Significance for the research:
This exchange confirmed that DCA receives tech company funding (with Meta as a known supporter) while operating under a 501(c)(4) structure that shields donor identities. Combined with DCA's rapid emergence (domain registered December 2024, paid lobbyist by May 2025) and Meta's simultaneous expansion of its Louisiana lobbying force from 2 to 7 lobbyists, this testimony supports the research finding (M3 in the anomaly report) about DCA's relationship with tech industry interests.

The Meta-DCA funding connection was further confirmed by a December 2025 Deseret News report.

---

## Correct Source URLs

- **legis.la.gov bill page:** https://www.legis.la.gov/Legis/BillInfo.aspx?i=248616
- **Enrolled text:** https://www.legis.la.gov/legis/ViewDocument.aspx?d=1425304
- **Enrolled Act (Act No. 481):** https://www.legis.la.gov/legis/ViewDocument.aspx?d=1427667
- **Original text:** https://www.legis.la.gov/Legis/ViewDocument.aspx?d=1404355
- **Engrossed text:** https://www.legis.la.gov/Legis/ViewDocument.aspx?d=1411236
- **Conference Committee Report:** https://www.legis.la.gov/legis/ViewDocument.aspx?d=1421828
- **Resume Digest (Act 481):** https://www.legis.la.gov/Legis/ViewDocument.aspx?d=1429703
- **LegiScan page:** https://legiscan.com/LA/bill/HB570/2025
- **FastDemocracy tracker:** https://fastdemocracy.com/bill-search/la/2025/bills/LAB00024814/

---

## Data Fix Notes

### What was wrong
The file `data/raw/bills/LA_HB-570.txt` contains binary PDF data of a property tax millage rate bill from a different legislative session. The LegiScan API query used the wrong session parameter, returning a different bill that happened to share the HB-570 designation.

### How to fix the raw data
1. Re-fetch the bill using LegiScan with the **2025 Regular Session** (session ID for 2025 RS on LegiScan).
2. Alternatively, download the enrolled text directly from legis.la.gov: `ViewDocument.aspx?d=1425304`
3. The bill collector script (`scripts/legislative/bill_collector.py`) needs the session parameter corrected for Louisiana. The `_scrape_louisiana` fallback should target session `25RS` or use the bill info ID `248616`.
4. After re-collection, rerun the bill similarity analysis — the current similarity scores involving LA HB-570 are invalid (binary PDF compared against HTML text).

### Impact on existing analyses
- **Bill similarity report** (`output/reports/bill_similarity_report.md`): All similarity scores involving LA HB-570 (bill #3) must be recalculated.
- **Bill status report** (`output/reports/bill_status_2026-03-11.md`): Status should be updated from numeric code `"1"` to `"enacted"`.
- **`bills` table row #3:** Session, status, and bill text all need correction.
- **`config/targets.yaml`:** Already has correct metadata (`session: "2025"`, `status: "enacted"`, `author: "Kim Carver"`). The config was right; the scraper fetched the wrong data.