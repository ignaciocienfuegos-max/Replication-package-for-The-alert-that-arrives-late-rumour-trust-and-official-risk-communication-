# Replication package

**"The alert that arrives late: rumour, trust and official risk communication across four Chilean disasters, 2010–2026"**
Ignacio Cienfuegos, Facultad de Gobierno, Universidad de Chile
Package assembled 4 September 2026 for submission to the *International Journal of Disaster Risk Reduction*.

This package contains everything behind the manuscript's four case timelines, cross-case coding and matrix, and figures/tables — except the raw survey microdata that data providers' terms do not allow to be redistributed. For those datasets (Subtel, ELSOC, Termómetro Social), this package gives the exact citation, the exact download source, and the derived, aggregated data actually used in the article, so every number in the paper can be traced and every figure regenerated once the researcher has obtained their own copy of the microdata.

## Contents

```
README.md                              — this file
timelines/                             — the four case timelines (evidentiary basis for §6 Results)
  timeline_27F_earthquake_tsunami.md
  timeline_covid19_chile.md
  timeline_2024_valparaiso_fire.md
  timeline_2026_norte_grande_floods.md
coding_and_matrix/
  coding_rubric_v1.md                  — the CERC x best-practice coding scheme applied to all four cases
  cross_case_matrix_v1.md              — Tables A-D: the 4x5 CERC matrix, latency measures, cross-case
                                          patterns, and the change/no-change comparison (§6.1-6.3 basis)
figures/
  data/                                — derived, aggregated data behind Figures 1-3 and Table 3
    fig1_subtel2024_channel_use.csv
    fig2_elsoc_trust_2016_2022.csv
    fig3_platforms_news_2017_2023.csv
    table1_ts3.md
    table1_ts3_sources_trust.csv
  out/                                 — rendered figures and the consolidated data workbook
    Figure1_channel_use_2024.png / .pdf
    Figure2_trust_2016_2022.png / .pdf
    Figure3_platforms_news_2017_2023.png / .pdf
    IJDRR_figure_data_v1.xlsx          — every number behind Figures 1-3 and Table 3, with n
  scripts/                             — regenerate the derived data and figures from raw microdata
    prep_data.py
    make_figures.py
cigiden/                               — CIGIDEN Barómetro Ciudadano del Desastre (2019), supplied
                                          by CIGIDEN in aggregate, chart-ready form, September 2026
  CIGIDEN_Barometro_2019_datos_para_graficos.xlsx
  CIGIDEN_Barometro_2019_Resultados_Generales.pptx
```

## 1. The four case timelines

Each timeline is a three-track (official / hazard-monitoring / public-information-environment) chronological reconstruction of one case, built from the sources listed in that file's own header, with a source and a confidence rating (High/Medium/Low) on every row, and a closing section listing unresolved contradictions in the record. These are the primary evidentiary base for the manuscript's §6 Results section and for every dated claim, quotation and figure in the case narratives.

- **`timeline_27F_earthquake_tsunami.md`** — 27 February 2010 earthquake and tsunami. ~110 sources: the 2010 Cámara de Diputados commission testimonies, the Armada/SHOA report, the IOC/UNESCO post-event assessment, the Fiscalía's formalisation and court record (2012-2025), CIPER's 2012 reconstruction, Mendoza, Poblete & Castillo (2010), the UN inter-agency mission report, and press 2010-2025.
- **`timeline_covid19_chile.md`** — COVID-19, March 2020-September 2021. 108 sources: BCN/Ley Chile decrees, MINSAL and Presidencia releases, Cámara and Senate records, Contraloría, CIPER, national press, fact-checkers, opinion polls and five Chilean academic studies of pandemic communication. Episode-based, not minute-by-minute.
- **`timeline_2024_valparaiso_fire.md`** — February 2024 Valparaíso-Viña del Mar mega-fire. ~90 sources: official documents, investigative reporting, CIGIDEN/WildfireX field reports, the Fiscalía and PDI reconstructions as reported, and SENAPRED's timestamped X posts.
- **`timeline_2026_norte_grande_floods.md`** — 16-19 August 2026 Norte Grande floods. 130 sources (~95 read in full): SENAPRED regional alert notices and national balances, DMC avisos/alertas/alarma, Ministerio del Interior decree DS 134, Cooperativa's live blogs, the regional press of Tarapacá and Antofagasta, national press and TV, Mala Espina's fact-checks, and municipalities' own reports. This case was 15 days old when the timeline was built (3 September 2026); its Stage V (evaluation) is empty and every count is provisional pending SENAPRED's consolidated report — a limitation stated explicitly in the manuscript (§7.5).

