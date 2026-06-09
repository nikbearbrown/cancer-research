# Radiation Oncology: Principles and Biology

## Learning Objectives

After working through this chapter, you should be able to:

- **Explain** how ionizing radiation kills cells, distinguishing the *direct* and *indirect* mechanisms of DNA damage and naming the most lethal lesion.
- **Use** the linear-quadratic model and the α/β ratio to explain *why fractionation works* — how splitting a dose into many small fractions favors tumor kill over late normal-tissue injury.
- **State and apply** the five Rs of radiobiology (Withers) to predict how a change in fractionation will affect tumor and normal-tissue outcomes.
- **Define** the therapeutic ratio as the gap between tumor cure dose and normal-tissue tolerance, and **evaluate** when that gap is comfortable and when it is narrow.
- **Produce** a comparison of two fractionation schedules for a given α/β ratio, computing the biologically effective dose and stating the trade-off.

## Opening Case

Two patients lie on two linear accelerators. The first has a head-and-neck cancer; the plan calls for 70 Gray (Gy — the unit of absorbed radiation dose) delivered in 35 daily fractions of 2 Gy over seven weeks. The second has the same total prescription written a different way by a hurried trainee: 70 Gy delivered in *ten* fractions of 7 Gy, finishing in two weeks. Same total dose. Same beams. Same tumor.

The first patient's tumor is controlled and her spinal cord, salivary glands, and mucosa recover. The second plan, had it been delivered, would have been a catastrophe: the larger fractions would have driven the late-responding normal tissues — spinal cord especially — far past tolerance, risking permanent paralysis, while not improving tumor control enough to justify it. The total dose was identical. The *biological* dose to the normal tissue was not.

Radiation damages DNA indiscriminately — it cannot tell a cancer cell from a spinal-cord neuron. So how does the same total dose, merely *divided differently*, spare the patient or destroy her? This chapter is about the answer: the therapeutic effect of radiation is not read off the total dose. It is *engineered* — produced by exploiting a measurable biological difference between tumor and normal tissue, fraction by fraction.

## Core Concepts

### How radiation kills: direct and indirect DNA damage

**Ionizing radiation** transfers energy to tissue and **ionizes** atoms — knocking out electrons, breaking chemical bonds, and generating reactive species [cba-35]. The most consequential target is DNA, damaged two ways:

- **Direct effect** — radiation energy breaks a DNA bond outright. Dominant for **high-LET** (high linear energy transfer) radiation such as alpha particles and protons at the end of their range [cba-35].
- **Indirect effect** — radiation ionizes the water surrounding DNA, producing **reactive oxygen species** (hydroxyl radicals and others) that diffuse a short distance and damage DNA. This is the dominant mechanism for **low-LET** radiation like the X-rays from a clinical linear accelerator [cba-35].

Among the lesions — single-strand breaks, base modifications, crosslinks — the **double-strand break** is the most lethal, because it is hard to repair accurately [cba-35]. A standard 2 Gy fraction produces roughly **40 double-strand breaks per cell** [cba-35].

The indirect mechanism has a clinically crucial dependency: it *requires oxygen*. Hold that fact — it returns as reoxygenation below, and it is why hypoxic tumor regions resist radiation.

### Why the same dose can spare or destroy: the linear-quadratic model

The relationship between dose and cell kill is captured by the **linear-quadratic (LQ) model**. The surviving fraction (SF) of cells after a dose *D* is:

**SF = exp(−αD − βD²)**

- The **α** term is linear cell kill — single-track damage that is lethal on its own.
- The **β** term is quadratic — two separate damage events combining to become lethal [cba-35].

The ratio **α/β** characterizes a tissue's response to *fraction size*, and it is the single number that explains the opening case:

- **High α/β tissues (~10 Gy)** — most cancers, plus acutely responding normal tissues (skin, mucosa, marrow). Their kill depends mostly on *total* dose; they are relatively insensitive to how the dose is split [cba-35].
- **Low α/β tissues (~3 Gy or less)** — late-responding normal tissues: spinal cord, brain, lung, kidney. These are *highly sensitive to fraction size* — large fractions hurt them far more than the same total dose given in many small fractions [cba-35].

