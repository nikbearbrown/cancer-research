# Cancer Diagnosis: Imaging and the Tissue Sample

## Learning Objectives

After working through this chapter, you should be able to:

- **Explain** why imaging produces a probability of cancer rather than a diagnosis, and identify the sources of false positives and false negatives for CT, MRI, ultrasound, and PET.
- **Justify** why tissue examined by a pathologist is the diagnostic ground truth, and describe what histology and immunohistochemistry add that imaging cannot.
- **Analyze** sampling error in biopsy — how a needle can miss the cancer, hit an unrepresentative region, or obtain too little tissue for molecular testing — and explain why a negative biopsy does not exclude cancer.
- **Compare** fine-needle aspiration and core needle biopsy by what each can and cannot establish.
- **Integrate** the diagnostic chain (suspicion → imaging → biopsy → pathology) and locate where each link can break.

## Opening Case

A 64-year-old woman has a 2-centimeter mass in the tail of the pancreas found incidentally on a CT scan ordered for back pain. The radiologist's report reads "mass suspicious for adenocarcinoma." Her family hears the word *adenocarcinoma* and assumes the diagnosis is made. It is not. An endoscopic ultrasound-guided fine-needle aspiration is performed; the cytology returns "atypical cells, cannot exclude malignancy — nondiagnostic." A second aspiration returns "benign pancreatic acinar tissue."

Now there are three pieces of evidence pointing in different directions: an image that looks like cancer, a first sample that is ambiguous, and a second sample that is reassuring. Her oncologist has to decide whether the reassuring biopsy means there is no cancer — or whether the needle simply missed it. Pancreatic tumors are surrounded by dense reactive tissue; a needle can pass through the mass and pull back stroma rather than tumor. A negative result here is genuinely ambiguous: it could mean *no cancer* or *missed the cancer*.

The image was never the diagnosis. The image was a probability. The tissue is supposed to be the ground truth — but only if the tissue is *the right tissue*. This chapter is about that chain: how imaging assigns a probability, why tissue is the arbiter, and how the tissue itself can lie when the sample is wrong.

## Core Concepts

### Imaging is probabilistic, not definitive

When a doctor says "the scan shows cancer," what the scan actually shows is an abnormality whose appearance is *consistent with* cancer to some degree. Every imaging modality reports a signal — density, water content, sound reflection, metabolic uptake — that correlates with malignancy imperfectly. The radiologist converts that signal into a probability, often expressed in calibrated language ("suspicious," "indeterminate," "likely benign").

**Computed tomography (CT)** reconstructs cross-sectional anatomy from X-rays acquired around the patient [NCI, *Cancer Imaging Basics*]. It is the workhorse for detecting masses and metastases and for guiding biopsy, but soft-tissue contrast is limited and it carries radiation (a body CT delivers roughly 8–15 mSv versus ~0.1 mSv for a chest X-ray) [source chapter; NCI, *CT Scans and Cancer Fact Sheet*]. CT is also the substrate for **RECIST (Response Evaluation Criteria In Solid Tumors)**, the standardized rules for measuring tumor size across scans.

**Magnetic resonance imaging (MRI)** uses magnetic fields and radiofrequency pulses; different sequences emphasize different tissue properties. It gives superior soft-tissue contrast for brain, spinal cord, soft-tissue tumors, pelvic cancers, and breast — breast MRI is the most sensitive modality for breast cancer detection [source chapter].

**Ultrasound** uses high-frequency sound, is real-time and radiation-free, and is excellent for superficial structures and image-guided biopsy. Its quality is **operator-dependent**, and it cannot penetrate gas or bone well.

**Positron emission tomography (PET)** with **fluorodeoxyglucose (FDG)** — a radiolabeled glucose analog trapped in metabolically active cells — images function rather than anatomy [NCI, *Cancer Imaging Basics*]. Cancer cells, with elevated glucose uptake, light up. But so does inflammation, infection, brown fat, and recent surgery (false positives), while some indolent or mucinous tumors barely take up FDG at all (false negatives). PET is read alongside CT or MRI (PET-CT) to combine function with anatomy.