## 2. Coding rubric and cross-case matrix

**`coding_and_matrix/coding_rubric_v1.md`** (v1.1, 3 September 2026) defines the unit of analysis (an official communicative act), the coded variables (CERC stage, content type, specificity 0-5, consistency with the monitoring record, reception, uncertainty acknowledgement, self-efficacy, honesty/openness, listening, orientation, SCCT strategy, rumour response), and the five latency measures (L1 hazard-to-alert through L5 event-to-evaluation). Its sources are Reynolds & Seeger (2005), Seeger (2006), Veil, Buehner & Palenchar (2011), Wendling et al. (2013), Mileti & Sorensen (1990), Mileti & O'Brien (1992), Eckert et al. (2018) and Peña y Lillo & Rosenberg (2024) — full citations in the manuscript's reference list.

**`coding_and_matrix/cross_case_matrix_v1.md`** (v1.0, 3 September 2026) applies the rubric across all four cases and assembles: Table A, the 4x5 CERC-stage matrix (what the official system did / what the public information environment did, in each of the five stages, for each case); Table B, latency measures L1-L5 by case; Table C, cross-case patterns; Table D, the change/no-change comparison across 2010-2026. Every cell is traceable to a specific row in the corresponding timeline file; cells marked with an empty-set symbol are empty because the historical record is empty, not because the stage did not occur.

## 3. Figures and Table 3 — survey data

`figures/figures_and_tables_v1.md` (not included as a separate file here; its captions and "what it shows" text are reproduced in the manuscript) documents the three figures and Table 3 in full. Summary:

- **Figure 1** — Channel ecology, Chile 2024. Source: **Subtel, XI Encuesta de Acceso, Usos y Usuarios de Internet 2024** (n = 4,418 persons; person weights). WhatsApp chat, social-network use, and reading news online, by age group and by region.
- **Figure 2** — Institutional trust, Chile 2016-2022. Source: **ELSOC 2016-2022 (COES)**, cross-sectional weights (n per point 2,450-3,740). Percentage answering "bastante" or "mucha confianza" in each of a set of institutions, wave by wave.
- **Figure 3** — Platforms used to inform oneself about current affairs, 2017 vs 2023. Source: **Subtel, IX (2017, n = 3,033) and X (2023, n = 4,696) Encuesta de Acceso y Uso de Internet**, module S3.3, person weights.
- **Table 3** — Information sources and trust during the first pandemic winter. Source: **Termómetro Social, round 3 (TS3), 30 May-10 June 2020** (n = 1,078, telephone, weight `factor`).

`figures/data/` holds the derived, aggregated CSVs actually plotted (`fig1_subtel2024_channel_use.csv`, `fig2_elsoc_trust_2016_2022.csv`, `fig3_platforms_news_2017_2023.csv`) and the Table 3 data (`table1_ts3.md`, `table1_ts3_sources_trust.csv`). `figures/out/` holds the rendered PNG (300 dpi) and PDF versions of each figure, plus `IJDRR_figure_data_v1.xlsx`, a single workbook with every number behind Figures 1-3 and Table 3, with sample sizes.

### Regenerating the figures

