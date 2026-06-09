# Cancer Screening: Finding It Early Enough to Cure

## Learning Objectives

After working through this chapter, you should be able to:

- **Distinguish** screening from diagnosis, and explain why a screening test is evaluated at the population level rather than the individual level.
- **Calculate** the positive predictive value (PPV) of a screening test from its sensitivity, specificity, and the prevalence of disease in the screened population, and explain why prevalence governs PPV.
- **Diagnose** lead-time bias, length-time bias, and overdiagnosis in a described screening scenario, and explain why each can make a screening program look more effective than it is.
- **Apply** the Wilson and Jungner criteria to evaluate whether a proposed screening program is justified.
- **Judge** when reported survival statistics are evidence of benefit and when they are statistical artifacts, using disease-specific mortality as the corrective.

## Opening Case

A 58-year-old man with no symptoms reads that a new blood test can "detect 50 cancers from a single tube of blood." He pays out of pocket and the test comes back positive, with a predicted tissue of origin of "pancreas/biliary." He is terrified. Over the next six weeks he undergoes a contrast CT, an MRI, an endoscopic ultrasound with fine-needle aspiration, and a PET scan. The pancreas is normal. The aspiration nicks a small vessel and he is admitted overnight for observation. Three months and several thousand dollars later, the working conclusion is that the test was a false positive — or possibly that something is there that nobody can find.

His physician is now in an uncomfortable position. The test reported "cancer signal detected," but every test that can actually *see* tissue says otherwise. Was the blood test wrong? Is there an occult tumor too small to image? Should they keep looking, or stop? The patient asks the obvious question: "If the test is so good, why can't anyone confirm it?"

The trouble is that the man was never told the number that mattered. The test's specificity sounds excellent. But a positive result in a healthy, low-risk person carries far less weight than the marketing implied — and nobody computed *how much* less before he was sent down a cascade of invasive follow-up. This chapter is about that number, and about the several ways early detection can fool us into thinking we are saving lives when we are mostly producing alarm.

## Core Concepts

### Screening is a population test, not a diagnosis

A **screening test** is applied to people *without symptoms*, drawn from a defined risk group, to find disease earlier than it would otherwise appear. This is categorically different from a **diagnostic test**, which is applied to someone in whom disease is already suspected. The distinction is not pedantic. Because most screened people do not have the disease, the test must be judged by what happens across the whole population — deaths prevented, false alarms generated, healthy people harmed by follow-up — not by whether it "found a cancer" in one person.

The mathematics of this is unforgiving, and it is the central skill of the chapter. Four outcomes are possible when a test meets a person:

- **True positive (TP):** test positive, disease present.
- **False positive (FP):** test positive, disease absent. The person is told they may have cancer and worked up unnecessarily.
- **True negative (TN):** test negative, disease absent.
- **False negative (FN):** test negative, disease present. The person is falsely reassured.

Two properties describe the test itself:

- **Sensitivity** = TP / (TP + FN): of people *with* the disease, the fraction the test correctly flags. A sensitive test misses few cancers.
- **Specificity** = TN / (TN + FP): of people *without* the disease, the fraction the test correctly clears. A specific test generates few false alarms.

Sensitivity and specificity are properties of the test. But the number a worried patient actually wants is the **positive predictive value (PPV)** = TP / (TP + FP): given a positive result, the probability that disease is truly present. And PPV is *not* a property of the test alone — it depends on **prevalence**, the fraction of the screened population that actually has the disease.

<!-- → [CHART: 2x2 confusion matrix — TP/FP/FN/TN cells with sensitivity, specificity, and PPV labeled on the margins] -->

### Why prevalence governs PPV

This is where intuition fails most students, so we will compute it explicitly in the Worked Example. The key fact: when prevalence is low — as it is for almost any single cancer in an asymptomatic population — even a very specific test produces *mostly false positives among its positives*. The false positives are drawn from the enormous pool of healthy people; the true positives are drawn from the tiny pool of sick people. Bayes' theorem applied to a population makes the result inevitable [NCI, *Cancer Screening Tests*]. The opening case is exactly this: a low-prevalence individual, a positive result, and a PPV nobody bothered to estimate.

### The biases that flatter screening

Three artifacts can make screening look effective even when it changes nothing about when people die.

**Lead-time bias.** Screening, by definition, moves the diagnosis date earlier. If a cancer is found at age 50 by screening but the patient still dies at 60, "survival from diagnosis" is 10 years. If the same cancer were found by symptoms at 55 with death at 60, survival is 5 years. The screening patient *appears* to survive twice as long — but died at the identical age. Earlier diagnosis inflates measured survival even when treatment helps not at all [verify — standard epidemiology; described in source chapter].