The unifying point: each modality has a characteristic false-positive and false-negative profile. None of them diagnoses cancer. They raise or lower the probability that tissue, when obtained, will show cancer.

<!-- → [DIAGRAM: diagnostic workup flow — clinical suspicion → imaging (probability) → biopsy (sampling) → pathology (ground truth) → molecular workup, with failure modes annotated at each arrow] -->

### Tissue is the ground truth

A radiographic abnormality, however suggestive, is not a cancer diagnosis. **Cancer diagnosis requires tissue or cells examined by a pathologist** [NCI, *Tests and Procedures Used to Diagnose Cancer*]. Why is tissue privileged over the image? Because malignancy is defined by what cells look like and how they are organized — features visible only under a microscope.

The pathologist fixes the tissue (formalin, then paraffin embedding — **FFPE**, the standard preparation), cuts thin sections, and stains them. The routine stain is **hematoxylin and eosin (H&E)**: hematoxylin turns nuclei blue, eosin turns cytoplasm pink, and the contrast reveals cell morphology and tissue architecture. The diagnosis rests on cell shape, nuclear features (enlargement, irregularity, prominent nucleoli), how cells are arranged (glands, sheets, nests), and context (invasion, necrosis). The pathology report names the tumor type, its **grade** (how closely it resembles normal tissue), its margins, and whether tumor has invaded vessels or nerves. This report is the foundation document for treatment.

### Immunohistochemistry: when H&E is not enough

Often morphology alone cannot distinguish two cancers, or identify where a metastasis came from. **Immunohistochemistry (IHC)** applies antibodies against specific proteins, then stains where the protein is present, letting the pathologist read a tumor's lineage and therapeutic targets [source chapter]. IHC identifies lineage (cytokeratins for carcinomas, CD20 for B-cell lymphomas), determines hormone-receptor status (ER/PR in breast cancer), and flags therapeutic targets (HER2, PD-L1, mismatch-repair status). IHC is what turns "adenocarcinoma" into "lung adenocarcinoma, TTF-1 positive, PD-L1 high" — a diagnosis a treatment can act on.

### Sampling error: when the tissue lies

Here is the chapter's hardest idea. Tissue is ground truth *only if the tissue is representative of the lesion*. A biopsy samples a tiny fraction of a heterogeneous mass through a needle the width of a pencil lead. Three things can go wrong:

- The needle **misses the tumor entirely**, pulling back adjacent normal or reactive tissue (the Opening Case).
- The needle hits the mass but samples an **unrepresentative region** — necrotic core, or a low-grade area of a tumor whose lethal high-grade region lies elsewhere.
- The needle obtains tissue but **too little** for the full molecular workup that modern treatment requires.

The consequence is asymmetric and crucial: **a positive biopsy is highly reliable, but a negative biopsy does not exclude cancer.** A positive result means malignant cells were seen — they are there. A negative result means *this sample* showed no malignancy, which is consistent with no cancer or with a missed cancer. The strength of a negative depends on how confident you are that the needle was in the right place.

### The two main needles

**Fine-needle aspiration (FNA)** uses a thin needle to aspirate loose cells for cytology — rapid, minimal, good for thyroid nodules and lymph nodes, but it yields *cells without architecture* and often too little material for molecular testing. **Core needle biopsy** uses a larger needle to obtain a cylinder of tissue, preserving architecture and providing enough material for IHC and molecular profiling [source chapter]. The choice trades invasiveness against how much the sample can establish.

## Worked Example

**Situation.** Return to the woman with the pancreatic-tail mass. Image: suspicious for adenocarcinoma. First FNA: atypical, nondiagnostic. Second FNA: benign acinar tissue. The team must decide: stop (call it benign) or proceed (repeat sampling or resect).

