# Quarantine
## File Formats used in Bioinformatics 

### 1. FASTA : 

FASTA format is a text-based format for representing either nucleotide sequences or peptide sequences, in which base pairs or amino acids are represented using single-letter codes. A sequence in FASTA format begins with a single-line description, followed by lines of sequence data. The format also allows for sequence names and comments to precede the sequences FASTA takes a given nucleotide or amino acid sequence and searches a corresponding sequence database by using local sequence alignment to find matches of similar database sequences. The FASTA program follows a largely heuristic method which contributes to the high speed of its execution.

### 2.  FASTQ

FASTQ format is a text-based format for storing both a biological sequence (usually nucleotide sequence) and its corresponding quality scores. It is a text file that contains the sequence data from the clusters that pass filter on a flow cell.
Each record in a FastQ file consists of four lines:
a)Sequence identifier.
b)Nucleotide sequence.
c)Quality score identifier line (always a single “+” (plus) sign)
d)Quality scores.
In FASTQ files, quality scores are encoded into a compact form, which uses only 1 byte per quality value.

