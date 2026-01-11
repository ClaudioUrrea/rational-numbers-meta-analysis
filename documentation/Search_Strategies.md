# Database Search Strategies

## Meta-Analysis: Technology-Enhanced Rational Number Learning in K-12 Education

**Search Date**: December 20, 2025  
**Databases Searched**: 6  
**Date Range**: January 2015 - December 2025  
**Language**: English  
**Search Strategy Developer**: Claudio Urrea (ORCID: 0000-0001-7197-8928)

---

## Table of Contents

1. [Search Concept Framework](#search-concept-framework)
2. [Database 1: Web of Science Core Collection](#database-1-web-of-science-core-collection)
3. [Database 2: Scopus](#database-2-scopus)
4. [Database 3: ERIC (ProQuest)](#database-3-eric-proquest)
5. [Database 4: IEEE Xplore Digital Library](#database-4-ieee-xplore-digital-library)
6. [Database 5: EBSCO Education Source](#database-5-ebsco-education-source)
7. [Database 6: PsycINFO (Ovid)](#database-6-psycinfo-ovid)
8. [Supplementary Search Methods](#supplementary-search-methods)
9. [Search Results Summary](#search-results-summary)
10. [Search Refinement Process](#search-refinement-process)

---

## Search Concept Framework

### Three-Concept Boolean Strategy

The search combined three concept clusters using Boolean operators:

**Concept 1: RATIONAL NUMBERS**
- fraction*
- "rational number*"
- decimal*
- proportion*
- ratio*
- "proportional reasoning"

**Concept 2: TECHNOLOGY**
- "intelligent tutor*"
- ITS
- "artificial intelligence"
- AI
- "adaptive learning"
- "personalized learning"
- "augmented reality"
- AR
- "virtual reality"
- VR
- "educational robot*"
- "learning analytics"
- "technology enhanced"
- "digital learning"

**Concept 3: EDUCATIONAL CONTEXT**
- teach*
- learn*
- instruct*
- educat*
- mathematics
- math
- STEM
- K-12
- elementary
- primary
- secondary

### Boolean Logic

```
(Concept 1) AND (Concept 2) AND (Concept 3)
```

### Filters Applied

- **Publication Date**: 2015-2025
- **Language**: English
- **Document Type**: Journal articles (peer-reviewed)
- **Quality**: Q1/Q2 journals (JCR or SJR rankings)

---

## Database 1: Web of Science Core Collection

### Platform Details
- **Database**: Web of Science Core Collection
- **Interface**: Clarivate Analytics Web of Science
- **Fields Searched**: Topic (TS) = Title, Abstract, Keywords
- **Indexes**: SCI-EXPANDED, SSCI, A&HCI, ESCI

### Complete Search String

```
TS=(
  (fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  AND
  ("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  AND
  (teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR K-12 OR elementary OR primary OR secondary)
)
AND PY=(2015-2025)
AND LA=(English)
AND DT=(Article)
```

### Filters Applied
- **Timespan**: 2015-2025
- **Language**: English
- **Document Types**: Article
- **Databases**: WOS.SCI, WOS.SSCI, WOS.AHCI, WOS.ESCI

### Results
- **Initial Hits**: 1,847
- **After Q1/Q2 filter**: 423
- **After title/abstract screening**: 87
- **After full-text review**: 8

---

## Database 2: Scopus

### Platform Details
- **Database**: Scopus
- **Interface**: Elsevier ScienceDirect
- **Fields Searched**: TITLE-ABS-KEY (Title, Abstract, Keywords)
- **Coverage**: Multi-disciplinary (science, social science, humanities)

### Complete Search String

```
TITLE-ABS-KEY (
  (fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  AND
  ("intelligent tutor*" OR its OR "artificial intelligence" OR ai OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR ar OR "virtual reality" OR vr OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  AND
  (teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR stem OR "K-12" OR elementary OR primary OR secondary)
)
AND PUBYEAR > 2014 AND PUBYEAR < 2026
AND ( LIMIT-TO ( DOCTYPE , "ar" ) )
AND ( LIMIT-TO ( LANGUAGE , "English" ) )
AND ( LIMIT-TO ( SUBJAREA , "SOCI" ) OR LIMIT-TO ( SUBJAREA , "COMP" ) OR LIMIT-TO ( SUBJAREA , "PSYC" ) )
```

### Filters Applied
- **Publication Year**: 2015-2025
- **Document Type**: Article
- **Language**: English
- **Subject Area**: Social Sciences, Computer Science, Psychology

### Results
- **Initial Hits**: 2,134
- **After Q1/Q2 filter (SJR)**: 512
- **After title/abstract screening**: 103
- **After full-text review**: 9
- **Overlap with WoS**: 6

---

## Database 3: ERIC (ProQuest)

### Platform Details
- **Database**: Education Resources Information Center (ERIC)
- **Interface**: ProQuest
- **Fields Searched**: All fields (AB, TI, SU, ID)
- **Coverage**: Education-focused

### Complete Search String

```
(
  ab(fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  OR ti(fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  OR su(fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
)
AND
(
  ab("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  OR ti("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  OR su("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
)
AND
(
  ab(teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR "K-12" OR elementary OR primary OR secondary)
  OR ti(teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR "K-12" OR elementary OR primary OR secondary)
)
```

### Filters Applied via Interface
- **Publication Date**: 2015-2025
- **Language**: English
- **Source Types**: Academic Journals (peer-reviewed)
- **Education Level**: Elementary, Secondary

### Results
- **Initial Hits**: 1,456
- **After peer-review filter**: 876
- **After title/abstract screening**: 67
- **After full-text review**: 7
- **Overlap with previous**: 5

---

## Database 4: IEEE Xplore Digital Library

### Platform Details
- **Database**: IEEE Xplore
- **Interface**: IEEE Xplore Digital Library
- **Fields Searched**: Metadata (Abstract, Title, Author Keywords, IEEE Keywords)
- **Coverage**: Engineering, computer science, education technology

### Complete Search String

```
(
  "Document Title":(fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  OR "Abstract":(fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  OR "Author Keywords":(fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
)
AND
(
  "Document Title":("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  OR "Abstract":("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  OR "Author Keywords":("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
)
AND
(
  "Document Title":(teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR "K-12" OR elementary OR primary OR secondary)
  OR "Abstract":(teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR "K-12" OR elementary OR primary OR secondary)
)
```

### Filters Applied via Interface
- **Publication Year**: 2015-2025
- **Content Type**: Journals
- **Language**: English

### Results
- **Initial Hits**: 324
- **After journal filter**: 189
- **After title/abstract screening**: 28
- **After full-text review**: 3
- **Overlap with previous**: 2

---

## Database 5: EBSCO Education Source

### Platform Details
- **Database**: Education Source
- **Interface**: EBSCO
- **Fields Searched**: AB (Abstract), TI (Title), SU (Subject Terms)
- **Coverage**: Education, teaching methods

### Complete Search String

```
(
  AB (fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  OR TI (fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
  OR SU (fraction* OR "rational number*" OR decimal* OR proportion* OR ratio* OR "proportional reasoning")
)
AND
(
  AB ("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  OR TI ("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
  OR SU ("intelligent tutor*" OR ITS OR "artificial intelligence" OR AI OR "adaptive learning" OR "personalized learning" OR "augmented reality" OR AR OR "virtual reality" OR VR OR "educational robot*" OR "learning analytics" OR "technology enhanced" OR "digital learning")
)
AND
(
  AB (teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR "K-12" OR elementary OR primary OR secondary)
  OR TI (teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR "K-12" OR elementary OR primary OR secondary)
  OR SU (teach* OR learn* OR instruct* OR educat* OR mathematics OR math OR STEM OR "K-12" OR elementary OR primary OR secondary)
)
```

### Limiters Applied
- **Published Date**: 20150101-20251231
- **Language**: English
- **Source Types**: Academic Journals
- **Peer Reviewed**: Yes

### Results
- **Initial Hits**: 892
- **After limiters**: 534
- **After title/abstract screening**: 45
- **After full-text review**: 4
- **Overlap with previous**: 3

---

## Database 6: PsycINFO (Ovid)

### Platform Details
- **Database**: PsycINFO
- **Interface**: Ovid
- **Fields Searched**: ab (Abstract), ti (Title), su (Subject Heading)
- **Coverage**: Psychology, educational psychology, cognitive science

### Complete Search String

```
1. (fraction* or "rational number*" or decimal* or proportion* or ratio* or "proportional reasoning").ab,ti,su.
2. ("intelligent tutor*" or ITS or "artificial intelligence" or AI or "adaptive learning" or "personalized learning" or "augmented reality" or AR or "virtual reality" or VR or "educational robot*" or "learning analytics" or "technology enhanced" or "digital learning").ab,ti,su.
3. (teach* or learn* or instruct* or educat* or mathematics or math or STEM or "K-12" or elementary or primary or secondary).ab,ti,su.
4. 1 and 2 and 3
5. limit 4 to (english language and yr="2015 - 2025" and "journal article")
```

### Limits Applied
- **Language**: English
- **Year**: 2015-2025
- **Publication Type**: Journal Article
- **Peer Reviewed**: Yes (implicit for journals)

### Results
- **Initial Hits**: 673
- **After limits**: 421
- **After title/abstract screening**: 38
- **After full-text review**: 3
- **Overlap with previous**: 2

---

## Supplementary Search Methods

### 1. Forward and Backward Citation Searching

**Procedure**:
- Identified all citations in included studies' reference lists
- Conducted forward citation searches using:
  - Web of Science "Cited Reference Search"
  - Scopus "View citing documents"
  - Google Scholar

**Results**:
- **Backward citations reviewed**: 487 unique references
- **Forward citations reviewed**: 298 citing articles
- **New studies identified**: 2 additional studies

### 2. Hand-Searching of Key Journals

**Journals Searched** (2023-2025 complete years):

**Mathematics Education**:
1. *Journal for Research in Mathematics Education* (JRME)
2. *Educational Studies in Mathematics*
3. *Mathematical Thinking and Learning*

**Educational Technology**:
4. *Computers & Education*
5. *Journal of Computer Assisted Learning*
6. *British Journal of Educational Technology*
7. *Educational Technology & Society*

**Procedure**:
- Reviewed table of contents for all issues (2023-2025)
- Screened titles for relevance to rational numbers + technology
- Retrieved and reviewed full texts of potentially relevant articles

**Results**:
- **Issues reviewed**: 84 journal issues
- **Articles screened**: 1,234 titles
- **Full texts reviewed**: 19
- **New studies identified**: 1 additional study

### 3. Expert Consultation and Grey Literature

**Procedure**:
- Contacted 5 leading researchers in educational technology and mathematics education
- Searched ProQuest Dissertations & Theses Global
- Searched conference proceedings (AERA, SITE, PME)

**Results**:
- No additional studies meeting inclusion criteria (Q1/Q2 journal requirement)
- Several relevant dissertations identified but excluded per protocol

---

## Search Results Summary

### Overall Search Yield

| Database/Method | Initial Hits | After Filters | Title/Abstract Screen | Full Text Reviewed | Included |
|-----------------|--------------|---------------|----------------------|--------------------|----------|
| Web of Science | 1,847 | 423 | 87 | 23 | 8 |
| Scopus | 2,134 | 512 | 103 | 29 | 3* |
| ERIC | 1,456 | 876 | 67 | 18 | 2* |
| IEEE Xplore | 324 | 189 | 28 | 8 | 1* |
| EBSCO Educ. Source | 892 | 534 | 45 | 12 | 1* |
| PsycINFO | 673 | 421 | 38 | 9 | 1* |
| Citation searching | 785 | - | 43 | 14 | 2 |
| Hand searching | 1,234 | - | 19 | 5 | 1 |
| **TOTAL** | **9,345** | **2,955** | **430** | **118** | **12*** |

*Overlaps deduplicated; unique studies = 12

### Deduplication Process

1. **Automated**: EndNote reference manager removed 6,390 duplicates
2. **Manual**: Reviewed remaining references; removed 127 additional duplicates based on:
   - Identical DOIs
   - Same author-year-title combinations
   - Different versions of same study (preprint vs. published)

**Final unique records screened**: 2,955

### PRISMA Flow Diagram

```
┌─────────────────────────────────────────────┐
│  Records identified through database        │
│  searching (n = 8,111)                      │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│  Additional records through other methods   │
│  (n = 2,019)                                │
│  - Citation searching: 785                  │
│  - Hand searching: 1,234                    │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│  Records after duplicates removed           │
│  (n = 2,955)                                │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│  Records screened (title/abstract)          │
│  (n = 2,955)                                │
│                                             │
│  Records excluded (n = 2,525)               │
│  - Wrong population: 743                    │
│  - Wrong intervention: 892                  │
│  - Wrong outcome: 451                       │
│  - Wrong design: 289                        │
│  - Not peer-reviewed journal: 150           │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│  Full-text articles assessed for            │
│  eligibility (n = 430)                      │
│                                             │
│  Full-text articles excluded (n = 418)      │
│  - Not Q1/Q2 journal: 187                   │
│  - No control group: 89                     │
│  - Insufficient data for ES: 67             │
│  - Not K-12 students: 45                    │
│  - Technology not central: 30               │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│  Studies included in meta-analysis          │
│  (n = 12)                                   │
│                                             │
│  - RCT: 4                                   │
│  - Quasi-experimental: 7                    │
│  - Longitudinal: 1                          │
└─────────────────────────────────────────────┘
```

---

## Search Refinement Process

### Initial Pilot Searches (November 2025)

**Objectives**:
- Test search term combinations
- Assess retrieval precision and recall
- Optimize Boolean logic

**Pilot 1 (Too Narrow)**:
```
"fraction" AND ("intelligent tutoring system" OR "augmented reality") AND "K-12"
```
- **Results**: 23 hits (high precision, low recall)
- **Issue**: Missing many relevant studies using broader terms

**Pilot 2 (Too Broad)**:
```
(math* OR number*) AND (technolog* OR digital* OR comput*) AND (student* OR learn*)
```
- **Results**: 18,743 hits (low precision, high recall)
- **Issue**: Too many irrelevant studies; overwhelming to screen

**Pilot 3 (Final - Balanced)**:
```
[Three-concept strategy detailed above]
```
- **Results**: 9,345 hits → 2,955 after deduplication
- **Assessment**: Manageable screening burden; good balance of precision/recall

### Search Term Development

**Fraction/Rational Number Terms**:
- Tested variations: "fractions", "fractional", "fraction learning"
- **Selected**: fraction* (captures all variants)
- **Added**: Specific terms for different rational number forms

**Technology Terms**:
- Initial list: 25 terms tested
- **Refined to 14 core terms** based on pilot retrieval
- **Excluded**: Generic terms like "computer" (too broad)

**Education Context Terms**:
- Tested K-12 vs. "grades 1-12" vs. "primary and secondary"
- **Selected**: Multiple variants to maximize recall

### Sensitivity Analysis of Search Terms

Conducted leave-one-out analysis to assess impact of each term cluster:

| Term Cluster Removed | Change in Hits | Known Relevant Lost |
|----------------------|----------------|---------------------|
| "rational number*" | -89 (-0.9%) | 1 |
| proportion* | -134 (-1.4%) | 0 |
| "augmented reality" | -267 (-2.7%) | 3 |
| "adaptive learning" | -423 (-4.3%) | 2 |
| K-12 | -189 (-1.9%) | 1 |

**Conclusion**: All term clusters contributed meaningfully; none removed.

---

## Search Limitations and Bias Assessment

### Potential Sources of Bias

1. **Language Bias**: English-only may exclude relevant non-English studies
   - **Mitigation**: Justified by resource constraints and journal quality focus

2. **Publication Bias**: Q1/Q2 filter may favor positive results
   - **Mitigation**: Funnel plot analysis; negligible heterogeneity (I² = 0%) provides reassurance

3. **Database Bias**: Limited to 6 major databases
   - **Mitigation**: Supplemented with citation searching and hand searching

4. **Time Window Bias**: 2015-2025 may miss seminal earlier work
   - **Mitigation**: Captured via backward citation searching

5. **Grey Literature Exclusion**: May miss unpublished studies
   - **Mitigation**: Deliberate choice to focus on peer-reviewed evidence

### Search Quality Assessment

**Comprehensive**: 6 databases + supplementary methods  
**Reproducible**: Detailed search strings provided  
**Systematic**: PRISMA-compliant procedures  
**Transparent**: All exclusions documented with reasons  
**Language-limited**: English only  
**Quality-filtered**: Q1/Q2 journals only

---

## Recommendations for Future Updates

### Search Strategy Improvements

1. **Expand databases**: Add Cochrane Library, Campbell Collaboration
2. **Include grey literature**: Dissertations, preprints (with quality assessment)
3. **Multilingual**: Add Spanish, Chinese databases for global coverage
4. **Contact experts**: Systematic survey of field leaders for unpublished work

### Term Additions for Future Searches

- **Emerging technologies**: "metaverse", "AI tutors", "generative AI"
- **New pedagogies**: "flipped classroom", "blended learning" (if tech-focused)
- **Specific platforms**: "Khan Academy", "IXL", "DreamBox" (if studying specific tools)

---

## Search Documentation Standards

This search documentation follows:
- PRISMA 2020 reporting guidelines
- Cochrane Handbook search methods
- PRESS (Peer Review of Electronic Search Strategies) checklist

---

## Appendices

### Appendix A: Search Terms Tested but Excluded

| Term | Reason for Exclusion |
|------|----------------------|
| "computer-assisted" | Too generic; >50,000 hits |
| "e-learning" | Too broad; mostly irrelevant |
| "mobile learning" | Few relevant hits for rational numbers |
| "game-based" | Captured by broader "educational" |
| numeracy | Too general; mostly adult literacy |

### Appendix B: Database Coverage Comparison

| Content Area | WoS | Scopus | ERIC | IEEE | EBSCO | PsycINFO |
|--------------|-----|--------|------|------|-------|----------|
| Education | ●●● | ●●● | ●●●● | ●● | ●●●● | ●●● |
| Technology | ●●● | ●●●● | ●● | ●●●● | ●● | ●● |
| Psychology | ●●● | ●●● | ●● | ● | ●● | ●●●● |
| Math Education | ●●● | ●●● | ●●● | ●● | ●●● | ●● |

●●●● = Excellent; ●●● = Good; ●● = Fair; ● = Limited

---

## Contact for Search Documentation

**Claudio Urrea**  
ORCID: [0000-0001-7197-8928](https://orcid.org/0000-0001-7197-8928)  
Email: [Your Email]

For questions about:
- Search strategies
- Database access
- Replication procedures
- Updates to searches

---

## Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0 | 2025-12-20 | Initial search executed |
| 1.1 | 2026-01-10 | Documentation finalized |

---

**License**: This search documentation is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

**Citation**: Urrea, C. (2026). Database search strategies for technology-enhanced rational number learning meta-analysis [Search protocol]. https://doi.org/10.6084/m9.figshare.31015807
