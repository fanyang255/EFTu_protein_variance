# EF-Tu protein variance


Yang *et al.* submitted the manuscript entitled __Engineered ***Agrobacterium*** mitigates plant immunity detection and improves T-DNA transfer__. This repo stores all EF-Tu sequence data in this study.

## Folder descriptions

### Raw

EF-Tu protein sequences were fetched from NCBI with Python BioEntrez query that search for full-length EF-Tu proteins of 21 bacterial genera. It includes:
- Acidovorax
- Agrobacterium
- Azospirillum
- Bacillus
- Burkholderia
- Clavibacter
- Dickeya
- Enterobacter
- Erwinia
- Escherichia
- Komagataeibacter
- Paenibacillus
- Pantoea
- Paraburkholderia
- Pectobacterium
- Phytoplasma
- Pseudomonas
- Ralstonia
- Rhizobium
- Serratia
- Xanthomonas 


### Preprocessed

Fasta files above were preprocessed by filtering accessions that contains explicit bacterial genus name and species name, and full-length EF-Tu protein. The filtered sequences from each genus were combined into one fasta file that contains 32,889 protein sequences.


### Aligned

The cleaned EF-Tu sequences above were aligned with multiple sequence alignment tool MAFFT (https://mafft.cbrc.jp/alignment/server/index.html). The output file was download and used to determine EF-Tu amino acid variance at each position. 