`figures/scripts/prep_data.py` and `figures/scripts/make_figures.py` reproduce the CSVs and figures from the raw microdata. **They will not run as-is**: the raw Subtel, ELSOC and Termómetro Social microdata files are not included in this package, per the data providers' redistribution terms. To regenerate:

1. Obtain the raw microdata yourself from the sources below.
2. Edit the file paths at the top of `prep_data.py` to point to your local copies.
3. Run `python3 prep_data.py` (requires `pyreadstat`, `pandas`, `numpy`) to regenerate the CSVs in `figures/data/`.
4. Run `python3 make_figures.py` to regenerate the PNG/PDF figures in `figures/out/`.

**Where to obtain the raw microdata:**

| Dataset | Citation | Source / download |
|---|---|---|
| Subtel Encuesta de Acceso y Uso de Internet, waves IX (2017), X (2023), XI (2024) | Subtel (Subsecretaría de Telecomunicaciones), *Encuesta de Acceso, Usos y Usuarios de Internet*, various years | https://www.subtel.gob.cl/estudios-y-estadisticas/ (public download, no registration) |
| ELSOC (Estudio Longitudinal Social de Chile) 2016-2022, v1.00 | Centro de Estudios de Conflicto y Cohesión Social (COES), *ELSOC 2016-2022* | Harvard Dataverse, doi:10.7910/DVN/QZEDUC (public download; codebook is a separate file on the same Dataverse page) |
| Termómetro Social, rounds 1 and 3 (TS1, TS3) | Centro de Microdatos, Universidad de Chile, *Termómetro Social* | https://www.microdatos.cl (public download, no registration) |

## 4. CIGIDEN Barómetro Ciudadano del Desastre (2019)

`cigiden/` contains the two files supplied directly by CIGIDEN (Centro de Investigación para la Gestión Integrada del Riesgo de Desastres) on 4 September 2026, in response to a data request sent 2 September 2026:

- **`CIGIDEN_Barometro_2019_datos_para_graficos.xlsx`** — chart-ready aggregate cross-tabulations (20 sheets).
- **`CIGIDEN_Barometro_2019_Resultados_Generales.pptx`** — the results presentation (40 slides).

**These are aggregate, chart-ready results tables, not respondent-level microdata.** CIGIDEN did not provide microdata, and none is included here. The survey itself: *Barómetro Ciudadano del Desastre*, CIGIDEN / Facultad de Comunicaciones UC, online non-probability panel, n = 970, fielded 1-21 May 2019. Full extracted findings and methodology notes are in the manuscript's Table 2 (data sources) and §6.1 (results); a fuller data note is `claude/data-cigiden-barometro-notes.md` in the project's document store. Citation for the manuscript's reference list: CIGIDEN, Facultad de Comunicaciones UC (2019), *Barómetro Ciudadano del Desastre*, online survey, n = 970, fielded 1-21 May 2019, results tables and presentation deck supplied by CIGIDEN, September 2026.

Because the panel is non-probability and skewed toward the capital and toward the university-educated, all Barómetro-based claims in the manuscript are qualified accordingly (§7.5 Limitations).

## 5. What is deliberately not included

- Raw Subtel, ELSOC or Termómetro Social **microdata** — publicly downloadable from the sources in the table above; not redistributed here per those providers' terms.
- CIGIDEN respondent-level **microdata** — not supplied by CIGIDEN; only the aggregate tables above exist.
- The manuscript text itself, references, front matter and cover letter — submitted separately to the journal.

## 6. Citing this package

A DOI for this package (via Zenodo or OSF) will be added here and in the manuscript's Data Availability statement once deposited. Until then, cite as: Cienfuegos, I. (2026). Replication package for "The alert that arrives late: rumour, trust and official risk communication across four Chilean disasters, 2010-2026." Unpublished, prepared for submission to the *International Journal of Disaster Risk Reduction*.