That asymmetry is the whole game. Because late-responding normal tissue has a low α/β and most tumors have a high α/β, **small fractions punish the tumor while sparing the late-responding normal tissue**. The trainee's 7 Gy fractions in the opening case would have hammered the low-α/β spinal cord exactly where it is most vulnerable [cba-35].

<!-- → [CHART: cell-survival curves under the LQ model for high-α/β tumor vs. low-α/β late-responding tissue, showing how the curves diverge as fraction size increases] -->

### The therapeutic ratio

The **therapeutic ratio** is the gap between the dose that controls the tumor and the dose that injures normal tissue [cba-35]. Fractionation does not change the *physics* of where the dose lands; it changes the *biology* of how tumor and normal tissue respond to it, widening that gap. **Fractionation is the act of engineering a therapeutic ratio out of an indiscriminate weapon.**

For some cancers the ratio is comfortable — Hodgkin lymphoma is cured at 20–30 Gy, well below normal-tissue tolerance [cba-35]. For others it is narrow — head-and-neck cancers need ~70 Gy, brushing several organ tolerances at once [cba-35]. The narrower the ratio, the more the fractionation scheme and beam precision matter.

### The five Rs of radiobiology

The classical framework explaining *why fractionated radiation works*, attributed to **Withers**, is the **five Rs** [cba-35; Withers]:

- **Repair.** Between fractions, normal tissue repairs sublethal damage better than tumor tissue (which often has a defective DNA-damage response). This repair differential is the basis of the fractionation advantage [cba-35].
- **Repopulation.** Cells divide during a treatment course. Acutely responding normal tissue *needs* to repopulate to stay functional — but so can a fast-growing tumor, which is why dragging treatment out can let the tumor regrow; accelerated fractionation counters this in head-and-neck cancer [cba-35].
- **Redistribution.** Cells in different cell-cycle phases differ in radiosensitivity (G2/M most sensitive, S most resistant). Fractionation lets cells caught in resistant phases redistribute into sensitive ones before the next fraction [cba-35].
- **Reoxygenation.** Hypoxic tumor cells are 2–3× more radioresistant (the indirect mechanism needs oxygen). After a fraction kills the well-oxygenated cells, the surviving hypoxic cells gain better blood supply and become oxygenated — and vulnerable to the next fraction [cba-35].
- **Radiosensitivity.** Intrinsic sensitivity varies by cell type and molecular state — p53 status, repair-pathway status (BRCA-mutant cells are more sensitive), and more [cba-35].

A sometimes-added sixth R is **Reactivation** of the immune system — radiation can provoke immune responses beyond direct kill, the basis for radiation-immunotherapy combinations [cba-35].

<!-- → [DIAGRAM: the five Rs across a fractionation course — repair, repopulation, redistribution, reoxygenation, radiosensitivity shown as what happens to tumor vs. normal tissue between fractions] -->

### Delivering the dose: fractionation schemes

The LQ model and the five Rs translate directly into how radiation is scheduled:

- **Conventional fractionation** — ~2 Gy/day, the workhorse, maximizing the repair differential [cba-35].
- **Hypofractionation** — fewer, larger fractions. Justified when the *tumor* has a low α/β. Prostate cancer (α/β ≈ 1.5) is the canonical case: it responds *like* a late-responding tissue, so larger fractions are biologically efficient, enabling SBRT regimens of ~36–40 Gy in 5 fractions [cba-35]. The **START trials** established that moderate hypofractionation for breast cancer (15–16 fractions instead of 25–30) gives equivalent outcomes [cba-35; START].
- **Stereotactic body radiotherapy (SBRT)** — extreme hypofractionation, 10–25 Gy per fraction in 1–5 fractions, made safe by conformal targeting [cba-35].
- **Brachytherapy** — radioactive sources placed *in or beside* the tumor, giving high local dose with steep falloff [cba-35].

