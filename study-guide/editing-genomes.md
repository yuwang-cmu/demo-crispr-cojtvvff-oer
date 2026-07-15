# Chapter 2: Editing Genomes—Repair Outcomes, Delivery, Limits, and Decisions

:::warning
**Demonstration only:** This AI-generated Coursewerk chapter is not intended for direct use in actual teaching, laboratory work, or clinical decision-making. It has not been subject-matter or classroom validated.
:::

:::info
**Reference:** Five-article, revision-bound English Wikipedia corpus; exact revisions in `metadata/SOURCE_RECORD.json`  
**Audience:** Introductory undergraduate biology and biotechnology learners  
**Package license:** CC BY-SA 4.0  
**Safety boundary:** Conceptual design and evidence reasoning only; no operational editing protocol
:::

:::success
**Chapter Learning Objectives**

- **2.1a–b:** Separate intended change, targeting, delivery, molecular action, repair, and selection.
- **2.2a–b:** Predict why break repair generates multiple alleles and why non-break editors still require outcome analysis.
- **2.3a–b:** Compare delivery strategies and construct a layered validation plan.
- **2.4a–b:** Distinguish technical evidence from context-specific ethical and governance judgments.
:::

## Chapter Logic

Genome editing is not one event. A question motivates an intended change; a targeting system must reach appropriate cells; molecular chemistry creates a lesion or conversion; cellular processes generate outcomes; assays sample those outcomes; and interpretation links genotype to function and phenotype. Weak claims skip steps. Strong claims make each link visible.

{{mermaid
flowchart LR
  A[question] --> B[intended change]
  B --> C[target and editor]
  C --> D[delivery]
  D --> E[molecular action]
  E --> F[cellular repair or conversion]
  F --> G[allele distribution]
  G --> H[validation]
  H --> I[function and phenotype]
  I --> J[bounded claim]
  K[controls and uncertainty] --> H
  K --> I
  K --> J
}}

**Visual description:** An editing claim forms a chain from question and intended change through target design, delivery, molecular action, cellular outcome, allele distribution, validation, function, phenotype, and a bounded claim. Controls and uncertainty support the final evidence steps.

## 2.1 Design the Claim Before the Reagent{{attrs[#blk-workflow21]}}

:::success
**Learning Objectives**

- Translate a biological question into an intended molecular and functional change.
- Distinguish an editing component from the claim it is supposed to support.
:::

An experiment should begin with the narrowest useful claim. “Gene X causes trait Y” is usually too broad. A more testable chain might be: changing a defined sequence alters a transcript, which changes a protein activity under specified conditions, which shifts a measured phenotype. That chain determines the required editor, cells, controls, assays, and time points.

Target choice includes more than sequence complementarity. A target needs compatible recognition context, a plausible route to the intended molecular outcome, and assays that can distinguish alternatives. Editing a coding exon to disrupt function, replacing a pathogenic base, repressing a promoter with dCas9, and inserting a tag are different tasks even if they use related targeting machinery.

| Design layer | Question | Example failure if skipped |
|---|---|---|
| Biological claim | What exactly should change, where, and under what conditions? | A phenotype is observed but cannot be linked to the intended mechanism. |
| Molecular outcome | Knockout, substitution, insertion, regulation, or other? | A break produces alleles that do not implement the intended change. |
| Target context | Is the site recognizable and biologically interpretable? | A convenient site has no useful functional consequence. |
| Delivery | Which cells receive how much editor for how long? | Strong editing occurs only in the wrong cells or with excessive stress. |
| Validation | Which assays rule out plausible alternatives? | One sequencing readout is treated as proof of function. |

:::: tabs
::: tab Problem
The intended claim is “loss of protein P reduces response R.” A team plans only to measure insertions and deletions at the DNA target. Name two additional evidence layers.
:::
::: tab Solution
They should verify that protein P is actually reduced or functionally impaired, then measure response R with appropriate controls. Replicate samples and a rescue or independent perturbation would further test whether the phenotype is caused by loss of P rather than delivery stress or another change.
:::
::::

**Self-check:**

- Why can the same target site be unsuitable for two different intended changes?
- Which claim can target-locus sequencing support directly, and which can it not?
- What negative and positive controls follow from the biological question?

## 2.2 A Break Produces a Distribution, Not a Command{{attrs[#blk-repair22]}}

:::success
**Learning Objectives**

- Compare end joining, microhomology-mediated joining, and template-supported repair.
- Explain why edited populations can contain many alleles, including unedited cells.
:::

A nuclease-induced double-strand break recruits pathways that evolved to protect genomes, not to obey an engineer's desired sequence. **Non-homologous end joining (NHEJ)** can rejoin ends precisely or after processing that creates insertions or deletions. **Microhomology-mediated end joining (MMEJ)** aligns short matching regions and commonly produces deletions. **Homologous recombination or homology-directed repair (HDR)** can copy from a related template when the necessary template and cellular state are available.

