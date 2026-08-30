# Bibliometric dataset for Fig. 1

Record identifiers and annual counts behind the bibliometric analysis shown in
Fig. 1 of the article. The search strategy, screening rules and classification
criteria are reported in the Supporting Information of the article; this
repository holds the record identifiers so that the analysed set can be
recovered exactly.

## Source

Records were retrieved from the Web of Science Core Collection on 12 March 2026,
by a topic search combining drinking water with odour terms, covering 1995 to
2026, with no restriction on document type, language or subject category.

Records for 2026 cover 1 January to 12 March 2026, a partial year of 71 days,
and are marked as such in Fig. 1C.

## From retrieval to the analysed set

| Step | Records | File |
|---|---|---|
| Retrieved | 2,500 | `retrieved_2500_accessions.txt` |
| Duplicates removed | 1,086 | `duplicates_removed_1086.csv` |
| Unique records analysed | **1,414** | `accession_doi_year.csv` |

The annual export files cover overlapping date ranges, so the combined download
contains repeated records. Duplicates were removed by accession number, then by
DOI, then by normalized title and year. The three counts are consistent:
2,500 − 1,086 = 1,414.

## Files

| File | Contents |
|---|---|
| `accession_doi_year.csv` | The 1,414 unique records: accession number, DOI, publication year |
| `annual_counts_1995_2026.csv` | Records per year, the direct source for Fig. 1C |
| `retrieved_2500_accessions.txt` | Accession numbers of the 2,500 retrieved records, one per line |
| `duplicates_removed_1086.csv` | Accession number and DOI of the 1,086 entries removed as duplicates |

All 1,414 records carry an accession number. DOIs are present for 1,320 of them;
the remainder were published mostly before 2000, when DOIs were not yet in
general use. The accession number is therefore the primary identifier.

## Annual counts

The counts in `annual_counts_1995_2026.csv` sum to 1,414. Two figures quoted in
the article can be checked directly against this file: the 1995 to 2005 subtotal
is 277, and 2026 contributes 23 records.

## Recovering the records

Only identifiers are deposited here. Web of Science records are licensed
content, so full bibliographic records are not redistributed. Readers with Web of
Science access can recover the analysed set exactly by searching the accession
numbers listed in `accession_doi_year.csv`, which returns the same 1,414 records.

Re-running the original search instead of using the accession numbers will not
reproduce the set, because the database grows over time: a repeat search on
27 August 2026 returned 1,535 records against the original 1,414. The accession
numbers are therefore the reproducible route.
