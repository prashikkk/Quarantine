# Quarantine
## File Formats used in Bioinformatics 

### 1. FASTA : 

FASTA format is a text-based format for representing either nucleotide sequences or peptide sequences, in which base pairs or amino acids are represented using single-letter codes. A sequence in FASTA format begins with a single-line description, followed by lines of sequence data. The format also allows for sequence names and comments to precede the sequences FASTA takes a given nucleotide or amino acid sequence and searches a corresponding sequence database by using local sequence alignment to find matches of similar database sequences. The FASTA program follows a largely heuristic method which contributes to the high speed of its execution.

<pre>
>sp|P02144|MYG_HUMAN Myoglobin OS=Homo sapiens OX=9606 GN=MB PE=1 SV=2
MGLSDGEWQLVLNVWGKVEADIPGHGQEVLIRLFKGHPETLEKFDKFKHLKSEDEMKASE
DLKKHGATVLTALGGILKKKGHHEAEIKPLAQSHATKHKIPVKYLEFISECIIQVLQSKH
PGDFGADAQGAMNKALELFRKDMASNYKELGFQG
<\pre>

### 2.  FASTQ :

FASTQ format is a text-based format for storing both a biological sequence (usually nucleotide sequence) and its corresponding quality scores. It is a text file that contains the sequence data from the clusters that pass filter on a flow cell.
Each record in a FastQ file consists of four lines:

1.Sequence identifier.
2.Nucleotide sequence.
3.Quality score identifier line (always a single “+” (plus) sign)
4.Quality scores.

In FASTQ files, quality scores are encoded into a compact form, which uses only 1 byte per quality value.

![FASTQ](https://www.researchgate.net/profile/Morteza-Hosseini-6/publication/309134977/figure/fig2/AS:417452136648711@1476539753452/A-sample-of-the-FASTQ-file.png)

### 3. GFF :

Generic Feature Format (GFF) is a biological sequence file format for representing features and annotations on sequences. It is a tab delimited format, making it accessible to biologists and editable in text editors and spreadsheet programs. It is also well defined and can be parsed via automated programs. In bioinformatics, the general feature format (gene-finding format, generic feature format, GFF) is a file format used for describing genes and other features of DNA, RNA and protein sequences. 

![GFF](http://learn.gencore.bio.nyu.edu/wp-content/uploads/2018/01/Screen-Shot-2018-01-07-at-10.10.20-PM-1024x590.png)

### 4. GTF :

The Gene transfer format (GTF) is a file format used to hold information about gene structure. It is a tab-delimited text format based on the general feature format (GFF), but contains some additional conventions specific to gene information. Given a sequence and a GTF file, one can check that the format is correct. This significantly reduces problems with the interchange of data between groups.

![GTF](https://upload.wikimedia.org/wikipedia/commons/2/22/GTF_file_example.jpg)

### 5. VCF :

The Variant Call Format (VCF) specifies the format of a text file used in bioinformatics for storing gene sequence variations. VCF is a text file format (most likely stored in a compressed manner). It contains meta-information lines, a header line, and then data lines each containing information about a position in the genome. The format also has the ability to contain genotype information on samples for each position. Since VCF files store contact information, they're often seen as the export/import format of some address book programs. This makes it easy to share one or more contacts, use the same contacts in different email programs or services, or back up your address book to a file.

![VCF](https://upload.wikimedia.org/wikipedia/commons/3/39/Binary_BCF_versus_VCF_format.png)

### 6. SAM : 

SAM stands for Sequence Alignment Map format. It is a TAB-delimited text format consisting of a header section, which is optional, and an alignment section. If present, the header must be prior to the alignments. The SAM Format is a text format for storing sequence data in a series of tab delimited ASCII columns. 

![SAM](https://miro.medium.com/max/1838/0*CePvh8XpBcbC1HjZ.png)

### 7. BAM : 

A Binary Alignment Map (BAM) file format is the compressed binary version of a SAM file that is used to represent aligned sequences up to 128 Mb. A BAM file contains two sections viz. Header and Alignment. Header—Contains information about the entire file, such as sample name, sample length, and alignment method. Alignments in the alignments section are associated with specific information in the header section. Alignments—Contains read name, read sequence, read quality, alignment information, and custom tags. 

![BAM](https://miro.medium.com/max/988/0*CePvh8XpBcbC1HjZ.png)


Submitted by -
@prashikkk
