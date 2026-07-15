<!-- deck
title: Chapter 2: Editing Genomes
theme: sage
ratio: 16:9
author: Yu Wang
footer: Coursewerk demonstration · Not for actual teaching · CC BY-SA 4.0
-->

<!-- slide template=title v=5 -->
# Editing Genomes
## Repair outcomes, delivery, limits, and decisions

**AI-generated Coursewerk demonstration—not intended for actual teaching or clinical guidance**

<!-- slide 2col -->
## Learning objectives
<!-- @left -->
- {{sp[info] 2.1}} Design the claim before the reagent
- {{sp[info] 2.2}} Predict repair outcome distributions
<!-- @right -->
- {{sp[info] 2.3}} Compare delivery and validation strategies
- {{sp[info] 2.4}} Separate evidence from governance judgments

:::success
**Repeated question:** What was changed, in which cells, how was it measured, and what conclusion follows?
:::

<!-- slide template=outline v=5 -->
# Chapter route
- Claim → intended molecular change
- Editor + delivery → exposure
- Cellular process → allele distribution
- Validation → bounded interpretation
- Context → governance

<!-- slide -->
## Editing is a chain, not an event
{{mermaid
flowchart LR
  A[question] --> B[intended change]
  B --> C[target + editor]
  C --> D[delivery]
  D --> E[molecular action]
  E --> F[cellular outcome]
  F --> G[validation]
  G --> H[bounded claim]
}}

**Visual description:** A question leads to an intended change, editor design, delivery, molecular action, cellular outcome, validation, and only then a bounded claim.

<!-- slide template=section v=2 -->
# 2.1 Design the claim
## The assay plan starts before the guide sequence

<!-- slide 2col -->
## Molecular target vs biological claim
<!-- @left -->
{{sp[success] Directly testable}}

- target locus changed
- allele frequencies differ
- RNA or protein level changed
<!-- @right -->
{{sp[warning] Requires more links}}

- function restored
- phenotype caused by the edit
- intervention is safe or beneficial

<!-- slide step -->
## Build the design backward
1. State the bounded biological claim.
2. Define the required molecular outcome.
3. Choose target and editor chemistry.
4. Select delivery for the cells and duration.
5. Precommit assays and controls.

<!-- slide template=section v=3 -->
# 2.2 Repair creates outcomes
## The cell finishes the edit

<!-- slide main-side 3/2 -->
## One lesion, several pathways
<!-- @main -->
![Targeted DNA lesion branching into multiple repair pathways and a mixed allele population](https://alembic.orz.how/d/doc-l4xqle1syvaf =650x)
<!-- @side -->
- NHEJ can be precise or mutagenic
- MMEJ often yields patterned deletions
- HDR depends on template and cell state
- unedited cells can remain

<!-- slide 3col -->
## Three repair logics
<!-- @left -->
**End joining**

reconnect available ends
<!-- @mid -->
**Microhomology**

align short matching regions
<!-- @right -->
**Template-supported**

copy from related sequence

<!-- slide 2col -->
## “90% edited” can hide the result
<!-- @left -->
**Collapsed report**

- 90% non-reference reads
- 10% reference reads
<!-- @right -->
**Needed report**

- identity of each allele
- frequency and uncertainty
- predicted and measured function
- sampling limits

<!-- slide 2col -->
## Non-break editors change—not erase—uncertainty
<!-- @left -->
**Base editing**

targeted chemical conversion within an activity window
<!-- @right -->
**Prime editing**

guide-directed templated rewriting architecture

:::warning
No programmed double-strand break ≠ no by-products or unintended effects.
:::

<!-- slide template=section v=4 -->
# 2.3 Delivery and validation
## Delivery is part of the causal mechanism

<!-- slide main-side 3/2 -->
## Three exposure profiles
<!-- @main -->
![Comparison of DNA, RNA, and RNP delivery trade-offs](https://alembic.orz.how/d/doc-0vzwjh1vbdpr =650x)
<!-- @side -->
- DNA: expression required
- mRNA: transient translation
- RNP: rapid preassembled activity
- cell type changes every trade-off

<!-- slide main-side 3/2 -->
## Measurements are physical
<!-- @main -->
![Researcher pipetting DNA into an electrophoresis gel](https://alembic.orz.how/d/doc-bfmos4nfl7qg =520x)
<!-- @side -->
- sample preparation matters
- every assay has resolution limits
- expected band size is not full sequence identity
- orthogonal evidence adds confidence

*Maggie Bartlett/NHGRI; public domain.*

<!-- slide main-side 3/2 -->
## Climb the evidence ladder
<!-- @main -->
![Evidence ladder from delivery through locus, function, phenotype, and causal claim](https://alembic.orz.how/d/doc-vfqc3uude56x =650x)
<!-- @side -->
1. reagent delivery
2. target-locus identity
3. allele distribution
4. molecular function
5. phenotype
6. bounded causal claim

<!-- slide quad -->
## Four distinct quality questions
<!-- @tl -->
**On-target efficiency**

how much target changed?
<!-- @tr -->
**On-target heterogeneity**

which changes occurred?
<!-- @bl -->
**Off-target activity**

what changed elsewhere?
<!-- @br -->
**Biological effect**

did function and phenotype change?

<!-- slide step -->
## Assay-bound reasoning
**Result:** Short amplicons contain the intended substitution.

1. Supported: sampled local sequence includes the change.
2. Not yet supported: every cell is edited.
3. Not yet supported: no larger on-target change.
4. Not yet supported: genome-wide specificity or functional rescue.

<!-- slide template=section v=5 -->
# 2.4 Context and governance
## Technical accuracy is necessary—not sufficient

<!-- slide quad -->
## Same editor, different decisions
<!-- @tl -->
**Research model**

knowledge and model validity
<!-- @tr -->
**Somatic intervention**

consent, benefit, monitoring
<!-- @bl -->
**Heritable intervention**

future generations and alternatives
<!-- @br -->
**Ecological release**

spread, reversibility, community voice

<!-- slide 2col -->
## Keep two question types visible
<!-- @left -->
{{sp[success] Empirical}}

- What changed?
- How often?
- With what uncertainty?
- What effects followed?
<!-- @right -->
{{sp[warning] Normative}}

- Which risks are acceptable?
- Who decides?
- Who benefits or bears costs?
- What duties persist over time?

<!-- slide template=closing v=2 -->
# Take-home model
- Design the claim before the reagent.
- The cell converts molecular action into allele distributions.
- Delivery determines exposure and stress.
- Validation must connect genotype, function, and phenotype.
- Governance depends on context, not technical accuracy alone.

<!-- slide -->
## Sources and media
Text adapted and reorganized from [CRISPR gene editing](https://en.wikipedia.org/wiki/CRISPR_gene_editing), [Genome editing](https://en.wikipedia.org/wiki/Genome_editing), [DNA repair](https://en.wikipedia.org/wiki/DNA_repair), and [Cas9](https://en.wikipedia.org/wiki/Cas9) by Wikipedia contributors, [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Exact revisions: `metadata/SOURCE_RECORD.json`.

Lab photos: Maggie Bartlett/NHGRI and NIH/NIAMS, public domain. Original SVG diagrams: Yu Wang, CC BY-SA 4.0.

**Demo only—not intended for actual teaching or clinical use.**
