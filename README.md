# deRSE Qualitative Methods Review

A lightweight review of practices methods in German RSE publications, focusing on qualitative methods practice.

## Aim of the Study

This study maps the empirical research methodologies used in recent publications of the German Research Software Engineering (deRSE) community.
The purpose is descriptive rather than confirmatory and examines the following:

* which empirical methodologies are represented;
* how frequently qualitative and mixed-method approaches occur;
* which forms of qualitative evidence are used;
* how explicitly qualitative methodology is reported;
* whether qualitative approaches are concentrated in particular topics or disciplinary contexts.

The resulting evidence may support a broader discussion about methodological competencies and representation within RSE.

## Corpus

**Sources:** 
- proceedings 2026: TBA
- proceedings 2025: https://eceasst.org/index.php/eceasst/issue/view/207
- proceedings 2024: https://eceasst.org/index.php/eceasst/issue/view/205
- Zenodo community: https://zenodo.org/communities/de-rse/records

**Time period:** `2024`–`2026`

**Unit of analysis:** one published contribution.

### Inclusion criteria

Include publications that:

* are part of the selected sources list
* contain a substantive research or experience-based contribution
* are available in full text

### Exclusion criteria

Exclude:

* editorials, prefaces, schedules, abstracts without full papers, and similar non-research material;
* duplicates;
* working group papers, working papers, white papers, etc. that do not include a formal research method
* contributions for which the full text cannot be obtained.

All included and excluded publications are recorded. Exclusions must contain a short reason.

## 3. Research Questions

**RQ1.** Which research methodologies are represented in recent deRSE publications?

**RQ2.** Which publications involve human participants or other qualitatively interpretable evidence?

**RQ3.** Which qualitative and mixed-method approaches are used?

**RQ4.** How explicitly are qualitative data collection and analysis procedures methodologically reported?

**RQ5.** Are qualitative approaches associated with particular topics, contribution types, or disciplinary contexts?

## 4. Extraction Scheme

For each publication, record at least the following variables:

| Variable                       | Values / description                                                                                                                                                                                        |
| ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `id`                           | Stable study-specific identifier                                                                                                                                                                            |
| `year`                         | Publication year                                                                                                                                                                                            |
| `title`                        | Publication title                                                                                                                                                                                           |
| `doi`                          | DOI, if available                                                                                                                                                                                           |
| `contribution_type`            | empirical study / experience report / software or tool / infrastructure / conceptual or methodological / other                                                                                              |
| `empirical`                    | yes / no                                                                                                                                                                                                    |
| `human_involvement`            | none / users as evaluators / survey respondents / interview participants / observation or ethnographic involvement / participatory or co-design / other                                                     |
| `evidence_source`              | benchmark / repository or log data / structured survey / free-text survey / interview / focus group / observation / documents or text / images / material artefacts / software artefacts / other / multiple |
| `methodological_orientation`   | quantitative / qualitative / mixed methods / computational or technical evaluation / descriptive experience report / unclear / not applicable                                                               |
| `data_collection_method`       | free text; use normalized terminology where possible                                                                                                                                                        |
| `analysis_method`              | e.g. statistical analysis, thematic analysis, qualitative content analysis, grounded theory, coding without named methodology                                                                               |
| `qualitative_method_named`     | yes / no / not applicable                                                                                                                                                                                   |
| `method_reference_provided`    | yes / no / not applicable                                                                                                                                                                                   |
| `sampling_described`           | yes / partly / no / not applicable                                                                                                                                                                          |
| `analysis_procedure_described` | yes / partly / no / not applicable                                                                                                                                                                          |
| `quality_or_rigor_discussed`   | yes / partly / no / not applicable                                                                                                                                                                          |
| `disciplinary_context`         | discipline/domain named by the paper                                                                                                                                                                        |
| `research_topic`               | short normalized category                                                                                                                                                                                   |
| `notes`                        | relevant methodological observations                                                                                                                                                                        |