**First attempt (the dead end).** "Two biopsies, and the more recent one is clearly benign. Tissue beats imaging — the mass is not cancer; reassure her." This reasoning correctly ranks tissue above imaging but mishandles the *negative* biopsy. It treats "benign tissue obtained" as equivalent to "lesion is benign." For a pancreatic mass, those are not the same statement.

**Reasoning with the numbers.** Suppose, from the imaging features and clinical context, the **pretest probability** of malignancy is high — say 80%. EUS-guided FNA of solid pancreatic masses has good sensitivity but it is not perfect; reported sensitivity sits roughly in the 80–90% range, meaning **10–20% of true cancers yield a non-malignant aspirate** [verify against current EUS-FNA literature]. Apply Bayes informally. Pretest odds of malignancy are 80:20 = 4:1. A negative result is about 15% likely if cancer is present (an imperfect-sensitivity miss) and about 95% likely if cancer is absent, giving a likelihood ratio of 0.15/0.95 ≈ 0.16. Posterior odds ≈ 4 × 0.16 ≈ 0.64, which converts to a **post-biopsy probability of malignancy still around 39%** — far too high to call benign.

The dense desmoplastic stroma around pancreatic adenocarcinoma is exactly the kind of tissue that fills a needle with reactive, non-malignant cells while the tumor sits millimeters away. The benign result is consistent with a missed sampling, not a benign lesion.

**Resolution.** The team does *not* reassure. They repeat sampling with a core technique to obtain architecture and more material, and present the case at a multidisciplinary conference; if repeat sampling remains nondiagnostic against a high pretest probability, resection for definitive pathology is considered. The image set the probability; the negative tissue could not overturn it because the negative tissue might be the wrong tissue.

**The lesson.** A negative biopsy is only as strong as your confidence that the needle sampled the lesion. Always interpret a biopsy result against the pretest probability the imaging and clinic established — a negative result lowers that probability but, when sensitivity is imperfect and pretest probability is high, may not lower it enough to act on.

**The limit.** This reasoning cuts both ways and has a cost. Refusing to accept negative biopsies drives repeat procedures, each with its own complication risk (bleeding, pancreatitis, pneumothorax depending on site). The skill is not "never trust a negative" but calibrating how much a given negative should move you — which requires knowing the test's sensitivity and the pretest probability, neither of which is printed on the pathology report.

## Common Misconceptions

**"The scan showed cancer, so the diagnosis is made."** Imaging reports a probability, not a diagnosis. The Opening Case began with a scan "suspicious for adenocarcinoma" — language that explicitly encodes uncertainty. Without tissue, "cancer" is a clinical hypothesis. Treating the image as the diagnosis skips the only step that can confirm malignancy.

**"A negative biopsy rules out cancer."** A negative biopsy means *this sample* showed no malignancy. Because needles can miss, a negative result against a high pretest probability may leave the probability of cancer substantial — as the Worked Example computed (~39% remaining). The positive biopsy is reliable; the negative biopsy is conditional on having sampled the right place.

**"PET lights up cancer, so a hot spot is cancer."** FDG-PET images glucose uptake, which is elevated in cancer but also in inflammation, infection, and healing surgical sites. A PET-positive focus raises probability; it does not establish malignancy. Conversely, indolent and mucinous tumors can be PET-negative, so a cold scan does not exclude cancer.

**"More tissue is always better, so always do the biggest biopsy."** The right biopsy is the one that obtains *representative, sufficient* tissue at acceptable risk — not the largest. FNA is appropriate when cytology answers the question; core biopsy is needed when architecture and molecular material are required. Choosing wrong wastes a procedure or under-samples for the molecular workup the next chapter depends on.

## Exercises

1. **(Understand.)** Explain in two or three sentences why a pathologist's reading of tissue is treated as the diagnostic ground truth while a radiologist's reading of an image is not, even when both experts are equally skilled.

