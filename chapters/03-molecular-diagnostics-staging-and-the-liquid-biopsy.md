# Molecular Diagnostics, Staging, and the Liquid Biopsy

## Learning Objectives

After working through this chapter, you should be able to:

- **Distinguish** analytic validity, clinical validity, and clinical utility, and explain why a test can pass the first and fail the third.
- **Explain** the logic of a companion diagnostic and why pairing a biomarker with a drug changes how the test must be evaluated.
- **Interpret** the TNM staging system and tumor grade as structured summaries of disease extent and biology, and explain why staging now incorporates molecular factors.
- **Evaluate** the strengths and limits of liquid biopsy (ctDNA) — comprehensive sampling and repeatability versus low shedding, clonal hematopoiesis, and unproven utility for some uses.
- **Judge** when a positive molecular result should change a treatment decision and when it should not.

## Opening Case

A 67-year-old man with metastatic non-small-cell lung adenocarcinoma has insufficient tissue left from his biopsy for full molecular profiling. His oncologist orders a blood-based **liquid biopsy** — a circulating tumor DNA (ctDNA) panel — hoping to find a targetable mutation. The report comes back flagging a *DNMT3A* mutation and a *TP53* mutation, but none of the classic targetable lung drivers (no EGFR, ALK, ROS1, KRAS G12C). A trainee reads the report and asks whether the *DNMT3A* finding means the patient should be referred for a hematologic workup, since *DNMT3A* mutations are common in blood cancers.

The oncologist pauses. *DNMT3A* is indeed a cancer gene — but it is also one of the most common mutations in **clonal hematopoiesis**, the age-related expansion of mutated blood-cell clones that has nothing to do with the lung tumor. The ctDNA assay cannot, by itself, tell whether that mutation came from the tumor or from the patient's own aging blood cells. Acting on it as a tumor finding would send the patient down a pointless and frightening path.

Worse, the *absence* of a targetable driver is also ambiguous. If the tumor is shedding little DNA into the blood, the panel could be reporting a clean result on an inadequate sample — a false negative driven not by the test's design but by tumor biology. The molecular report looks authoritative. Whether it should change a single decision depends on questions the report does not answer: where did each signal come from, and how much tumor DNA was actually in the tube? This chapter is about those questions — the difference between a test that *measures* something and a test that *should change what you do*.

## Core Concepts

### Three kinds of validity, and why utility is the hard one

A molecular test can be evaluated at three levels, and conflating them is the central error this chapter guards against.

- **Analytic validity:** Does the assay accurately measure what it claims to measure? If the report says *EGFR exon 19 deletion present*, is that deletion really in the sample, reproducibly, with known limits of detection? This is a laboratory question about the instrument.
- **Clinical validity:** Does the measured result correlate with a clinical state or outcome? Does the *EGFR* deletion actually predict that the tumor will respond to an EGFR inhibitor?
- **Clinical utility:** Does *using* the test to guide decisions improve patient outcomes compared with not using it? Does ordering the test, and acting on it, lead to longer life or better quality of life?

A test can be analytically perfect (it measures the mutation flawlessly) and clinically valid (the mutation predicts response) yet still lack demonstrated utility if acting on it does not improve outcomes — or if the action it implies is harmful, costly, or unavailable. Utility is the highest bar and the one most often skipped. The FDA's recent oncology emphasis on confirmatory evidence and "meaningful clinical benefit" is precisely an insistence on utility over mere measurement [FDA, *Oncology Center of Excellence*; NCI, *Research Areas: Cancer Diagnosis*]. In the Opening Case, the *DNMT3A* finding has analytic validity (the mutation is really in the plasma DNA) but no clinical validity *as a lung-tumor marker*, because it likely came from blood cells, not tumor.

### Companion diagnostics: the test is part of the drug

A **companion diagnostic** is a test that determines whether a specific drug is likely to work in a specific patient. The FDA increasingly approves a drug together with its companion diagnostic, so the test is effectively required for the drug [source chapter]. This couples the test's evaluation to the drug's: the relevant evidence is no longer "does the test measure the biomarker?" but "do biomarker-positive patients, identified by *this* test, benefit from *this* drug?"

Canonical biomarker–drug pairs include HER2 (IHC/FISH) for HER2-targeted antibodies in breast and gastric cancer; EGFR mutations for EGFR inhibitors in lung cancer; BRAF V600E for BRAF inhibitors in melanoma; BRCA1/2 for PARP inhibitors; and the tumor-agnostic markers — microsatellite instability and NTRK fusions — where the same drug works across tumor types if the molecular feature is present [source chapter]. The infrastructure behind these tests is **next-generation sequencing (NGS)**: high-throughput parallel sequencing that reads millions of short DNA fragments, enabling **comprehensive genomic profiling (CGP)** across hundreds of genes from a single specimen.

### Staging: TNM and the move toward biology

Once cancer is confirmed, **staging** describes its extent. The dominant system is **TNM**, maintained by the American Joint Committee on Cancer (AJCC) [AJCC Cancer Staging Manual, 8th ed., 2017]: **T** for primary tumor size/invasion, **N** for regional lymph nodes, **M** for distant metastasis. The categories combine into stage groups (0–IV) that summarize prognosis and standardize communication. **Clinical staging** uses pre-surgical information; **pathological staging** uses the resected specimen and often upstages, because surgery reveals disease that imaging missed.