Do not infer a methodology merely from the presence of interviews, open-text answers, or human participants.

## Qualitative-Method Reporting Scale

For publications using qualitative evidence, classify methodological reporting as:

**0 — No methodological specification**
Qualitative material is used, but no recognizable analysis procedure is described.

**1 — Technique mentioned**
The paper mentions activities such as coding, categorization, or interview analysis but gives little methodological detail.

**2 — Method identified**
A recognizable qualitative method or analytical approach is named and sufficiently described.

**3 — Methodologically substantiated**
The method is named, described, appropriately referenced, and accompanied by relevant methodological considerations such as sampling, analytic procedure, reflexivity, triangulation, or quality criteria.

The scale evaluates **reporting**, not the intrinsic quality of the research.

## Report Analysis

Primary analysis is descriptive.

Report at least:

* number of included publications per year;
* proportion of empirical and non-empirical contributions;
* distribution of methodological orientations;
* frequency of different evidence sources;
* number and proportion of qualitative and mixed-method studies;
* qualitative methods used;
* methodological reporting scores;
* distribution across research topics and disciplinary contexts.

Avoid treating publication counts as evidence about the competence of individual RSE practitioners.

Where useful, cross-tabulate:

* methodology × year;
* methodology × contribution type;
* qualitative methodology × disciplinary context;
* human involvement × methodological orientation;
* qualitative evidence × reporting score.

## Interpretation Boundaries

The study concerns the **selected deRSE publication corpus**.

It does not by itself establish:

* the methodological composition of RSE globally;
* the methodological competence of individual RSEs;
* the prevalence of unpublished qualitative work;
* the methods used in RSE projects that do not result in conference publications.

Possible findings should therefore be phrased as evidence about **publication practice and methodological representation in the investigated corpus**.

The study should explicitly report counterevidence, including well-developed qualitative, mixed-method, humanities, archaeological, participatory, or other interpretive approaches.

## Reproducibility Requirements

The repository should contain:

* the exact corpus definition;
* retrieval date;
* source URLs or persistent identifiers;
* inclusion and exclusion decisions;
* versioned codebook;
* raw reviewer classifications;
* resolved classifications;
* analysis scripts;
* software/dependency versions;
* instructions for reproducing tables and figures.

Where redistribution of article PDFs is not permitted, store only bibliographic metadata, persistent identifiers, and retrieval instructions.

## Collaboration Workflow

1. Create an issue for methodological changes or unresolved classification questions.
2. Use pull requests for changes to the protocol, codebook, extraction data, or analysis.
3. Never silently change coding rules during extraction.
4. Record substantive protocol deviations.
5. Preserve individual reviewer assessments before consensus resolution.
6. Add new categories only when existing categories clearly fail to represent the evidence.
7. Prefer `unclear` plus a review note over unsupported inference.

## Minimal Reproduction Workflow

A reproducer should be able to:

1. obtain the corpus from the documented ECEASST proceedings;
2. verify the included publication list;
3. inspect the complete coding scheme;
4. access reviewer-level and resolved extraction data;
5. run the analysis scripts;
6. regenerate all reported counts, tables, and figures.

## Expected Outputs

The study should produce:

* a documented corpus of recent deRSE publications;
* an openly reusable methodology-classification scheme;
* descriptive statistics of methodological practice;
* a mapping of qualitative and mixed-method use;
* an assessment of how explicitly qualitative methodology is reported;
* evidence both supporting and challenging claims of methodological underrepresentation in RSE.

## Open Science

Where legally and ethically possible, the protocol, extraction data, analysis scripts, and derived results should be openly published and versioned.

A release used for a publication should be archived with a persistent identifier, for example through Zenodo.

The protocol and analysis decisions should be fixed before interpreting the results in relation to the proposed qualitative-research working group.


## Resources
- historical RSE events:  https://de-rse.org/en/events