**Length-time bias.** Screening catches cancers during their detectable preclinical phase. Slow-growing tumors spend longer in that phase, so they are over-represented among screen-detected cancers; fast, lethal tumors tend to surface as symptoms *between* screening rounds. Screen-detected cancers are therefore, on average, biologically more indolent — they would have done better regardless.

**Overdiagnosis.** The most consequential. Screening can detect cancers that would never have caused symptoms in the person's lifetime — slow tumors in older patients, indolent histologies, in-situ lesions. The patient is diagnosed, treated, and harmed, but would have lived just as long untreated. Overdiagnosis is especially severe in prostate (PSA-detected indolent disease), thyroid (papillary microcarcinomas), and some screen-detected breast disease (DCIS) [source chapter; NCI, *Cancer Screening Tests*].

The corrective for all three is to evaluate screening by **disease-specific mortality** in randomized trials with long follow-up — does the screened group die of this cancer less often than the unscreened group? — not by survival time from diagnosis, and not by how many cancers were found.

### Wilson and Jungner: when screening is justified

In 1968 a WHO report by Wilson and Jungner laid out criteria still used today [Wilson & Jungner, WHO 1968]: the disease must be important; it must have a detectable preclinical phase; effective treatment for early disease must exist; the test must be acceptable to the population; the test must perform adequately; and crucially, **the benefits must outweigh the harms**. Most accepted programs fail at least one criterion somewhere. The accepted ones are those where benefit clearly dominates harm in a *defined* population.

## Worked Example

**Situation.** A single-cancer blood screen has **sensitivity 90%** and **specificity 99%** — numbers that sound superb. We apply it to two populations: (A) an asymptomatic general-population cohort where prevalence is **0.5%** (5 per 1,000), and (B) a high-risk cohort where prevalence is **10%**. What is the PPV in each?

**First attempt (the dead end).** A natural reading: "Specificity is 99%, so only 1% of results are wrong — a positive is 99% likely to be real." This is the mistake that sent the man in the opening case into a six-week workup. It confuses specificity (a property among the *disease-free*) with PPV (a property among the *test-positive*). They are not the same number, and the gap between them is set by prevalence.

**Population A — build the 2×2 on 100,000 people, prevalence 0.5%.**

- Diseased: 0.005 × 100,000 = **500**. TP = 0.90 × 500 = **450**; FN = 50.
- Disease-free: **99,500**. FP = 0.01 × 99,500 = **995**; TN = 98,505.
- PPV = TP / (TP + FP) = 450 / (450 + 995) = 450 / 1,445 = **31%**.

So a positive result is *real* only about 1 time in 3. Nearly **two-thirds of positives are false** — 995 healthy people sent for follow-up to find 450 true cancers. The "99% specific" test produces a PPV of 31% because the 1% of false positives is drawn from a vast healthy pool.

**Population B — same test, prevalence 10%.**

- Diseased: 10,000. TP = 9,000; FN = 1,000.
- Disease-free: 90,000. FP = 900; TN = 89,100.
- PPV = 9,000 / (9,000 + 900) = **91%**.

**Resolution.** The identical test — same sensitivity, same specificity — yields PPV 31% in the low-prevalence population and 91% in the high-prevalence one. Nothing about the test changed; only *who was tested* changed. This is why screening guidelines specify populations so narrowly (age bands, smoking pack-years, risk syndromes): targeting raises prevalence, which raises PPV, which reduces the harm-to-benefit ratio of false positives.

<!-- → [CHART: PPV as a function of prevalence at fixed sensitivity 90% / specificity 99% — curve climbing steeply from low prevalence] -->

**The lesson.** PPV is not a property of the test. A test is only as trustworthy as the population it is pointed at. "99% specific" tells you almost nothing about whether *your* positive result means cancer until you know how common the cancer is in people like you.

**The limit.** PPV is necessary but not sufficient. Even a test with perfect PPV could be useless if the cancers it finds are overdiagnosed (length and overdiagnosis bias) or if finding them earlier does not change the death rate (lead-time bias). PPV tells you whether a positive is real; it does not tell you whether acting on it saves a life. That requires a randomized trial with a mortality endpoint.

## Common Misconceptions

**"A more specific test means a positive result is almost certainly true."** This conflates specificity with PPV. As the Worked Example shows, a 99%-specific test had a PPV of 31% in a low-prevalence population, because the false positives are drawn from the large disease-free majority. This is precisely the error in the Opening Case — the man's "highly specific" result was treated as near-certain when its PPV in a low-risk person was modest at best.

**"Earlier detection always means better outcomes."** Earlier detection guarantees *longer measured survival from diagnosis* (lead-time bias) but does not guarantee a *later death*. A program can improve five-year survival statistics dramatically while leaving the age at death unchanged. Only disease-specific mortality, ideally in a randomized trial, separates real benefit from the lead-time illusion.

