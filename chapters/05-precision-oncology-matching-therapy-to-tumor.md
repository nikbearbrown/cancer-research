# Precision Oncology: Matching Therapy to Tumor

## Learning Objectives

After working through this chapter, you should be able to:

- **Explain** how a molecular biomarker functions as a *prediction* about drug response, and distinguish a biomarker that is *prognostic* (forecasts outcome regardless of treatment) from one that is *predictive* (forecasts response to a specific drug).
- **Compare** basket, umbrella, and platform trial designs, and **identify** which design produces which kind of evidence claim (tumor-agnostic approval vs. type-specific matching).
- **Evaluate** a "matched but didn't respond" case and **diagnose** the most likely reasons — wrong biomarker, wrong threshold, resistance, or co-occurring alterations.
- **Critique** a tumor-agnostic approval by asking what response rate, across which cancers, with what denominator, justified the claim.
- **Produce** a molecular-profiling-to-treatment reasoning chain for a hypothetical patient, naming the test, the actionable alteration, the matched drug, and the expected durability.

## Opening Case

A 58-year-old never-smoker is diagnosed with metastatic lung adenocarcinoma. Comprehensive genomic profiling of her tumor — next-generation sequencing of several hundred cancer genes — returns a *KRAS G12C* mutation. KRAS G12C is, on paper, an actionable alteration: sotorasib and adagrasib, approved in 2021 and 2022, target precisely this mutation. The molecular tumor board calls it a match. She starts sotorasib.

Her tumor shrinks for four months. Then it grows again. A repeat biopsy shows the KRAS G12C mutation is still there — but now the tumor also carries new alterations in the downstream signaling pathway, and a subpopulation of cells has switched to a different growth driver entirely. The drug still binds its target. The target still drives the cancer. And yet the cancer is winning.

Down the hall, a different patient with the *same* KRAS G12C mutation never responded at all. Same biomarker, same drug, no shrinkage from day one.

The match was real. The response was not durable in one patient and absent in the other. This chapter is about why a molecular match is a *hypothesis about response*, not a guarantee — and how oncology builds and tests that hypothesis.

## Core Concepts

### What "precision" actually means

For most of cancer therapy's history, drugs were assigned by tumor type: this chemotherapy for everyone with this cancer, regardless of the cancer's underlying biology. Some patients responded, others didn't, and the difference was filed under "biological variability" — a polite name for ignorance.

**Precision oncology** is the reframing of that variability as *molecular* rather than random. The plain-language version: the cancer's genetic and protein features, more than its tissue of origin, tell you which drug will work. The formal definition: precision oncology matches a therapy to a specific, measurable molecular feature of a tumor — a feature shown, in trials, to predict response to that therapy.

Note what *precision* does **not** mean. It does not mean the treatment is unique to one person. Two patients with the same alteration usually get the same drug. The "precision" is in the molecular targeting, not in individual customization (that is **personalized medicine**, a related but stronger claim that accounts for the whole person — comorbidities, preferences, genetic background — and remains largely aspirational in routine practice) [NCI Targeted Therapy].

### Actionable alteration

An **actionable alteration** is a molecular feature for which a matched therapy exists and has demonstrated benefit. These come in several types: point mutations (*EGFR*, *BRAF* V600E, *KRAS* G12C), gene fusions (*ALK*, *ROS1*, *RET*, *NTRK*), copy-number changes (*HER2* amplification), expression patterns (estrogen receptor, PD-L1), and functional signatures (microsatellite instability, tumor mutational burden) [cba-32].

The word *actionable* is doing quiet, load-bearing work. It does not mean "present." It means "present **and** linked, by evidence, to a drug that helps." A mutation you can detect but cannot exploit is not actionable, however dramatic it looks on the report.

### Predictive vs. prognostic — the distinction that drives everything

This is the single most important distinction in the chapter, and it is the one students most often collapse.

- A **prognostic biomarker** forecasts the patient's outcome *regardless of treatment*. It tells you how aggressive the cancer is.
- A **predictive biomarker** forecasts response *to a specific therapy*. It tells you whether *this drug* will work.

