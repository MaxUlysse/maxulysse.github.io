<section data-background-image="{{ site.url }}/assets/img/background/Sarek-Park-01.jpg" data-background-opacity=0.5 >

# Sarek and rnafusion

## Detect variants and fusion genes

Maxime Garcia

<small>

[<i class="fab fa-twitter"></i> @gau](https://twitter.com/gau)

[<i class="fab fa-github"></i> @MaxUlysse](https://github.com/MaxUlysse)

[<i class="fa fa-globe-europe"></i> maxulysse.github.io](https://maxulysse.github.io/)

</small>

DNA Club

<small>
Science for Life Laboratory, Stockholm - 2020/09/16
</small>

---

[![Barntumörbanken]({{ site.url }}/assets/img/svg/barntumorbanken_logo.svg "Barntumörbanken")](https://ki.se/forskning/barntumorbanken) <!-- .element class="image-H10" -->

The Swedish Childhood Tumor Biobank (BTB)

[![KI]({{ site.url }}/assets/img/svg/ki_logo.svg "KI")](https://ki.se) <!-- .element class="image-H10" -->

Note:

* Working for The Swedish Childhood Tumor Biobank located at KI

---

[![SciLifeLab]({{ site.url }}/assets/img/svg/scilifelab_logo.svg "SciLifeLab")](https://scilifelab.se/) <!-- .element class="image-H10" -->

National centre for molecular biosciences with focus on health and environmental research

[![KI]({{ site.url }}/assets/img/svg/ki_logo.svg)](https://ki.se/) <!-- .element class="image-H75" --> | [![KTH]({{ site.url }}/assets/img/svg/kth_logo.svg)](https://www.kth.se/) <!-- .element class="image-H75" --> | [![SU]({{ site.url }}/assets/img/svg/su_logo.svg)](https://www.su.se/) <!-- .element class="image-H75" --> | [![UU]({{ site.url }}/assets/img/svg/uu_logo.svg)](https://www.uu.se/) <!-- .element class="image-H75" -->
:-:|:-:|:-:|:-:

Note:

* SciLifeLab is several infrastructures

===

[![NGI]({{ site.url }}/assets/img/svg/ngi_logo.svg "NGI")](https://ngisweden.scilifelab.se/) <!-- .element class="image-H10" -->

* State-of-the-art infrastructure
  * Sequencing (DNA, RNA ...)
* Guidelines and support
  * Sample collection, study design, protocol selection
  * Bioinformatics analysis

Note:

* NGI is a sequencing facility used by researchers all over Sweden

===

[![NBIS]({{ site.url }}/assets/img/svg/nbis_logo.svg "NBIS")](https://www.nbis.se/) <!-- .element class="image-H10" -->

* Swedish ELIXIR node
* Bioinformatics support for Swedish researchers

---

## Reproducibility is central

[![Figure 1]({{ site.url }}/assets/img/slides/gigascience_giy077_fig1.jpg "figure 1")](https://academic.oup.com/view-large/figure/118918033/giy077fig1.jpg) <!-- .element class="image-50" -->

[<i class="ai ai-doi"></i> 10.1093/gigascience/giy077](https://doi.org/10.1093/gigascience/giy077)

Note:

* For me, as a bioinformatician it is a crucial matter

---

## What is Sarek

<section data-background-image="{{ site.url }}/assets/img/background/Sarek-beer.jpg" data-background-opacity=0.5 >

<div class="fragment fade-in" data-fragment-index="2">

A [National Park](https://www.sverigesnationalparker.se/en/choose-park---list/sarek-national-park/) in Northern Sweden.

<small>

* Long, deep, narrow valleys and wild, turbulent water
* A tortuous delta landscape
* Completely lacking in comfortable accommodations
* One of Sweden’s most inaccessible national parks
* There are no roads leading up to the national park

</small>

</div>

---

<section data-background-image="{{ site.url }}/assets/img/background/Sarek-Park-02.jpg">

---

<section data-background-image="{{ site.url }}/assets/img/background/Sarek-Park-02.jpg" data-background-opacity=0.5 >

* [Ruotes](https://github.com/SciLifeLab/Sarek/releases/tag/2.1.0)
* [Skårki](https://github.com/SciLifeLab/Sarek/releases/tag/2.2.0)
* [Äpar](https://github.com/SciLifeLab/Sarek/releases/tag/2.3)
* [Ålkatj](https://github.com/nf-core/sarek/releases/tag/2.5)
  * [Årjep-Ålkatjjekna](https://github.com/nf-core/sarek/releases/tag/2.5.1)
  * [Jåkkåtjkaskajekna](https://github.com/nf-core/sarek/releases/tag/2.5.2)
* [Piellorieppe](https://github.com/nf-core/sarek/releases/tag/2.6)
  * [Gådokgaskatjåhkkå](https://github.com/nf-core/sarek/releases/tag/2.6.1)

---

[![Sarek]({{ site.url }}/assets/img/svg/nf-core_sarek_logo.svg "Sarek")](https://nf-co.re/sarek) <!-- .element class="image-H10" -->

<div class="fragment fade-in" data-fragment-index="2">

* Open-Source Nextflow Pipeline
* Started at NGI
* In collaboration with NBIS
* Support from BTB
* In collaboration with QBiC (Tübingen)

</div>

===

[![Nextflow]({{ site.url }}/assets/img/slides/nextflow.png "Nextflow")](https://www.nextflow.io/) <!-- .element class="image-50" -->

* Workflow manager
  * Data driven language
  * Portable
    * executable on multiple platforms
  * Shareable and reproducible
    * with containers or virtual environments

Note:

* Early adopters of Nextflow for its portability, shareability and of course reproducibility

---

## Multiple flavors

![Sarek]({{ site.url }}/assets/img/svg/sarek_logo.svg "Sarek") <!-- .element class="image-10" -->

<div class="fragment fade-in" data-fragment-index="2">

![Sarek]({{ site.url }}/assets/img/svg/sarek-germline.svg "Sarek") <!-- .element class="image-10" --> | ![Sarek]({{ site.url }}/assets/img/svg/sarek-somatic.svg "Sarek") <!-- .element class="image-10" -->
:-:|:-:

</div>

===

## WES and Targeted Sequencing

![]({{ site.url }}/assets/img/svg/appleseq.svg "WGS, WES, and Targeted") <!-- .element class="image-25" -->

===

## Reference genomes

[AWS iGenomes](https://registry.opendata.aws/aws-igenomes/)

* GRCh37
* GRCh38
* GRCm38

---

## Preprocessing

[![GATKBP]({{ site.url }}/assets/img/svg/gatk-bp_logo.svg "GATK Best Practices")](https://software.broadinstitute.org/gatk/best-practices/) <!-- .element class="image-H25" -->

Based on GATK Best Practices (GATK 4.1.7.0)

<div class="fragment fade-in" data-fragment-index="2">

* Reads mapped to reference genome with `bwa`
* Duplicates marked with `picard MarkDuplicates`
* Recalibrate with `GATK BaseRecalibrator`

</div>

===

## Germline Variant Calling

* SNVs and small indels
  * HaplotypeCaller
  * Strelka2
  * Freebayes
  * mpileup
* Structural variants
  * Manta
  * TIDDIT

===

## Somatic Variant Calling

* SNVs and small indels
  * Mutect2
  * Strelka2
  * Freebayes
* Structural variants
  * Manta
* Sample heterogeneity, ploidy and CNVs
  * ASCAT
  * Control-FREEC
* Microsatellite instability
  * MSIsensor

===

## Annotation

* VEP and SnpEff
  * <i class="fas fa-database"></i> ClinVar, COSMIC, dbSNP, GENCODE, gnomAD, polyphen, sift, etc.

===

## Reports

[![MultiQC]({{ site.url }}/assets/img/svg/multiqc_logo.svg "MultiQC")](https://multiqc.info/) <!-- .element class="image-H25" -->

---

## Workflow

[![Sarek Workflow]({{ site.url }}/assets/img/svg/sarek_workflow_2.6.1.svg "Sarek Workflow 2.6.1")](https://github.com/nf-core/sarek/releases/tag/2.6.1) <!-- .element class="image-25" -->

---

## Prioritization

* First step towards clinical use
* Rank scores are computed for all variants
  * COSMIC, ClinVar, SweFreq and MSK-IMPACT (cancerhotspots.org)
* Findings are ranked
  * Well known, high-impact variants
  * Variants in known cancer-related genes
  * Remaining variants

---

## What is coming soon

* <i class="far fa-check-square"></i> `@sarek-team` to mention the core sarek developers on Slack
* <i class="far fa-check-square"></i> `@nf-core/sarek` to mention the core sarek developers on GitHub
* <i class="far fa-check-square"></i> BWA-MEM2 ([dev](https://github.com/nf-core/sarek/tree/dev))
* <i class="far fa-check-square"></i> Bug-fixes ([dev](https://github.com/nf-core/sarek/tree/dev))
* <i class="far fa-square"></i> DSL 2 ([dsl2](https://github.com/nf-core/sarek/tree/dsl2)) with [@ggabernet](https://github.com/ggabernet) and [@FriederikeHanssen](https://github.com/FriederikeHanssen)

===

## What is coming next

* Validation tests
* More tools
* Sub-workflows for specific usage
  * Improved cloud usage
  * Improved usage for non-model organism
* More downstream processing of the final vcf files
* Easier connection to [Scout](https://www.clinicalgenomics.se/scout/)

Note:

* Scout is a tool developed by SciLifeLab Clinical Genomics to analyse VCF files

---

## Sarek usage

* Within BTB
  * Tumor/normal pairs

* In production at NGI
  * All normal samples
  * Tumor/normal pairs

* The whole SweGen dataset
  * 1 000 normal samples (GRCh38)

* Genome Medicine Sweden

Note:

* GMS is an initiative to implement Precision Medicine at a national level

---

## Publication in F1000Research

Sarek: A portable workflow for whole-genome sequencing</br>
analysis of germline and somatic variants</br>
[version 2; peer review: 2 approved]

<small>

Maxime Garcia, Szilveszter Juhos, Malin Larsson, Pall I. Olason, Marcel Martin,</br>
Jesper Eisfeldt, Sebastian DiLorenzo, Johanna Sandgren, Teresita Díaz De Ståhl,</br>
Philip Ewels, Valtteri Wirta, Monica Nistér, Max Käller, Björn Nystedt

</small>

[<i class="ai ai-doi"></i> doi.org/10.12688/f1000research.16665.2](https://doi.org/10.12688/f1000research.16665.2)

---

[![rnafusion]({{ site.url }}/assets/img/svg/nf-core_rnafusion_logo.svg "rnafusion")](https://nf-co.re/rnafusion) <!-- .element class="image-H10" -->

<div class="fragment fade-in" data-fragment-index="2">

* Open-Source Nextflow Pipeline
  * Part of nf-core
  * Started at NGI
  * Support from BTB

</div>

<div class="fragment fade-in" data-fragment-index="3">

<small>

Project initiated by [Rickard Hammarén](https://github.com/Hammarn),
fully matured under [Martin Proks](https://github.com/matq007),
shamelessly taken over by me.

</small>

</div>

===

Run and gather outputs from

* Arriba
* EricScript
* FusionCatcher
* Pizzly
* Squid
* STAR-Fusion

<div class="fragment fade-in" data-fragment-index="2">

Generate a nice final report

</div>

---

## Get involved

* Our code is hosted on Github
  * [<i class="fab fa-github"></i> github.com/nf-core](https://github.com/nf-core)
  * [<i class="fab fa-github"></i> github.com/nf-core/sarek](https://github.com/nf-core/sarek)
  * [<i class="fab fa-github"></i> github.com/nf-core/rnafusion](https://github.com/nf-core/rnafusion)
* We have Slack
  * [<i class="fab fa-slack"></i> nfcore.slack.com](https://nfcore.slack.com/)
  * [<i class="fab fa-slack"></i> #sarek](https://nfcore.slack.com/channels/sarek)
  * [<i class="fab fa-slack"></i> #rnafusion](https://nfcore.slack.com/channels/rnafusion)

---

<div class="r-stack">
  <img src="/assets/img/svg/acknowledgments_2020.svg" title="Acknowledgements" alt="Acknowledgements" class="image-75 fragment fade-out" data-fragment-index="0"/>
  <img src="/assets/img/svg/institutes_2020.svg" title="Acknowledgements" alt="Acknowledgements" class="image-75 fragment fade-in-then-out" data-fragment-index="0"/>
  <img src="/assets/img/slides/nf-core_contributors_jobim.png" title="Acknowledgements" alt="Acknowledgements" class="image-75 fragment fade-in-then-out" data-fragment-index="1"/>
  <img src="/assets/img/slides/nf-core_sarek_contributors_2.6.1.png" title="Acknowledgements" alt="Acknowledgements" class="image-75 fragment fade-in-then-out" data-fragment-index="2"/>
  <img src="/assets/img/slides/nf-core_rnafusion_contributors_1.2.0.png" title="Acknowledgements" alt="Acknowledgements" class="image-75 fragment fade-in-then-out" data-fragment-index="3"/>
</div>

---

<section data-background-image="{{ site.url }}/assets/img/background/Stockholm-by-night.jpg" data-background-opacity=0.5 >

## Any questions

* [<i class="fa fa-globe-europe"></i> nf-co.re](https://nf-co.re/)
* [<i class="fab fa-github"></i> nf-co.re/sarek](https://nf-co.re/sarek)
* [<i class="fab fa-slack"></i> #sarek](https://nfcore.slack.com/channels/sarek)
* [<i class="fab fa-github"></i> nf-co.re/rnafusion](https://nf-co.re/rnafusion)
* [<i class="fab fa-slack"></i> #rnafusion](https://nfcore.slack.com/channels/rnafusion)
