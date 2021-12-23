# cisMetalysis

Metalysis and cis-Metalysis

Charles Blatti (blatti@illinois.edu) and Saurabh Sinha (sinhas@illinois.edu)

Our computational tool, called "Metalysis", provides a powerful framework for meta-analysis of annotation - condition associations across multiple conditions.

Its typical inputs are:

(1) sets of up- and down-regulated genes for each of several experimental conditions, and

(2) sets of genes defined by common biological annotations.

This tool reports annotations that are associated with dysregulated gene sets from a subset of conditions, along with a statistical assessment of the strength of such multi-condition ("meta") associations.


"cis-Metalysis" is an extension to Metalysis specifically designed to use motif target sets as annotation sets. It takes gene target predictions of the transcription factor motifs and then uses the Metalysis framework to identify meta associations between a motif and set of conditions. Because of the general consensus that condition-specific expression of a gene may be determine by combinations of transcription factors, cis-Metalysis also searches for motif combinations associated with expression.


For example, suppose motifs M_A and M_R correspond to an activator A and a repressor R respectively. Genes up-regulated in a condition in which MA and MR are expressed may be (partly) characterized by the motif combination "MA and not MR". In a different condition, repressor R may be absent, and the up-regulated gene set in that condition may be associated simply with the motif M_A.


In searching for a cis-regulatory influence common to multiple conditions, cis-Metalysis fixes the motifs involved while allowing the specific combination of those motifs to change from one condition to another. Put another way, cis- Metalysis is able to identify meta associations between a set of motifs and a set of conditions.

Source code: cisMetalysis-1.3.zip

Original publication: https://pubmed.ncbi.nlm.nih.gov/22691501/