![Diagram branching from a targeted DNA lesion to several repair pathways and a mixed allele population](https://alembic.orz.how/d/doc-l4xqle1syvaf)

*Figure 2.1. A programmed lesion leads to context-dependent repair outcomes. Original schematic by Yu Wang.*

**Visual alternative:** A targeted lesion enters a cell and branches to end joining, microhomology-mediated joining, and template-supported repair. All branches converge on a box labelled “mixture of alleles and unedited cells,” with cell type, timing, delivery, locus, and assay listed as influences.

The word **knockout** describes a functional goal, not a guaranteed DNA pattern. An insertion or deletion may disrupt a reading frame, preserve it, alter splicing, or create an unexpected protein. Conversely, a sequence change can be functional without being a frameshift. The genotype distribution must be connected to the biological function actually tested.

Base editors and prime editors expand the design space by coupling programmable targeting to conversion or templated-writing chemistries without intentionally making the same double-strand break used by ordinary nuclease editing. They can reduce some classes of outcome while introducing other constraints and by-products. “No programmed double-strand break” does not mean “no unintended consequence.”

:::: tabs
::: tab Problem
Sequencing shows 55% allele A, 25% allele B, 10% allele C, and 10% unedited sequence. Why is reporting “90% editing efficiency” incomplete?
:::
::: tab Solution
The 90% figure collapses three different edited alleles. Their functional consequences may differ: one could implement the intended change, another could be neutral, and another harmful. The result should report allele identities and frequencies, sampling uncertainty, and the relationship between each genotype and the functional claim.
:::
::::

**Self-check:**

- Can NHEJ ever restore the original sequence precisely?
- Why does cell-cycle state influence access to homologous templates?
- What information is lost when all non-reference reads are grouped as “edited”?

## 2.3 Delivery and the Evidence Ladder{{attrs[#blk-validation23]}}

:::success
**Learning Objectives**

- Compare DNA, RNA, and RNP delivery as trade-off bundles.
- Build a validation plan from reagent presence to a bounded causal interpretation.
:::

Delivery is part of the mechanism. DNA expression constructs require transcription and translation and may sustain exposure. Messenger RNA plus guide RNA is transient but still requires translation. A preassembled ribonucleoprotein (RNP) can act quickly and then decay, but uptake and cargo constraints remain. Viral, lipid, nanoparticle, and physical methods differ across tissues and cell types. No delivery strategy is universally best.

![Three-column comparison of DNA, RNA, and ribonucleoprotein delivery](https://alembic.orz.how/d/doc-0vzwjh1vbdpr)

*Figure 2.2. Delivery choices alter onset, duration, cargo, and stress. Original qualitative diagram by Yu Wang.*

**Visual alternative:** DNA constructs, RNA plus guide, and preassembled RNP appear as three columns. Each lists onset, duration, expression, cargo, and uptake considerations. A footer says the choice depends on cell type, tissue, toxicity, scale, and claim.

![NHGRI researcher using a pipette to load DNA into an electrophoresis gel](https://alembic.orz.how/d/doc-bfmos4nfl7qg)

*Figure 2.3. NHGRI researcher Milton English loading DNA into a gel. Maggie Bartlett/NHGRI; U.S. federal government work, public domain.*

Electrophoresis makes one part of laboratory validation visible: biological samples are physical, measurements require preparation, and every readout has resolution limits. A band of an expected size is useful evidence, but it does not reveal every sequence or every cell. Amplicon sequencing, longer-read methods, protein assays, functional measurements, and orthogonal approaches answer different questions.

![Scientist examining electrophoresis equipment in an NIH laboratory](https://alembic.orz.how/d/doc-b1s80yksezi8)

*Figure 2.4. Anastassia Tikhonova using electrophoresis equipment. NIH/NIAMS; U.S. federal government work, public domain.*

![Six-step ladder from delivery and target sequence to phenotype and a causal claim](https://alembic.orz.how/d/doc-vfqc3uude56x)

*Figure 2.5. An evidence ladder for genome-editing claims. Original diagram by Yu Wang.*

**Visual alternative:** Steps ascend from delivery to target-locus sequence, allele frequencies, molecular function, phenotype, and a bounded causal claim. A rail underneath lists controls, orthogonal assays, biological replicates, blinded analysis, and transparent uncertainty.

Validation should consider:

- **On-target identity:** What sequence changes occurred at the intended locus?
- **On-target heterogeneity:** Are there mixed alleles, larger changes, rearrangements, or mosaic populations?
- **Off-target activity:** Which plausible unintended loci changed, and what can the assay detect?
- **Molecular function:** Did RNA, protein, localization, or activity change as predicted?
- **Phenotype and toxicity:** Is the effect reproducible, appropriately sized, and separable from delivery stress?
- **Causality:** Do independent guides, rescue, matched controls, or orthogonal perturbations support the same explanation?

:::: tabs
::: tab Problem
A short-amplicon assay shows the intended small substitution and no nearby indels. Give two claims it supports and two it does not establish.
:::
::: tab Solution
It supports that the sampled amplicons contain the intended substitution and that nearby small indels were not detected within the assay's limits. It does not establish genome-wide absence of off-target changes, absence of larger on-target rearrangements, uniform editing across all cells, or functional rescue. Those require other assays.
:::
::::

**Self-check:**

- Why can shorter editor exposure be useful without guaranteeing safety?
- Which assay would you add after confirming the intended DNA sequence?
- How can delivery stress imitate a phenotype attributed to editing?

## 2.4 Applications, Boundaries, and Governance{{attrs[#blk-governance24]}}

:::success
**Learning Objectives**

- Separate technical feasibility from evidence of benefit and social acceptability.
- Compare governance questions across somatic, heritable, agricultural, and ecological settings.
:::

Genome editing is used in research models, functional screens, agriculture, biotechnology, and therapeutic development. The same molecular capability can sit inside very different decision structures. Editing a cultured cell for a mechanistic study, modifying a patient's somatic cells, changing an embryo in a heritable way, altering a crop, and releasing a gene drive into an ecosystem do not share one risk–benefit calculation.

| Context | Key distinction | Questions beyond “does editing work?” |
|---|---|---|
| Research model | Knowledge generation | Are controls adequate? Is the model relevant? |
| Somatic intervention | Change is intended for treated tissues | What is the expected benefit, monitoring plan, consent, and access? |
| Heritable intervention | Changes may pass to descendants | Who can consent, what alternatives exist, and how is long-term uncertainty governed? |
| Agriculture | Organism and food-system change | Who benefits, how are ecological and distributional effects assessed? |
| Gene drive | Biased inheritance can spread a trait | Can spread be contained or reversed, and who participates in the decision? |

Technical precision cannot answer questions about justice, disability perspectives, acceptable uncertainty, access, or intergenerational consent. Conversely, ethical debate should not rest on false technical premises. Responsible analysis keeps empirical and normative questions distinct while showing where they interact.

:::: tabs
::: tab Problem
Two proposals use the same editor with the same measured on-target accuracy. One edits a patient's blood stem cells outside the body; the other alters embryos so changes could be inherited. Why can the governance conclusions differ?
:::
::: tab Solution
The contexts differ in consent, reversibility, monitoring, who is exposed, and whether effects can pass to future generations. Equal molecular accuracy does not equal equal social risk or ethical acceptability. Technical evidence is necessary but not sufficient for either decision.
:::
::::

**Self-check:**

- Which questions are empirical, and which require value judgments?
- Why is “more precise” not a complete argument for deployment?
- What stakeholders could be affected by an ecological editing proposal?

## Synthesis

Genome editing joins programmable recognition to delivery, chemistry, cellular repair, sampling, and interpretation. Break-based editors generate multiple repair outcomes; base and prime editors alter but do not eliminate uncertainty. Delivery changes exposure and cell stress. Validation must climb from target sequence through allele distributions, function, phenotype, and causality. Applications should be evaluated in their own biological and social contexts rather than placed on a single ladder of technical progress.

## Asset and License Record for This Chapter

| Asset | Source | License | Attribution |
|---|---|---|---|
| `edit-to-outcome.svg` | Original for this package | CC BY-SA 4.0 | Yu Wang |
| `delivery-tradeoffs.svg` | Original for this package | CC BY-SA 4.0 | Yu Wang |
| `evidence-ladder.svg` | Original for this package | CC BY-SA 4.0 | Yu Wang |
| `loading-dna-gel.jpg` | [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Load_DNA_Gel.jpg) | Public domain | Maggie Bartlett/NHGRI; unchanged |
| `electrophoresis-equipment.jpg` | [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Electrophoresis_equipment.jpg) | Public domain | NIH/NIAMS; unchanged |

**Text adaptation:** Adapted and reorganized from [CRISPR gene editing](https://en.wikipedia.org/wiki/CRISPR_gene_editing), [Genome editing](https://en.wikipedia.org/wiki/Genome_editing), [DNA repair](https://en.wikipedia.org/wiki/DNA_repair), and [Cas9](https://en.wikipedia.org/wiki/Cas9) by Wikipedia contributors, CC BY-SA 4.0. Exact revisions are recorded in `metadata/SOURCE_RECORD.json`.