## Worked Example

**Situation.** Compare two prostate-cancer plans, given prostate α/β ≈ 1.5 Gy [cba-35]:

- **Plan A:** 60 Gy in 30 fractions of 2 Gy (conventional).
- **Plan B:** 36.25 Gy in 5 fractions of 7.25 Gy (SBRT).

The crude objection: "Plan B delivers only 36 Gy and Plan A delivers 60 Gy — Plan B must badly undertreat the tumor." Is that right?

**The reasoning — including a dead end.**

The dead end is comparing *physical* total doses directly: 36 < 60, so Plan B looks like under-dosing by a third. This is exactly the trap the opening case sets — total Gy is not biological effect. Two schedules with different fraction sizes are not on the same biological scale, and subtracting their totals is meaningless.

The productive path is to convert each to a common currency: **biologically effective dose (BED)**, BED = *n · d · [1 + d/(α/β)]*, where *n* is the number of fractions and *d* the dose per fraction.

- **Plan A (conventional), α/β = 1.5:** BED = 60 · [1 + 2/1.5] = 60 · [1 + 1.333] = 60 · 2.333 = **140 Gy** (BED units).
- **Plan B (SBRT), α/β = 1.5:** BED = 36.25 · [1 + 7.25/1.5] = 36.25 · [1 + 4.833] = 36.25 · 5.833 = **211 Gy** (BED units).

Far from under-treating, Plan B delivers a *higher* biologically effective dose to the tumor — because the prostate's low α/β means large fractions are disproportionately effective. The 7.25 Gy fractions land on the steep, fraction-size-sensitive part of the survival curve [cba-35]. (For a high-α/β tissue, the same arithmetic would show much less amplification — which is exactly why hypofractionation is *safe* only where the tumor's α/β is low and dangerous where a low-α/β *normal* tissue is in the field, as in the opening case.)

**Resolution.** Plan B is not under-dosing; it exploits prostate radiobiology to deliver more biological dose in fewer visits. The crude total-Gy comparison fails because it ignores α/β.

**The lesson.** Radiation dose is not a single number you can add and subtract across schedules. The *biological* effect depends on fraction size and the tissue's α/β. Fractionation is a lever, and the LQ model tells you which way it moves tumor versus normal tissue.

**The limit.** The LQ model is an approximation, and it is least reliable at the very high fraction sizes used in SBRT (above ~8–10 Gy per fraction), where additional mechanisms — vascular damage and immune effects — may contribute and the simple LQ extrapolation can mislead [cba-35; contested — see pantry flag]. BED arithmetic guides, but does not replace, clinical trial evidence at the extremes.

## Common Misconceptions

**"More total dose is always more tumor kill, and the schedule is just logistics."** Plausible — dose is the obvious variable, and "more is more" is intuitive. It fails because fraction *size*, via α/β, can change the biological effect of the same total dose dramatically — the opening case (70 Gy safe in 35 fractions, catastrophic in 10) and the worked example (36 Gy biologically *exceeding* 60 Gy for prostate) both break it.

**"Hypofractionation is just a convenient shortcut with no biological basis."** Plausible, since fewer visits is plainly convenient. It fails because hypofractionation is *justified specifically* when the tumor's α/β is low (prostate ≈ 1.5), where large fractions are biologically efficient — and is *dangerous* where a low-α/β normal tissue sits in the field [cba-35]. The convenience is real; the licence for it is radiobiological, not logistical.

**"Radiation works by selectively targeting cancer cells."** Plausible — it is a precise, targeted-sounding therapy. It fails because radiation damages DNA *indiscriminately*; it cannot distinguish a tumor cell from a spinal-cord neuron [cba-35]. The selectivity is *engineered* — through fractionation (the repair differential), conformal beam targeting, and the five Rs — not intrinsic to the radiation.

**"If a tumor isn't responding, just raise the dose."** Plausible — escalation is the obvious move. It fails when the limiting factor is **hypoxia**: hypoxic cells are 2–3× radioresistant because the indirect kill mechanism needs oxygen, and no feasible dose escalation overcomes that without also exceeding normal-tissue tolerance [cba-35]. The answer is reoxygenation across fractions or hypoxia-directed strategies, not brute force.