Precision oncology runs on predictive biomarkers. *EGFR* exon-19 deletion predicts response to osimertinib; *BRCA1/2* mutation predicts response to PARP inhibitors through synthetic lethality (the drug is lethal only in cells already missing a DNA-repair pathway) [cba-32]. A feature can be both, but conflating them produces exactly the failure mode of treating a marker of *bad biology* as if it were a *drug target*.

<!-- → [DIAGRAM: predictive vs. prognostic biomarker — two-by-two showing biomarker status × treatment, with response curves diverging only for predictive markers] -->

### Tumor-agnostic therapy

The most evolved form of precision oncology is **tumor-agnostic therapy**: a drug approved across cancer types based on a molecular feature, *regardless of tissue of origin*. The first was pembrolizumab for **microsatellite-instability-high (MSI-H)** tumors in 2017 — approved on response rates of roughly 30–50% in MSI-H cancers spanning colorectal, endometrial, gastric, and biliary sites [cba-32]. Then larotrectinib and entrectinib for *NTRK* fusion-positive tumors (2018–2019); pembrolizumab for tumor-mutational-burden-high (≥10 mutations/megabase) tumors (2020); dabrafenib + trametinib for *BRAF* V600E solid tumors (2022) [cba-32]. The claim embedded in each approval: *the biology is what matters; the tissue is incidental.*

That claim is powerful and contestable. The denominator behind a tumor-agnostic approval is a patchwork of small cohorts across many cancers — the response rate that looks like one number may hide tissue-specific variation [verify].

### Trial designs encode evidence claims

Precision oncology needed new trial machinery, because the molecular subgroups are small and scattered across cancer types. The design you choose determines the *kind* of claim you can make. **Basket trials** enroll patients by *molecular alteration* across many tumor types — the design that produces tumor-agnostic claims; larotrectinib and entrectinib reached approval this way [cba-32]. **Umbrella trials** enroll one *cancer type* and assign patients to arms by molecular feature — Lung-MAP in non-small-cell lung cancer is the classic example [cba-32]. **Platform trials** maintain permanent infrastructure and add or drop arms over time (I-SPY 2 in breast cancer) [cba-32]. Reading a precision-oncology result therefore requires knowing which design produced it: a basket result speaks to a biomarker across tissues, an umbrella result to matching within one tissue.

<!-- → [DIAGRAM: basket vs. umbrella vs. platform trial designs — basket enrolls one alteration across many tumor types; umbrella enrolls one tumor type split by alteration; platform adds/drops arms over time] -->

## Worked Example

**Situation.** Return to the opening patient with KRAS G12C lung adenocarcinoma. We want to reason about *why a real match failed*, and what that teaches about reading molecular reports.

**The reasoning — including a dead end.**

First instinct (the dead end): "The biomarker must have been wrong — maybe the sequencing called a mutation that wasn't really there, or the test was low quality." This is worth checking, and it is the right reflex in general: a precision decision is only as good as the assay's analytic validity. But the repeat biopsy confirms KRAS G12C is present, and it was present at baseline. The test was right. The match was real. So a bad-assay explanation fails here, and clinging to it would send us hunting for a measurement error that doesn't exist.

Second pass (the productive path): distinguish the *target* from the *tumor's dependence on that target over time*. At baseline the cancer was driven by KRAS G12C signaling, sotorasib blocked it, and the tumor shrank — the hypothesis "this tumor depends on KRAS G12C" was, for four months, confirmed by the response itself. Resistance then emerged not because the drug stopped binding, but because the tumor *evolved*: new downstream mutations restored the signal, and a subclone adopted an entirely different driver [cba-32]. Treatment is selection pressure. It does not act on a static tumor; it acts on an evolving population, and it selects for the cells that can route around the blockade.

