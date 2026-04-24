# Codebook — Variable Definitions and Coding Scheme

This document defines all variables used in the dataset and their coding categories.

## Dataset Sheets

### Sheet 1: All 853 Records

Contains every unique record after deduplication.

| Variable | Type | Description |
|----------|------|-------------|
| `#` | Integer | Sequential record number |
| `Title` | Text | Full title of the study |
| `Authors` | Text | Author names |
| `Year` | Integer | Publication year |
| `Database` | Categorical | Source database (Google Scholar, ACM, IEEE, Scopus, WoS) |
| `Query` | Categorical | Search query that retrieved the record (S1, S2, S3) |
| `Relevance` | Categorical | Relevance rating assigned during screening |
| `Screening` | Categorical | Screening outcome (PASS / FAIL) |
| `Decision` | Categorical | Final decision on inclusion |
| `Abstract (preview)` | Text | Truncated abstract excerpt |

**Decision values:**
- `INCLUDED (Final 71)` — Included in final review
- `PASSED TO CURATION` — Passed screening but excluded during full-text curation
- `EXCLUDED (E2: Victimisation only)` — Excluded: victimisation focus only
- `EXCLUDED (E3: Not crime-related)` — Excluded: search terms matched incidentally
- `EXCLUDED (Low relevance)` — Excluded during relevance assessment

### Sheet 2: Duplicate Identification

| Variable | Type | Description |
|----------|------|-------------|
| `#` | Integer | Duplicate record number |
| `Title` | Text | Title of the duplicated study |
| `Kept In (Database)` | Text | Database where the record was retained |
| `Kept In (Query)` | Text | Query associated with the retained record |
| `Duplicate Found In (Database)` | Text | Database where duplicate was found |
| `Duplicate Found In (Query)` | Text | Query that retrieved the duplicate |
| `Duplicate Type` | Categorical | Type of duplication detected |

### Sheet 3: Screening Pipeline

PRISMA-compliant breakdown of each screening stage with counts of records in and out.

### Sheet 4: Final 71 Studies

The primary analytical dataset containing all included studies.

| Variable | Type | Description | Categories |
|----------|------|-------------|------------|
| `ID` | Integer | Study identifier (1–71) | — |
| `Authors (Year)` | Text | Author surname(s) and publication year | — |
| `Title` | Text | Full study title | — |
| `Source/Journal` | Text | Publication venue | — |
| `Design` | Categorical | Study design / methodology | See below |
| `Crime Type` | Categorical | Primary crime focus | See below |
| `Glorification Level` | Categorical | How centrally the study addresses glorification | See below |
| `Country` | Text | Geographic focus of the study | See below |

#### Design Categories

| Category | Description |
|----------|-------------|
| Qualitative | Interview-based, thematic analysis, or grounded theory |
| Quantitative | Statistical analysis, surveys with quantitative measures |
| Mixed Methods | Combines qualitative and quantitative approaches |
| Theoretical | Conceptual or framework-building paper |
| Ethnography | Participant observation or immersive fieldwork |
| Content Analysis | Systematic analysis of media content |
| Discourse Analysis | Analysis of language and framing in texts |
| Network Analysis | Social network or relational mapping |
| Literature Review | Narrative or scoping review |
| Systematic Review | Follows PRISMA or similar structured protocol |
| Survey | Structured questionnaire-based study |
| Case Study | In-depth examination of a specific instance |
| Crime Script Analysis | Procedural mapping of criminal processes |
| Corpus Linguistics | Large-scale computational text analysis |
| Media Analysis | Analysis of news or media coverage |
| Profiling Study | Offender profiling or classification |

#### Crime Type Categories

| Category | Description |
|----------|-------------|
| Cybercrime | General cybercrime including hacking, malware, DDoS |
| Cybercrime (fraud) | Internet fraud, advance-fee fraud, romance scams, "Yahoo Boys" |
| Hacktivism | Politically motivated hacking (e.g., Anonymous) |
| Gang culture | Street gang activity with cyber/digital dimension |
| Crime (general) | Comparative studies covering multiple crime types |
| Terrorism | Violent extremism and terrorist activity |

#### Glorification Level Categories

| Category | Description |
|----------|-------------|
| Central | Glorification/flex culture is the primary research focus |
| Central (Nigeria) | Central focus specifically on Nigerian cybercrime glamorisation |
| Central (terrorism) | Central focus on glorification of terrorism |
| Central (gangs) | Central focus on glorification of gang culture |
| Tangential | Glorification is discussed but not the main focus |
| Peripheral | Brief or passing mention of glorification/prestige |
| Absent | No mention of glorification; included for other relevance |
| Absent (implied) | Glorification not mentioned but implied by findings |

**Consolidated coding** (used in analyses):
- **Central** = Central + Central (Nigeria) + Central (terrorism) + Central (gangs)
- **Tangential** = Tangential
- **Peripheral** = Peripheral
- **Absent** = Absent + Absent (implied)

#### Country/Region Coding

Studies are coded by primary geographic focus. Multi-country studies use combined codes (e.g., `UK/USA`). Studies without a specific national focus are coded as `International` or `Global`.

### Sheet 5: Database Breakdown

Summary table showing the number of records found and exported per database per search query.
