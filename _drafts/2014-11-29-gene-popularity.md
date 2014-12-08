---
layout: post
title:  "The 20 Most Studied Genes"
tags: genbank bioinformatics
---
The Nation Center for Biotechnology Information (NCBI) maintains an enormous
amount of biological data and provides it all to the public for no cost as a
collection of databases. One of the most popular is [GenBank](http://www.ncbi.nlm.nih.gov/genbank/), which contains
information about annotated genes. Consider the [gene
p53](http://www.ncbi.nlm.nih.gov/gene/7157), which encodes a tumor
suppressor protein, the absence of which allows many cancers to proliferate. By
looking at its entry in GenBank, we can immediately find out its full name
(tumor protein p53), which organism this entry corresponds to (Human), aliases
(BCC7, LFS1, TRP53), a short description and a whole host of other technical
information. 

Among the information provided with each entry is a section which contains a
list of papers which have referenced this gene. In a sense, each reference 
is a paper which has contributed some bit of knowledge
about the function of this piece of DNA (or RNA).  This got me
wondering, which are the most studied genes? Which genes have
made an appearance in the most published papers?

To answer, this, I [downloaded the
table](ftp://ftp.ncbi.nlm.nih.gov/gene/DATA/) which contains the reference
information from GenBank, and performed some rudimentary analysis, and generated the
following table of the top 20 most popular genes, as measured by the number of
times they have been cited:

<div class='chart'>
<div id="gene-counts-chart"></div>
<link rel="stylesheet" href="/css/d3_bar_chart.css">
<script src="http://d3js.org/d3.v3.min.js"></script>
<script src="js/d3_bar_chart.js"></script>
 <script>renderGeneCountsChart();</script>
 </div>

 The genese on the list can be broadly placed into 6 categories:

 1. **Cancer related** - All of the genes with 'tumor' or
 'cancer' in their name, along with those containing 'growth factor' are
 associated with various cancer and are involved in either helping cells
 proliferate ([oncogenes](http://en.wikipedia.org/wiki/Oncogene)) or preventing them from becoming cancerous ([tumor suppressor genes](http://en.wikipedia.org/wiki/Tumor_suppressor_gene)).

 2. **Immune system related** - Interleukins, ['nuclear factor
 kappa-light-chain-enhancer of activated B
 cells'](http://en.wikipedia.org/wiki/NF-%CE%BAB) (also known as NF-κB) and
 [major histocompatibility complex
 (MHC)](http://en.wikipedia.org/wiki/Major_histocompatibility_complex) are all
 associated with immune responses such as recognizing pathogens and mounting a
 response against them.

 3. **HIV related** - [gp160 envelope
 glycoprotein](http://en.wikipedia.org/wiki/Env_%28gene%29) is one of the
 proteins on the surface retroviruses which allow it to attach to and enter
 various cells. Needless to say, it is extremely important in finding
 treatments and vaccines for such viruses.

 4. **Other disease** - [Apolipoprotein
 E](http://en.wikipedia.org/wiki/Apolipoprotein_E) is involved in heart disease
 and Alzheimer's disease, while [Methylenetetrahydrofolate reductase
 (MTHFR)](http://en.wikipedia.org/wiki/Methylenetetrahydrofolate_reductase) has
 associated with susceptibility to a variety of disorders including Alzheimer's
 colon cancer and others.

 6. **Regulatory** - [Ubiquitin](http://en.wikipedia.org/wiki/Ubiquitin) is a
 protein involved in the translocation and degradation (among other processes)
 of other proteins. [Angiotensin-converting enzyme
 (ACE)](http://en.wikipedia.org/wiki/Angiotensin-converting_enzyme) is a
 regulatory enzyme which is involved in the control of blood pressure.
[Estrogen receptor 1 (ESR1)](http://en.wikipedia.org/wiki/Estrogen_receptor_alpha).
is a transcription factor which responds to the hormone estrogen, leading
to a variety of downstream effcts.

 7. **Other** - The only remaining gene on the list, [w
 (white)](http://en.wikipedia.org/wiki/White_%28mutation%29), is popular
 largely due to its historical cachet. It was the first mutation to be
 discovered which did not display typical Mendelian inheritance due to its
 location on a sex-chromosome in *D. melanogaster*. Gene trap [ROSA 26
 (gt(ROSA)26Sor)](http://en.wikipedia.org/wiki/ROSA26) is simply convenient
 place to insert genes for study in a mouse model. 

 Immediately evident is the overrepresentation of disease-related genes.
 15 of the 20 genes are heavily involved in some human disease.  The
 remaining entries are either regulatory (UBC, ACE and ESR1), historic (w) or
 just simply useful (Gt(ROSA)26Sor). The majority come from human, followed by
 mouse (expressing genes also found in humans, Tnf and Trp53), and finally HIV
 and Drosophila. This is something of a reflection of where our interests and
 funding lie. The two most studied genes are involved in cancer, research in
 which is both well-funded and heavily reliant on genetic analysis.  Four on
 the list are associated with the immune system (IL6, IL10, NFKB1, and
 HLA-DRB1), two (APOE and ACE) are associated with heart disease and one with
 HIV. We focus the majority of our attention on the things which are likely to
 kill us.

 Conspicuously absent from the list are any genes from plants or genes involved
 in metabolism. Important pathways such as differentiation, DNA replication and
 protein synthesis are all absent. That's not to say that they are not studied,
 it's just that they recieve less attention than processes involved in our
 demise. Then again, the age of molecular genetics has only begun in the last
 century or so. Perhaps our interests will shift in the future as we find cures
 and treatments for existing maladies and start having to deal with others such
 as a a changing climate, energy crises and an aging population. Biology may
 hold partial solutions to these problems and the proportional amount of effort
 we put into finding processes to remove carbon dioxide from the
 air, to produce fuels from biomatter or to limit or reverse aging may grow to
 eclipse that put into research in the current top-20 genes.