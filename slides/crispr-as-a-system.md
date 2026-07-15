<!-- deck
title: Chapter 1: CRISPR as a Biological System
theme: sage
ratio: 16:9
author: Yu Wang
footer: Coursewerk demonstration · Not for actual teaching · CC BY-SA 4.0
-->

<!-- slide template=title v=5 -->
# CRISPR as a Biological System
## Memory, targeting, and Cas9

**AI-generated Coursewerk demonstration—not intended for actual teaching**

<!-- slide 2col -->
## Learning objectives
<!-- @left -->
- {{sp[info] 1.1}} Decode a CRISPR locus
- {{sp[info] 1.2}} Trace guide biogenesis
- {{sp[info] 1.3}} Explain PAM-dependent targeting
<!-- @right -->
- {{sp[info] 1.4}} Compare active Cas9, nickase, and dCas9
- Preserve the distinction between Cas9 and CRISPR diversity

:::success
**Repeated question:** Where is the information, and what molecular step uses it?
:::

<!-- slide template=outline v=5 -->
# Chapter route
- Encounter → spacer record
- Array → guide RNA
- PAM + pairing → checkpoint progression
- Recognition separated from catalytic action

<!-- slide -->
## CRISPR is an information-flow system
{{mermaid
flowchart LR
  A[invader] --> B[spacer acquisition]
  B --> C[array]
  C --> D[guide RNA]
  D --> E[Cas effector]
  E --> F[target interrogation]
  F --> G[interference]
}}

**Visual description:** Invader-derived sequence enters an array, becomes a guide, joins a Cas effector, and supports target interrogation and interference.

<!-- slide template=section v=2 -->
# 1.1 Molecular memory
## A partial record of prior encounters

<!-- slide main-side 3/2 -->
## Start with the biological pressure
<!-- @main -->
![Electron micrograph of bacteriophages attached to a bacterial cell wall](https://alembic.orz.how/d/doc-u0lmzufzh892 =500x)
<!-- @side -->
- phages inject nucleic acid
- microbes face repeated invasion
- CRISPR is one defense among many
- selection acts on both host and phage

*Professor Graham Beards; CC BY-SA 3.0.*

<!-- slide main-side 3/2 -->
## Read the array
<!-- @main -->
![Phage fragment becoming a spacer near the array leader](https://alembic.orz.how/d/doc-g9rsmfe767h8 =650x)
<!-- @side -->
- repeats recur
- spacers vary
- leader gives orientation
- new does not mean complete

<!-- slide 2col -->
## Spacer ≠ protospacer
<!-- @left -->
{{sp[success] Host array}}

**Spacer:** stored sequence between repeats
<!-- @right -->
{{sp[warning] Invader}}

**Protospacer:** corresponding source sequence

**Adjacent PAM:** context, not guide content

<!-- slide step -->
## Adaptation as a cautious inference
1. A foreign fragment is selected.
2. Cas1–Cas2 machinery can integrate it.
3. A repeat is duplicated around the new spacer.
4. Arrays can also lose and rearrange spacers.

==Sequence order is evidence—not a perfect infection diary.==

<!-- slide template=section v=3 -->
# 1.2 From array to guide
## Stored sequence becomes usable RNA

<!-- slide -->
## Type II guide biogenesis
{{mermaid
flowchart LR
  A[array DNA] --> B[pre-crRNA]
  C[tracrRNA] --> D[paired intermediate]
  B --> D
  D --> E[mature crRNA + tracrRNA]
  E --> F[Cas9 complex]
  G[engineered fusion] --> H[sgRNA]
  H --> F
}}

**Visual description:** Array transcription and tracrRNA-assisted processing produce a natural two-RNA guide; engineering fuses guide functions into sgRNA.

<!-- slide 2col -->
## What engineering changes
<!-- @left -->
{{sp[success] Retained}}

- RNA scaffold–Cas9 assembly
- guide-directed pairing
- PAM dependence
<!-- @right -->
{{sp[info] Simplified}}

- crRNA + tracrRNA → sgRNA
- new target → new guide segment
- same protein can be redirected

<!-- slide template=section v=4 -->
# 1.3 Target checkpoints
## Complementarity is necessary—but not the whole rule

<!-- slide main-side 3/2 -->
## PAM beside the target
<!-- @main -->
![Cas9 beside double-stranded DNA, a guide-pairing region, and adjacent PAM](https://alembic.orz.how/d/doc-xe09bqbh95sh =660x)
<!-- @side -->
- SpCas9 example: often `5′-NGG-3′`
- PAM is adjacent to pairing region
- different effectors use other contexts
- no universal CRISPR PAM

<!-- slide main-side 3/2 -->
## Recognition progresses
<!-- @main -->
![Four checkpoints from PAM sampling through guide pairing to nuclease activation](https://alembic.orz.how/d/doc-ug659aasmvvm =660x)
<!-- @side -->
1. sample PAM
2. open DNA locally
3. extend RNA–DNA pairing
4. activate nuclease domains

<!-- slide 2col -->
## Why mismatch rules are conditional
<!-- @left -->
**Molecular variables**

- mismatch position and identity
- guide and nuclease variant
- number and spacing
<!-- @right -->
**Cellular variables**

- chromatin accessibility
- editor concentration and duration
- assay sensitivity

:::warning
Prediction must be tested; no string rule guarantees activity.
:::

<!-- slide template=section v=5 -->
# 1.4 Separate targeting from action
## One recognition platform, several outputs

<!-- slide 3col -->
## Cas9 variants
<!-- @left -->
**Active Cas9**

usually cuts both DNA strands
<!-- @mid -->
**Nickase**

one catalytic activity disabled
<!-- @right -->
**dCas9**

binds without ordinary cleavage

<!-- slide quad -->
## CRISPR is larger than Cas9
<!-- @tl -->
**Cas9**

Type II DNA targeting
<!-- @tr -->
**Cas12**

different DNA-effector properties
<!-- @bl -->
**Cas13**

RNA-targeting systems
<!-- @br -->
**Fusions**

regulation, base editing, prime editing

<!-- slide step -->
## Reasoning check
**Observation:** dCas9 at a promoter lowers transcription, but DNA sequence is unchanged.

1. dCas9 retains guide-directed binding.
2. It lacks ordinary nuclease activity.
3. Binding can obstruct or recruit regulators.
4. ==Expression change without sequence editing is coherent.==

<!-- slide template=closing v=2 -->
# Take-home model
- CRISPR arrays store partial sequence records.
- Guide biogenesis connects stored sequence to effectors.
- PAM, pairing, and conformation create checkpoints.
- Recognition and catalytic action are modular.
- Cas9 is an example, not the whole field.

**Next:** delivery, cellular repair, outcome distributions, and evidence.

<!-- slide -->
## Sources and media
Text adapted and reorganized from [CRISPR](https://en.wikipedia.org/wiki/CRISPR), [Cas9](https://en.wikipedia.org/wiki/Cas9), and [CRISPR gene editing](https://en.wikipedia.org/wiki/CRISPR_gene_editing) by Wikipedia contributors, [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Exact revisions: `metadata/SOURCE_RECORD.json`.

Phage micrograph: Professor Graham Beards, [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Phage.jpg), CC BY-SA 3.0. Original SVG diagrams: Yu Wang, CC BY-SA 4.0.

**Demo only—not intended for actual teaching.**