Now the **second patient**, who never responded at all. Same mutation, zero shrinkage. The likely explanations differ: a **co-occurring alteration** (for instance a loss in a tumor-suppressor pathway) may have made the cancer independent of KRAS signaling from the start, so blocking KRAS changed nothing. The biomarker was present but not, in that tumor, *the* dependency.

**Resolution.** Two patients, one biomarker, three outcomes (transient response, no response, and — in some KRAS G12C patients — durable benefit). The match identified a *candidate dependency*. Whether the tumor actually depended on it, and kept depending on it, was an empirical question the drug itself answered. KRAS G12C inhibitors are, by the field's own assessment, "meaningful but not dramatic," with response rates well below the EGFR or ALK inhibitors and resistance that develops reliably [cba-32].

**The lesson.** A molecular match is a *prediction*, scored by the response, not a property you can read off the report. "Matched" and "responded" are different measurements, and the gap between them is where precision oncology earns or loses its claims.

**The limit.** This reasoning explains *that* responses vary and *some* mechanisms of resistance. It does not let us predict, before treatment, which KRAS G12C patient will get four months, which will get none, and which will get durable control. Pre-treatment prediction of durability remains, across most targeted therapies, unsolved [contested — see pantry flag].

## Common Misconceptions

**"If the tumor carries the target, the matched drug will work."** Plausible — it is the whole promise of precision oncology. It fails because target *presence* is not the same as target *dependence*, and dependence can be absent from the start (co-occurring alterations) or lost over time (resistance evolution). The opening case is the counterexample: target present, target still driving, drug still binding, tumor still winning.

**"Tumor shrinkage means the treatment worked."** Plausible, because shrinkage is visible and feels like benefit. It fails because the endpoint that matters — does the patient live longer or better — is not the same measurement as response rate. A drug can shrink tumors (high response rate) without extending survival, and a drug with modest shrinkage can extend life. The opening patient's tumor shrank for four months; whether that translated to meaningful benefit is a separate, harder question requiring survival data [cba-32; pantry notes, "Endpoints matter"].

**"A tumor-agnostic approval means the drug works the same in every cancer."** Plausible, since the approval is, by name, agnostic to tissue. It fails because the approval rests on a *pooled* response rate across heterogeneous small cohorts; the true rate can vary by tissue, and rare tissues may be underrepresented or absent from the trial entirely [verify]. Agnostic in the *label* does not mean uniform in the *biology*.

**"Precision oncology has solved cancer treatment."** It transformed cancers driven by a single dominant oncogene — chronic myeloid leukemia (BCR-ABL, imatinib), EGFR-mutant lung cancer, HER2-positive breast cancer, melanoma [cba-32]. It has barely touched pancreatic cancer and glioblastoma, where most patients have no actionable alteration and the few targeted options help small subsets [cba-32]. The failure pattern is informative: single-driver cancers yield; multi-driver, microenvironment-dominated cancers resist.

## Exercises

1. **(Comprehension.)** In one sentence each, define *predictive biomarker*, *prognostic biomarker*, and *actionable alteration*. Then state which of the three is the load-bearing concept for tumor-agnostic approvals, and why.

2. **(Apply.)** A patient with metastatic colorectal cancer has a *BRAF* V600E mutation. In melanoma, BRAF V600E predicts strong response to BRAF + MEK inhibitors; in colorectal cancer, single-agent BRAF inhibition works poorly and the combination requires adding an anti-EGFR antibody [cba-32]. Explain, in terms of *target dependence* and *co-occurring signaling*, why the same mutation behaves differently across tissues — and what this does to the "tissue is incidental" claim of tumor-agnostic therapy.

3. **(Apply / Analyze.)** You are designing a trial to test a new drug against an *NTRK* fusion present in fewer than 1% of tumors across all cancer types. Choose between a basket and an umbrella design, justify the choice, and state the *specific evidence claim* your chosen design can and cannot support. (Recall: larotrectinib and entrectinib reached tumor-agnostic approval through basket designs [cba-32].)