Crucially, staging has begun absorbing **non-anatomical factors**. The AJCC 8th edition formally incorporates hormone-receptor status, HER2, and Oncotype DX recurrence score into breast cancer *prognostic stage groups*, and PSA and Gleason score into prostate staging [AJCC 8th ed.]. This reflects a measurement insight: anatomic extent alone does not fully capture prognosis, so biology is now part of the ruler.

Separately, **grade** measures how closely tumor cells resemble normal tissue (well- to poorly differentiated; Gleason score for prostate, Nottingham grade for breast). Stage is *how much*; grade is *how aggressive-looking*.

<!-- → [DIAGRAM: TNM components combining into stage groups, with a sidebar showing where molecular factors (ER/PR, HER2, PSA, Gleason) now enter] -->

### Liquid biopsy: what blood can and cannot tell you

**Liquid biopsy** detects and characterizes cancer from blood, mainly via **circulating tumor DNA (ctDNA)** — fragments shed by tumor cells that carry the tumor's mutations [NIH Research Matters, *Detecting cancer*]. Its advantages are real: it samples DNA from across the whole tumor and metastatic sites (averaging out the spatial heterogeneity that defeats a single needle); it is easily repeatable for monitoring; and it works when tissue is unavailable. Established uses include genomic profiling when tissue is insufficient, resistance monitoring (detecting EGFR T790M emergence to trigger a drug switch), and **minimal residual disease (MRD)** detection — finding microscopic disease after curative-intent surgery that imaging cannot see, which is reshaping adjuvant decisions in colorectal cancer (the DYNAMIC trial showed MRD-guided care reduced chemotherapy use without compromising outcomes) [DYNAMIC trial].

But the limits are exactly the failure modes in the Opening Case:

- **Low shedding.** Small, early-stage tumors and brain tumors release little ctDNA. A negative result may reflect inadequate sampling, not absent disease — a biology-driven false negative.
- **Clonal hematopoiesis.** Mutations in plasma DNA can come from age-related mutated blood-cell clones (e.g., *DNMT3A*, *TP53*), not tumor. Distinguishing tumor signal from this background requires care.
- **No spatial information.** ctDNA gives molecular features but not the architecture, grade, and margin information that tissue pathology provides.
- **Unproven utility for some uses.** Resistance monitoring and tissue-substitute profiling are well established; MRD-guided therapy is maturing; but multi-cancer early detection from ctDNA remains under prospective evaluation [contested — see pantry flag].

## Worked Example

**Situation.** A patient with newly diagnosed metastatic colon cancer has surgery with curative intent. Postoperatively, the team must decide whether to give adjuvant chemotherapy, which has real toxicity. A ctDNA MRD assay is run four weeks after surgery. It returns **negative**. Should they skip chemotherapy?

**First attempt (the dead end).** "MRD-negative means no residual cancer, so spare the patient the chemotherapy entirely." This jumps from a *measurement* (no ctDNA detected) to a *decision* (no treatment) without asking the three-validity questions. It assumes the test has clinical utility for this exact decision — that acting on MRD-negativity improves or preserves outcomes — and it ignores the test's detection floor.

**Reasoning with the structure.** Walk the three levels:

- *Analytic validity:* Can the assay reliably detect ctDNA at the relevant low fractions? MRD assays push detection to very low tumor-DNA fractions, but every assay has a limit of detection below which residual disease is invisible. A negative is "below threshold," not "zero."
- *Clinical validity:* Does MRD status correlate with recurrence? Yes — MRD-positive patients recur at much higher rates than MRD-negative patients; this is well supported in colorectal cancer.
- *Clinical utility:* Does *using* MRD to decide adjuvant therapy improve outcomes? The DYNAMIC trial provides the strongest evidence: an MRD-guided strategy reduced the proportion of patients receiving adjuvant chemotherapy without compromising recurrence-free survival [DYNAMIC trial]. That is a utility finding, not just a correlation.

So the negative result *can* support de-escalation — but only because a randomized trial demonstrated utility for this specific decision in this specific cancer, and only within the assay's detection limits.

**Resolution.** The team treats the MRD-negative result as evidence supporting (not proving) the safety of withholding adjuvant chemotherapy, consistent with the trial's strategy, while making clear to the patient that "negative" means "below detection," not "guaranteed cured," and that surveillance continues. The decision rests on demonstrated utility, not on the measurement alone.

**The lesson.** A molecular result earns the right to change a decision only when it clears all three bars — analytic validity, clinical validity, and clinical utility — for the *specific* decision at hand. The same MRD test that has utility for adjuvant de-escalation in colon cancer does not automatically have it for a different cancer or a different decision.

**The limit.** Utility evidence is decision-specific and cancer-specific, and it lags the technology badly. ctDNA assays can be ordered for dozens of situations where only the first two validities are established. Knowing a result is *real* and *correlated* is not permission to act on it; that permission comes from outcome trials, which exist for only a handful of uses.

