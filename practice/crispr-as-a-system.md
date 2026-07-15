# Chapter 1 Practice: CRISPR as a Biological System

:::warning
**Demonstration only:** This practice set shows what Coursewerk can produce. It is not intended for direct use in actual teaching.
:::

These 15 items cover every chapter objective. Attempt each question before revealing the worked answer.

**(Objective 1 · component classification)**

:::: tabs
::: tab Q
Classify each item as a **sequence record**, **RNA guide component**, **protein**, or **engineered shorthand**: (a) a spacer within a CRISPR array; (b) tracrRNA; (c) Cas9; (d) “CRISPR–Cas9.”
:::
::: tab Answer
(a) sequence record; (b) RNA guide component; (c) protein; (d) engineered shorthand for a system assembled from multiple components. The shorthand should not be treated as the name of every natural CRISPR system.
:::
::::

**(Objective 1 · array interpretation)**

:::: tabs
::: tab Q
A locus is written as leader–repeat–spacer A–repeat–spacer B–repeat. Which feature is repeated, and which features can preserve sequence information from different encounters?
:::
::: tab Answer
The repeat sequence is repeated. Spacer A and spacer B can preserve sequence-derived information from different prior encounters. The leader is a neighboring regulatory region, not another spacer.
:::
::::

**(Objective 2 · pathway ordering)**

:::: tabs
::: tab Q
Put these stages in order: interference; acquisition of a new spacer; guide-RNA biogenesis; recognition of a matching target.
:::
::: tab Answer
Acquisition of a new spacer → guide-RNA biogenesis → recognition of a matching target → interference. The first stage changes the array; the later stages use information represented in it.
:::
::::

**(Objective 2 · stage failure)**

:::: tabs
::: tab Q
A bacterium retains its CRISPR array and interference proteins but cannot acquire new spacers. Which capability is most directly impaired, and which might remain?
:::
::: tab Answer
Adaptation to newly encountered sequence information is most directly impaired. Use of already present spacers for guide production and interference might remain, provided the corresponding processing and effector components still function.
:::
::::

**(Objective 2 · guide formation)**

:::: tabs
::: tab Q
In a simplified type II system, explain the relationship among pre-crRNA, tracrRNA, and an engineered single-guide RNA.
:::
::: tab Answer
The pre-crRNA is transcribed from the array and processed to provide spacer-derived targeting information. tracrRNA pairs with repeat-derived RNA and helps form the Cas9 guide complex. An engineered single-guide RNA joins key crRNA and tracrRNA functions into one molecule; it is a laboratory design, not a claim that all natural systems use one RNA.
:::
::::

**(Objective 3 · spacer/protospacer/PAM)**

:::: tabs
::: tab Q
Distinguish a spacer, a protospacer, and a PAM without calling all three “the target.”
:::
::: tab Answer
A spacer is stored within the CRISPR array. A protospacer is the corresponding sequence in the encountered or experimental target DNA. A PAM is a short neighboring motif recognized by a particular effector system; it is adjacent to the protospacer rather than copied into the spacer in the same way.
:::
::::

**(Objective 3 · claim boundary)**

:::: tabs
::: tab Q
Two DNA sites match a guide equally well. Site A is next to a PAM recognized by the chosen SpCas9; site B is not. Which site is the stronger candidate for productive targeting, and what remains uncertain?
:::
::: tab Answer
Site A is the stronger candidate because guide complementarity and a compatible neighboring PAM are both required in this simplified SpCas9 model. Productive cleavage is still not guaranteed: chromatin, molecular context, mismatches, enzyme state, and experimental conditions can alter the outcome.
:::
::::

**(Objective 3 · avoid overgeneralization)**

:::: tabs
::: tab Q
Repair this statement: “Every CRISPR nuclease requires the sequence 5′-NGG-3′.”
:::
::: tab Answer
“A commonly used *Streptococcus pyogenes* Cas9 recognizes PAMs often summarized as 5′-NGG-3′, but PAM preferences differ among CRISPR effectors and variants.” The example is system-specific, not a universal CRISPR rule.
:::
::::

**(Objective 4 · checkpoint evidence)**

:::: tabs
::: tab Q
An experiment detects Cas9 bound near a DNA site but finds no double-strand break. Which checkpoint has evidence, and which has not been demonstrated?
:::
::: tab Answer
The data support target engagement or stable binding under the assay conditions. They do not demonstrate completion of the conformational and catalytic steps required for double-strand cleavage.
:::
::::

**(Objective 4 · mismatch reasoning)**

:::: tabs
::: tab Q
A single guide–DNA mismatch reduces cleavage at one site but not another. Why is “one mismatch prevents Cas9 cleavage” too strong?
:::
::: tab Answer
Mismatch effects depend on position, number, surrounding sequence, effector variant, and assay context. These observations show that the tested mismatch had a context-dependent effect; they do not establish a universal one-mismatch rule.
:::
::::

**(Objective 4 · model repair)**

:::: tabs
::: tab Q
Replace the “exact string search” model of Cas9 targeting with a four-step checkpoint model.
:::
::: tab Answer
One defensible simplified model is: compatible PAM sampling → local DNA opening → guide–target pairing → catalytic activation and strand cleavage. The steps emphasize that complementarity is necessary in many designs but is not by itself a complete prediction of activity.
:::
::::

**(Objective 5 · active Cas9 versus dCas9)**

:::: tabs
::: tab Q
A Cas9 variant is guided to a promoter, remains bound, and changes transcription without detectable DNA cleavage. Which platform best fits the observation?
:::
::: tab Answer
Catalytically inactive Cas9, or dCas9, best fits: guide-directed binding is retained while nuclease activity is disabled. The transcriptional effect could arise from steric interference or from a fused regulatory domain, depending on the construct.
:::
::::

**(Objective 5 · nickase comparison)**

:::: tabs
::: tab Q
How does a Cas9 nickase differ conceptually from active Cas9 and dCas9?
:::
::: tab Answer
Common active Cas9 can cleave both DNA strands through two nuclease domains. A nickase has one catalytic activity disabled and ordinarily cuts one strand under the simplified model. dCas9 has both catalytic activities disabled and is used primarily as a programmable binding platform.
:::
::::

**(Objective 6 · controlled comparison)**

:::: tabs
::: tab Q
Guide X and guide Y target different sites and produce different cleavage levels. Can the difference be attributed to guide sequence alone? Design a better comparison.
:::
::: tab Answer
Not from that observation alone: target context, PAM, chromatin accessibility, measurement, and delivery may differ. A better comparison changes one defined factor at a time, uses matched delivery and measurement conditions, includes replicates and controls, and reports the remaining contextual differences.
:::
::::

**(Objectives 1–6 · synthesis)**

:::: tabs
::: tab Q
Write a four-link evidence chain from a CRISPR array to cleavage of an invading DNA sequence, naming one uncertainty at each transition.
:::
::: tab Answer
Array spacer → processed guide RNA (**uncertainty:** processing and guide abundance) → guide-bearing effector complex (**uncertainty:** assembly and localization) → PAM-dependent target engagement and pairing (**uncertainty:** context and mismatch tolerance) → catalytic cleavage (**uncertainty:** conformational activation and enzyme activity). The chain makes clear why a sequence match alone is not proof of cleavage.
:::
::::

**Text adaptation:** Chapter concepts are adapted and reorganized from the revision-bound Wikipedia sources in `metadata/SOURCE_RECORD.json`, CC BY-SA 4.0.