## Exercises

1. **(Comprehension.)** Distinguish the direct and indirect mechanisms of radiation-induced DNA damage. Which dominates for the X-rays of a clinical linear accelerator, and why does that mechanism make tumor oxygenation matter?

2. **(Apply.)** Using the five Rs, predict what happens if a seven-week head-and-neck treatment course is interrupted for two weeks by a machine breakdown. Which of the Rs works *against* the patient during the gap, and what fractionation strategy is used to counter it? [cba-35]

3. **(Apply — quantitative.)** A late-responding normal tissue has α/β = 3 Gy. Compute the BED for (a) 60 Gy in 30 fractions of 2 Gy and (b) 60 Gy in 10 fractions of 6 Gy. Show that the *same total dose* gives a higher BED to this tissue under the large-fraction schedule, and explain in one sentence why that endangers the spinal cord in the opening case.

4. **(Produce.)** For a tumor with α/β = 10 Gy, design *two* fractionation schedules that deliver an approximately equal tumor BED, one conventional and one moderately hypofractionated. Compute both BEDs, then write two sentences on what you would need to check about the *normal tissues* in the field before choosing the hypofractionated option.

5. **(Evaluate.)** Find the published result of one START trial (breast hypofractionation) or a prostate SBRT trial. State the fractionation compared, the primary outcome, and whether equivalence (or superiority) was shown. In two sentences, connect the result to the α/β reasoning in this chapter.

## What Would Change My Mind

The central claim is that radiation's selectivity is *engineered* — produced by fractionation exploiting the α/β difference between tumor and late-responding normal tissue, as described by the linear-quadratic model and the five Rs — rather than being an intrinsic property of the radiation. What would revise this is convincing evidence that, at the high doses used in modern SBRT, the dominant determinant of outcome is *not* the LQ/α/β framework but a distinct mechanism — vascular collapse, endothelial death, or radiation-triggered immunity — that fractionation reasoning fails to capture. If clinical outcomes at extreme fraction sizes systematically departed from BED predictions in a way explained by these alternative mechanisms, the "engineered therapeutic ratio via α/β" account would become a special case valid only at conventional fraction sizes [cba-35; contested — see pantry flag]. The data on this are actively debated.

## Still Puzzling

- Does the linear-quadratic model break down at SBRT fraction sizes, and if so, what replaces it — vascular effects, immune activation, or a modified LQ? [contested — see pantry flag]
- How much of SBRT's effect is direct DNA-damage cell kill versus indirect (vascular and immune) mechanisms, and can the two be disentangled clinically? [verify]
- Reoxygenation predicts that fractionation should overcome hypoxia, yet hypoxic tumors remain stubbornly radioresistant. Why doesn't reoxygenation fully rescue them, and which hypoxia-directed strategies actually help?
- Can we measure a *patient-specific* α/β or radiosensitivity before treatment, rather than relying on population averages — and would individualizing fractionation on that basis improve the therapeutic ratio?

## References

- Source chapter (cba-35), *Radiation Oncology: Principles and Biology*, for DNA-damage mechanisms, the linear-quadratic model and α/β ratios, the five Rs, fractionation schemes, tissue tolerances, and tumor cure doses.
- Withers HR. *The Four R's of Radiotherapy* (origin of the Rs framework; later extended to five). *Advances in Radiation Biology*, 1975.
- START Trialists' Group. *The UK Standardisation of Breast Radiotherapy (START) Trials* of radiotherapy hypofractionation for breast cancer. *Lancet* / *Lancet Oncology*, 2008.
- National Cancer Institute. *Radiation Therapy to Treat Cancer.* https://www.cancer.gov/about-cancer/treatment/types/radiation-therapy
- Background units and dose-tolerance values (TD5/5, BED formula) per standard radiation-oncology references [verify specific tolerance figures against current QUANTEC constraints].

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