## Common Misconceptions

**"If the assay accurately detects the mutation, the result is actionable."** This conflates analytic validity with clinical utility. The Opening Case's *DNMT3A* finding was accurately detected (analytic validity) but was not a valid tumor marker (likely clonal hematopoiesis) and certainly not actionable for the lung cancer. Accurate measurement is the floor, not the goal.

**"A liquid biopsy that finds no driver means there is no driver."** Low-shedding tumors release little ctDNA, so a clean panel can be a false negative produced by tumor biology rather than true absence of a mutation. A negative liquid biopsy in a low-shedding setting should prompt tissue testing, not reassurance — exactly the ambiguity that opened the chapter.

**"Higher stage always means the test changed the right decision."** Staging summarizes extent; it does not by itself dictate treatment, and pathological staging can differ from clinical staging once surgery reveals more disease. Treating a stage number as a treatment command skips the biology now embedded in modern staging (receptor status, grade, molecular score).

**"Multi-cancer early detection from blood is just another molecular test, so it must be ready."** MCED tests have analytic validity and growing clinical validity, but their clinical utility — whether using them reduces cancer mortality — is still under prospective trial [contested — see pantry flag]. The same three-validity discipline that justified MRD de-escalation has not yet been satisfied for population MCED.

## Exercises

1. **(Understand.)** Define analytic validity, clinical validity, and clinical utility in one sentence each, and give one example of a test that has the first two but not yet the third.

2. **(Apply.)** A ctDNA panel on a patient with metastatic breast cancer reports an *ESR1* mutation. Explain what this finding could mean for hormone-therapy resistance, then list two reasons (one biological, one technical) why you would or would not change therapy on the basis of this single result.

3. **(Apply+.)** A new comprehensive genomic profiling test reports that 45% of advanced cancers carry an "actionable" alteration. A colleague concludes that "nearly half of patients will benefit." Identify the gap between *actionable alteration present* and *patient benefits*, and name the specific kind of evidence (and study design) that would close it. Tie your answer to the three-validity framework.

4. **(Produce — a decision table.)** For three biomarker–drug pairs of your choice (e.g., HER2/trastuzumab, MSI-high/checkpoint inhibitor, BRCA/PARP inhibitor), build a table with columns: biomarker, test method, what analytic validity requires, what clinical validity requires, and what evidence establishes clinical utility. Mark which pairs are tumor-agnostic.

5. **(Evaluate.)** The AJCC 8th edition added molecular factors to breast and prostate staging. Argue either that this improves staging (more accurate prognosis) or that it blurs the line between "extent of disease" and "biology of disease." Support your position with one concrete consequence for how a patient would be counseled.

## What Would Change My Mind

The central claim is that a molecular measurement should change a clinical decision only when clinical *utility* — not merely accuracy or correlation — has been demonstrated for that specific decision. What would revise the strong form of this claim? Convincing evidence that a class of molecular tests reliably improves outcomes *across* decisions and cancers from analytic and clinical validity alone — for instance, if large prospective trials showed that comprehensive genomic profiling at diagnosis, applied broadly, improved survival even where no decision-specific utility trial had been run [NCI, *Research Areas: Cancer Diagnosis*]. That would suggest utility can sometimes be inferred from validity plus a credible mechanism, loosening the demand for per-decision outcome trials. Conversely, continued findings that utility is narrow and decision-specific — that the same test helps in one setting and not another — would harden the claim that measurement and utility must be evaluated separately, every time.

## Still Puzzling

- Can ctDNA-based multi-cancer early detection ever clear the utility bar, given that the curable early cancers shed the least DNA? Or is there a biological floor that confines liquid biopsy to monitoring known disease rather than finding new disease? [contested]
- As staging absorbs more molecular factors, where does "stage" end and "molecular subtype" begin? If two tumors share TNM but differ in a dozen genomic features, is a single stage number still the right summary?
- Clonal hematopoiesis confounds liquid biopsy and increases with age. As the screened and tested population ages, will the background of non-tumor mutations grow fast enough to undermine the specificity of blood-based cancer tests?

## References

- National Cancer Institute. *Research Areas: Cancer Diagnosis* (biomarkers, genomic analysis, liquid biopsy, AI). https://www.cancer.gov/research/areas/diagnosis
- National Cancer Institute. *Tests and Procedures Used to Diagnose Cancer.* https://www.cancer.gov/about-cancer/diagnosis-staging/diagnosis
- NIH Research Matters. *Detecting cancer* (liquid biopsy). https://www.nih.gov/news-events/nih-research-matters/detecting-cancer
- American Joint Committee on Cancer. *AJCC Cancer Staging Manual,* 8th edition, 2017.
- Tie J, et al. Circulating tumor DNA analysis guiding adjuvant therapy in stage II colon cancer (DYNAMIC trial). *N Engl J Med* 2022.
- US Food and Drug Administration. *Oncology Center of Excellence.* https://www.fda.gov/about-fda/fda-organization/oncology-center-excellence

## Prompts

*No figures have been generated for this chapter yet.*
*Run the Cowork enrichment pass to populate this section.*
