# EF-Tu protein variance


Yang *et al.* submitted the manuscript entitled __Engineered Agrobacterium mitigates plant immunity detection and improves T-DNA transfer__. This repo stores all EF-Tu sequence data in this study.

## Folder description

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
- Serratia and 
- Xanthomonas 


### Preprocessed

Fasta files above were preprocessed by filtering accessions that contains explicit bacterial genus name and species name, and full-length EF-Tu protein. The filtered sequences from each genus were combined into one fasta file that contain 32,889 protein sequences.


### Aligned

The cleaned EF-Tu sequence above aligned with multiple sequence alignment tool MAFFT (https://mafft.cbrc.jp/alignment/server/index.html). Output was download and used to subsequent analysis of amino acid variation. 