2. **(Apply.)** A lung nodule is FDG-avid on PET (SUV high). List three benign processes that could produce this and three tumor types that could be FDG-negative despite being malignant. State, in one sentence each, how the PET result should change your estimated probability of cancer up or down.

3. **(Apply+ — produce a calculation.)** A breast core biopsy has sensitivity 95% for a sampled lesion. A radiologist estimates the pretest probability of malignancy for a particular mass at 60% (BI-RADS 4C). The biopsy returns benign. Using a likelihood-ratio or 2×2 approach, estimate the post-biopsy probability of malignancy. Then state whether you would accept the benign result or recommend re-biopsy, and justify the threshold you used.

4. **(Produce — a decision flow.)** Draw the diagnostic chain for a suspected liver lesion: clinical suspicion → imaging choice → biopsy choice → pathology → IHC. At each arrow, write the dominant failure mode (e.g., "ultrasound operator-dependent," "needle misses lesion," "insufficient tissue for IHC") and what you would do to mitigate it.

5. **(Evaluate.)** Compare FNA and core needle biopsy for a 2-cm thyroid nodule versus a 4-cm retroperitoneal soft-tissue mass. Which would you choose for each, and what specifically does the choice depend on — diagnosis alone, or the need for molecular material downstream?

## What Would Change My Mind

The central claim is that imaging is probabilistic and that tissue, when correctly sampled, is the arbiter — so a negative biopsy must be weighed against pretest probability rather than accepted at face value. What would revise this? Rigorous prospective evidence that a non-invasive modality — for example, advanced quantitative MRI (diffusion and perfusion imaging) or a molecular-imaging tracer — could distinguish malignant from benign tissue with a positive and negative predictive value high enough to *replace* biopsy for a defined lesion type, validated against pathology as the reference standard [*Advances in Diffusion and Perfusion MRI for Quantitative Cancer Imaging*, 2020; NCI, *Cancer Imaging Basics*]. If imaging could deliver tissue-equivalent certainty for some cancers, the privileged status of the needle would erode for those cancers. So far, imaging informs the probability and tissue settles it — but this is an empirical claim about current technology, not a law of nature.

## Still Puzzling

- How heterogeneous is a tumor allowed to be before a single core biopsy is fundamentally inadequate? For some cancers, the region a needle hits may not carry the mutations that drive lethality. Where is the line, and how would we know we had crossed it? [contested]
- AI tools now read mammograms, lung CTs, and digital pathology slides. When an algorithm and a human radiologist disagree, whose probability should drive the biopsy decision — and how do we validate the algorithm against a ground truth that is itself a sampled, imperfect biopsy?
- For lesions that cannot be safely biopsied (some brain, some pancreatic, some lung), we are forced to treat on imaging probability alone. How should the threshold for treating-without-tissue be set, and who decides?

## References

- National Cancer Institute. *Cancer Imaging Basics.* https://dctd.cancer.gov/research/research-areas/imaging/basics
- National Cancer Institute. *Tests and Procedures Used to Diagnose Cancer.* https://www.cancer.gov/about-cancer/diagnosis-staging/diagnosis
- National Cancer Institute. *CT Scans and Cancer Fact Sheet.* https://www.cancer.gov/about-cancer/diagnosis-staging/ct-scans-fact-sheet
- *Advances in Diffusion and Perfusion MRI for Quantitative Cancer Imaging.* 2020. https://pmc.ncbi.nlm.nih.gov/articles/PMC7747414/
- Eisenhauer EA, et al. RECIST 1.1: New response evaluation criteria in solid tumors. *Eur J Cancer* 2009.
- National Cancer Institute. *Research Areas: Cancer Diagnosis* (imaging, biomarkers, AI, biopsy). https://www.cancer.gov/research/areas/diagnosis

## Prompts

*No figures have been generated for this chapter yet.*
*Run the Cowork enrichment pass to populate this section.*