**"If we find more cancers, we're doing good."** Finding more cancers can reflect overdiagnosis — detecting indolent disease that would never have killed the patient. Counting detected cancers conflates benefit (catching lethal disease early) with harm (treating disease that needed no treatment). The man in the Opening Case illustrates the milder cousin: a "detection" that generated harm with no demonstrable disease at all.

**"Screening and diagnosis are basically the same procedure done earlier."** Screening operates on asymptomatic people where prevalence — and therefore PPV — is low; diagnostic testing operates on people with elevated pretest probability where the same test performs far better. A test appropriate for diagnosis can be inappropriate for screening for exactly this reason.

## Exercises

1. **(Recall/Understand.)** Define sensitivity, specificity, and PPV in one sentence each. State which of the three depends on disease prevalence and explain why.

2. **(Apply — produce a 2×2.)** A mammography program has sensitivity 85% and specificity 90%. In women aged 40–49, breast cancer prevalence at screening is roughly 0.4% [verify against current incidence data]. Build the full 2×2 table on 100,000 women, then compute PPV. Repeat for a 70-year-old cohort with prevalence 1.2%. Write one sentence explaining the difference in terms of who is being tested. Then state what *additional* evidence (beyond PPV) you would need before concluding the program saves lives.

3. **(Apply+.)** A new screening test reports that screen-detected patients have five-year survival of 80% versus 45% for symptom-detected patients. A colleague concludes the test "nearly doubles survival." Identify the three biases (lead-time, length-time, overdiagnosis) that could each, on their own, produce this gap with *zero* true benefit. For each bias, describe one feature of a study design that would let you rule it out.

4. **(Produce — a decision chart.)** Choose one screening program from the chapter (cervical, breast, colorectal, lung, or prostate). Draw a decision chart that takes a hypothetical patient from eligibility (age, risk factors) through a positive result to confirmatory workup, marking at each branch the rough probability of a true positive. Annotate where false positives enter and what harm they cause.

5. **(Evaluate.)** Apply the Wilson and Jungner criteria to prostate-specific antigen (PSA) screening. Identify which criteria it satisfies and which it strains, and explain why reasonable experts disagree about it [contested — see pantry flag].

## What Would Change My Mind

The chapter's central claim is that screening must be judged by population-level mortality reduction, because survival statistics, detection counts, and even PPV can each mislead. What would revise this? A large, well-conducted randomized trial of a multi-cancer early detection blood test (the NHS-Galleri trial enrolling ~140,000 people, or the NCI's prospective MCED studies) that demonstrated a clear reduction in *cancer-specific mortality* — not just more cancers found, not just longer survival from diagnosis, but fewer deaths — with an acceptable false-positive and overdiagnosis burden, would show that broad blood-based screening can deliver real benefit at population scale [NHS-Galleri; NCI MCED program]. Conversely, if such trials showed the now-familiar pattern — more diagnoses, better survival statistics, unchanged mortality — it would confirm that the biases described here remain the binding constraint on any new screening technology, however sophisticated.

## Still Puzzling

- For multi-cancer detection tests, the curable early-stage cancers shed the least circulating tumor DNA — precisely the cancers screening most needs to catch. Can sensitivity at stage I ever be high enough to matter, or is there a floor set by tumor biology? [contested]
- How should overdiagnosis be counted when it is, by construction, invisible at the individual level? We can never know which particular screen-detected patient was overdiagnosed — only the population rate. What does informed consent even mean under that uncertainty?
- Risk-stratified screening (polygenic scores, family history, biomarkers) promises to raise prevalence in the screened group and thus PPV. But does concentrating screening on the highest-risk people leave too many cancers in the larger, lower-risk majority where most absolute cases actually arise?

## References

- National Cancer Institute. *Cancer Screening Tests.* https://www.cancer.gov/about-cancer/screening/screening-tests
- National Cancer Institute. *Cancer Screening Overview.* https://www.cancer.gov/about-cancer/screening
- Wilson JMG, Jungner G. *Principles and Practice of Screening for Disease.* WHO, 1968.
- US Preventive Services Task Force. Screening recommendations (breast, cervical, colorectal, lung, prostate). https://www.uspreventiveservicestaskforce.org
- National Lung Screening Trial (NLST) Research Team. Reduced lung-cancer mortality with low-dose CT screening. *N Engl J Med* 2011.
- European Randomized Study of Screening for Prostate Cancer (ERSPC); PLCO trial — conflicting PSA screening mortality results.
- NHS-Galleri trial (multi-cancer early detection); NCI MCED prospective studies.
- National Cancer Institute. *Tests and Procedures Used to Diagnose Cancer.* https://www.cancer.gov/about-cancer/diagnosis-staging/diagnosis

## Prompts

*No figures have been generated for this chapter yet.*
*Run the Cowork enrichment pass to populate this section.*
