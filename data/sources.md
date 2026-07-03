# Data Sources

This document compiles and consolidates the authoritative data sources identified for the
Apollo (University of Cambridge Repository) project. Each entry records bibliographic
metadata (title, author/publisher, year, URL, DOI where available), access and license
terms, and links to raw data where available.

Related issue: [Collect data from sources (#1)](https://github.com/jvzhu/Apollo---University-of-Cambridge-Repository/issues/1)

---

## 1. Institutional Repositories

### 1.1 Apollo — University of Cambridge Repository

- **Title:** Apollo, the institutional repository of the University of Cambridge
- **Author/Publisher:** University of Cambridge, Cambridge University Libraries (Office of Scholarly Communication)
- **Year:** 2003–present (ongoing)
- **URL:** https://www.repository.cam.ac.uk/
- **DOI:** Individual records are assigned DataCite DOIs with the prefix `10.17863`
- **Raw data access:** OAI-PMH endpoint at https://www.repository.cam.ac.uk/server/oai/request; REST API available via the DSpace 7 API
- **License/usage:** Metadata is generally reusable (CC0 for most records); item-level content licensing varies per deposit (many items under Creative Commons licenses, some under all-rights-reserved). Check the license field on each record.

### 1.2 Cambridge University Library Catalogue (iDiscover)

- **Title:** iDiscover — Cambridge Libraries catalogue
- **Author/Publisher:** Cambridge University Libraries
- **Year:** Ongoing
- **URL:** https://idiscover.lib.cam.ac.uk/
- **DOI:** N/A (catalogue records; linked resources may carry DOIs)
- **Raw data access:** Public search interface; bulk access requires arrangement with the library
- **License/usage:** Catalogue freely searchable; reuse of bibliographic records subject to library terms

### 1.3 Cambridge Digital Library

- **Title:** Cambridge Digital Library
- **Author/Publisher:** Cambridge University Library
- **Year:** 2011–present
- **URL:** https://cudl.lib.cam.ac.uk/
- **DOI:** N/A (item-level persistent URLs provided)
- **Raw data access:** IIIF image API and metadata available per collection; some collection metadata published on GitHub (https://github.com/cambridge-collection)
- **License/usage:** Varies by collection; many images under CC BY-NC 3.0. Check the rights statement on each item.

## 2. Aggregators and Academic Databases

### 2.1 DataCite

- **Title:** DataCite Metadata Store / DataCite Commons
- **Author/Publisher:** DataCite e.V.
- **Year:** 2009–present
- **URL:** https://commons.datacite.org/ (API: https://api.datacite.org/)
- **DOI:** DOI registration agency; metadata for all registered DOIs (including Apollo's `10.17863` prefix)
- **Raw data access:** Open REST API (JSON); public data file releases
- **License/usage:** Metadata released under CC0 1.0

### 2.2 Crossref

- **Title:** Crossref Metadata API
- **Author/Publisher:** Crossref
- **Year:** 2000–present
- **URL:** https://www.crossref.org/ (API: https://api.crossref.org/)
- **DOI:** DOI registration agency for scholarly publications
- **Raw data access:** Open REST API (JSON); annual public data files
- **License/usage:** Metadata facts are openly reusable; API usage subject to polite-use guidelines

### 2.3 CORE

- **Title:** CORE — Aggregator of open access research papers
- **Author/Publisher:** The Open University / Jisc
- **Year:** 2011–present
- **URL:** https://core.ac.uk/
- **DOI:** Reference paper: Knoth & Zdrahal, "CORE: Three Access Levels to Underpin Open Access", D-Lib Magazine, 2012 — https://doi.org/10.1045/november2012-knoth
- **Raw data access:** REST API (registration required for API key); bulk dataset dumps available
- **License/usage:** API free for research/non-commercial use; dataset dumps under ODC-By

### 2.4 OpenDOAR

- **Title:** OpenDOAR — Directory of Open Access Repositories
- **Author/Publisher:** Jisc
- **Year:** 2005–present
- **URL:** https://v2.sherpa.ac.uk/opendoar/
- **DOI:** N/A
- **Raw data access:** REST API (free API key required)
- **License/usage:** CC BY-NC-ND 4.0 for the directory data

### 2.5 Google Scholar

- **Title:** Google Scholar
- **Author/Publisher:** Google LLC
- **Year:** 2004–present
- **URL:** https://scholar.google.com/
- **DOI:** N/A (indexes works that may carry DOIs)
- **Raw data access:** No official API; manual search and citation export only
- **License/usage:** Terms of Service prohibit automated scraping; use for manual discovery and citation lookup only

### 2.6 OpenAIRE

- **Title:** OpenAIRE Graph
- **Author/Publisher:** OpenAIRE AMKE
- **Year:** 2010–present
- **URL:** https://graph.openaire.eu/
- **DOI:** https://doi.org/10.5281/zenodo.3516917 (OpenAIRE Research Graph dump)
- **Raw data access:** Public APIs and full graph dumps on Zenodo
- **License/usage:** Graph dumps under CC BY 4.0

## 3. Published Papers and Reference Works

### 3.1 DSpace Platform (Apollo's underlying software)

- **Title:** "DSpace: An Open Source Dynamic Digital Repository"
- **Author/Publisher:** MacKenzie Smith et al.
- **Year:** 2003
- **URL:** http://www.dlib.org/dlib/january03/smith/01smith.html
- **DOI:** https://doi.org/10.1045/january2003-smith
- **Raw data access:** N/A (reference article)
- **License/usage:** D-Lib Magazine article, freely accessible; DSpace software is BSD-licensed (https://github.com/DSpace/DSpace)

### 3.2 Open Access at Cambridge

- **Title:** University of Cambridge Open Access policies and guidance
- **Author/Publisher:** Cambridge University Libraries, Office of Scholarly Communication
- **Year:** Ongoing
- **URL:** https://www.openaccess.cam.ac.uk/
- **DOI:** N/A
- **Raw data access:** N/A
- **License/usage:** Public guidance pages; consult individual policy documents for reuse terms

---

## Data Quality and Coverage Notes

| Source | Coverage | Quality notes |
| --- | --- | --- |
| Apollo | Cambridge research outputs (articles, theses, datasets) from ~2003 | Authoritative for Cambridge outputs; metadata quality high, DOIs minted via DataCite; some legacy records have sparse metadata |
| iDiscover | Cambridge library holdings | Comprehensive catalogue; bibliographic records only, no full text |
| Cambridge Digital Library | Digitised special collections | High-quality curated metadata and IIIF images; coverage limited to digitised collections |
| DataCite | All DataCite-registered DOIs globally | Excellent for dataset metadata; completeness depends on depositor input |
| Crossref | Scholarly publications with Crossref DOIs | Very broad coverage of journal literature; dataset coverage limited |
| CORE | Open access full texts aggregated worldwide | Large full-text corpus; deduplication imperfect, metadata quality varies by source repository |
| OpenDOAR | Repository-level directory | Useful for discovering further repositories; not item-level data |
| Google Scholar | Broad scholarly index | Widest discovery coverage; no bulk access, citation counts not fully transparent |
| OpenAIRE | EU-funded and open access research | Strong linkage between publications, datasets, and funding; European emphasis |

## Access and License Verification Status

- [x] Apollo — open access, verified 2026-07
- [x] DataCite API — CC0 metadata, verified 2026-07
- [x] Crossref API — open, verified 2026-07
- [x] CORE — API key required (free registration), verified 2026-07
- [x] OpenDOAR — API key required (free registration), verified 2026-07
- [x] Google Scholar — manual use only (no API), verified 2026-07
- [x] OpenAIRE — open dumps and APIs, verified 2026-07
- [ ] Restricted datasets — none identified yet; contact relevant data owners if restricted sources are added later

## Next Steps

1. Harvest an initial metadata sample from Apollo via OAI-PMH and store it under `data/`.
2. Cross-reference Apollo DOIs against DataCite for metadata completeness checks.
3. Add new sources here as they are identified, following the entry format above (title, author, year, URL, DOI, raw data access, license/usage).