4. **(Produce.)** Write a one-page molecular-profiling-to-treatment reasoning chain for a hypothetical never-smoker with metastatic lung adenocarcinoma. Name (a) the test you would order, (b) at least three alterations you would hope to find and the matched drug for each, (c) the expected response durability where known, and (d) one point in the chain where a "matched but didn't respond" outcome could arise. Cite the alteration-drug pairings to the chapter or to a named source; mark anything you are unsure of `[verify]`.

5. **(Evaluate / Produce.)** Find the FDA label or pivotal-trial publication for one tumor-agnostic approval (e.g., larotrectinib, or pembrolizumab for MSI-H). Report the overall response rate, the number of distinct cancer types in the cohort, and the smallest per-tissue subgroup. Write two sentences on whether the "agnostic" claim is well supported by that denominator.

## What Would Change My Mind

The central claim of this chapter is that a molecular match is a *hypothesis about response*, validated only by the response itself — that "matched" and "responded" are distinct measurements separated by an irreducible gap. What would revise this claim is a *pre-treatment* assay — likely multi-omic, integrating the alteration with co-occurring mutations, expression state, and microenvironment — that predicts response *and durability* for a targeted drug with accuracy high enough to act on (say, a positive predictive value above 80% for durable response, prospectively validated). If such an assay existed and held up across cancer types, the gap between "matched" and "responded" would largely close, and the match would become close to a guarantee rather than a hypothesis. Patient-derived organoid testing and AI-integrated multi-omic models are the current candidates [cba-32]; none has yet met that bar.

## Still Puzzling

- Why do some patients with a textbook actionable alteration never respond at all, when the target is present and the drug demonstrably binds it? Co-occurring alterations explain some cases, but not all [contested — see pantry flag].
- What is the right *denominator* for a tumor-agnostic approval? Pooling across tissues maximizes statistical power but assumes a uniformity the biology may not honor. How small can a per-tissue cohort be before "agnostic" becomes a statistical artifact?
- Can resistance be *predicted and pre-empted* — combinations chosen at baseline to block the escape routes — or is treatment-driven evolution fast enough that we will always be one step behind?
- Why have cancers like pancreatic adenocarcinoma resisted precision approaches despite exhaustive molecular characterization? Is the limit the absence of druggable drivers, or our inability to drug the drivers (KRAS, MYC, p53) that are present?

## References

- National Cancer Institute. *Targeted Therapy to Treat Cancer.* https://www.cancer.gov/about-cancer/treatment/types/targeted-therapies
- National Cancer Institute. *Immunotherapy to Treat Cancer.* https://www.cancer.gov/about-cancer/treatment/types/immunotherapy
- National Cancer Institute. *Tests and Procedures Used to Diagnose Cancer.* https://www.cancer.gov/about-cancer/diagnosis-staging/diagnosis
- U.S. Food and Drug Administration, Oncology Center of Excellence. *Project Optimus* (dose optimization in oncology drug development). https://www.fda.gov/about-fda/oncology-center-excellence/project-optimus
- Source chapter (cba-32), *Precision Oncology: Matching Therapy to Tumor*, for biomarker-drug pairings, tumor-agnostic approval history, trial frameworks, and the success/failure pattern across cancer types.
- Druker BJ. Development of imatinib (Gleevec) against BCR-ABL in chronic myeloid leukemia — the founding case of targeted therapy. (See chapter source for context.)
- Trials referenced for trial-design frameworks: Lung-MAP (umbrella, NSCLC); I-SPY 2 (platform, breast); basket designs underlying larotrectinib/entrectinib approvals [verify specific citations against pivotal publications].

## Prompts

<!-- This section is populated automatically by the Cowork enrichment
     pass. Each D3 figure generated in this chapter gets an entry here:
     the figure number, a short title, and a ready-to-paste prompt
     that produces a close approximation of that figure.

     Prerequisites: paste CLAUDE.md and DESIGN.md from the brutalist/
     folder before each prompt, or load them into your Claude project
     context once and reference them by name.
-->

*No figures have been generated for this chapter yet.*
