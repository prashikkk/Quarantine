# Quarantine
## File Formats used in Bioinformatics 

### 1. FASTA : 

FASTA format is a text-based format for representing either nucleotide sequences or peptide sequences, in which base pairs or amino acids are represented using single-letter codes. A sequence in FASTA format begins with a single-line description, followed by lines of sequence data. The format also allows for sequence names and comments to precede the sequences FASTA takes a given nucleotide or amino acid sequence and searches a corresponding sequence database by using local sequence alignment to find matches of similar database sequences. The FASTA program follows a largely heuristic method which contributes to the high speed of its execution.

<pre>
>sp|P02144|MYG_HUMAN Myoglobin OS=Homo sapiens OX=9606 GN=MB PE=1 SV=2
MGLSDGEWQLVLNVWGKVEADIPGHGQEVLIRLFKGHPETLEKFDKFKHLKSEDEMKASE
DLKKHGATVLTALGGILKKKGHHEAEIKPLAQSHATKHKIPVKYLEFISECIIQVLQSKH
PGDFGADAQGAMNKALELFRKDMASNYKELGFQG
</pre>

### 2.  FASTQ :

FASTQ format is a text-based format for storing both a biological sequence (usually nucleotide sequence) and its corresponding quality scores. It is a text file that contains the sequence data from the clusters that pass filter on a flow cell.
Each record in a FastQ file consists of four lines:

1.Sequence identifier.
2.Nucleotide sequence.
3.Quality score identifier line (always a single “+” (plus) sign)
4.Quality scores.

In FASTQ files, quality scores are encoded into a compact form, which uses only 1 byte per quality value.

<pre>
@SEQ_ID
GATTTGGGGTTCAAAGCAGTATCGATCAAATAGTAAATCCATTTGTTCAACTCACAGTTT
+
!''*((((***+))%%%++)(%%%%).1***-+*''))**55CCF>>>>>>CCCCCCC65
</pre>

### 3. GFF :

Generic Feature Format (GFF) is a biological sequence file format for representing features and annotations on sequences. It is a tab delimited format, making it accessible to biologists and editable in text editors and spreadsheet programs. It is also well defined and can be parsed via automated programs. In bioinformatics, the general feature format (gene-finding format, generic feature format, GFF) is a file format used for describing genes and other features of DNA, RNA and protein sequences. 

<pre>
##gff-version 3
##sequence-region P02144 1 154
P02144	UniProtKB	Initiator methionine	1	1	.	.	.	Note=Removed;Ontology_term=ECO:0000269,ECO:0000269;evidence=ECO:0000269|PubMed:5285572,ECO:0000269|PubMed:7895732;Dbxref=PMID:5285572,PMID:7895732	
P02144	UniProtKB	Chain	2	154	.	.	.	ID=PRO_0000053303;Note=Myoglobin	
P02144	UniProtKB	Metal binding	65	65	.	.	.	Note=Iron (heme distal ligand);Ontology_term=ECO:0000269;evidence=ECO:0000269|PubMed:2342104;Dbxref=PMID:2342104	
P02144	UniProtKB	Metal binding	94	94	.	.	.	Note=Iron (heme proximal ligand);Ontology_term=ECO:0000269,ECO:0007744;evidence=ECO:0000269|PubMed:2342104,ECO:0007744|PDB:3RGK;Dbxref=PMID:2342104	
P02144	UniProtKB	Modified residue	4	4	.	.	.	Note=Phosphoserine;Ontology_term=ECO:0000250;evidence=ECO:0000250|UniProtKB:Q9QZ76	
P02144	UniProtKB	Modified residue	68	68	.	.	.	Note=Phosphothreonine;Ontology_term=ECO:0000250;evidence=ECO:0000250|UniProtKB:P04247	
P02144	UniProtKB	Natural variant	55	55	.	.	.	ID=VAR_003180;Note=E->K;Ontology_term=ECO:0000269;evidence=ECO:0000269|PubMed:5805522;Dbxref=dbSNP:rs145465287,PMID:5805522	
P02144	UniProtKB	Natural variant	134	134	.	.	.	ID=VAR_003181;Note=K->N;Ontology_term=ECO:0000269;evidence=ECO:0000269|PubMed:5555226;Dbxref=dbSNP:rs766095327,PMID:5555226	
P02144	UniProtKB	Natural variant	140	140	.	.	.	ID=VAR_003182;Note=R->Q;Ontology_term=ECO:0000269;evidence=ECO:0000269|PubMed:5540041;Dbxref=dbSNP:rs142225854,PMID:5540041	
P02144	UniProtKB	Natural variant	140	140	.	.	.	ID=VAR_003183;Note=R->W;Ontology_term=ECO:0000269;evidence=ECO:0000269|PubMed:5555219;Dbxref=dbSNP:rs767663245,PMID:5555219	
P02144	UniProtKB	Sequence conflict	106	106	.	.	.	Note=E->Q;Ontology_term=ECO:0000305;evidence=ECO:0000305	
P02144	UniProtKB	Sequence conflict	129	129	.	.	.	Note=Q->E;Ontology_term=ECO:0000305;evidence=ECO:0000305	
P02144	UniProtKB	Helix	5	18	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	19	21	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	22	36	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	38	43	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	45	47	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	53	57	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	60	77	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Turn	78	81	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	84	96	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	102	119	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Turn	121	123	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
P02144	UniProtKB	Helix	126	149	.	.	.	Ontology_term=ECO:0007829;evidence=ECO:0007829|PDB:3RGK	
</pre>

### 4. GTF :

The Gene transfer format (GTF) is a file format used to hold information about gene structure. It is a tab-delimited text format based on the general feature format (GFF), but contains some additional conventions specific to gene information. Given a sequence and a GTF file, one can check that the format is correct. This significantly reduces problems with the interchange of data between groups.

<pre>
chr1 HAVANA gene 11869 14409 . + . gene_id "ENSG00000223972.5"; gene_type "transcribed_unprocessed_pseudogene"; 
gene_name "DDX11L1"; level 2; havana_gene "OTTHUMG00000000961.2";
</pre>

### 5. VCF :

The Variant Call Format (VCF) specifies the format of a text file used in bioinformatics for storing gene sequence variations. VCF is a text file format (most likely stored in a compressed manner). It contains meta-information lines, a header line, and then data lines each containing information about a position in the genome. The format also has the ability to contain genotype information on samples for each position. Since VCF files store contact information, they're often seen as the export/import format of some address book programs. This makes it easy to share one or more contacts, use the same contacts in different email programs or services, or back up your address book to a file.

<pre>
##fileformat=VCFv4.3
##fileDate=20090805
##source=myImputationProgramV3.1
##reference=file:///seq/references/1000GenomesPilot-NCBI36.fasta
##contig=<ID=20,length=62435964,assembly=B36,md5=f126cdf8a6e0c7f379d618ff66beb2da,species="Homo sapiens",taxonomy=x>
##phasing=partial
##INFO=<ID=NS,Number=1,Type=Integer,Description="Number of Samples With Data">
##INFO=<ID=DP,Number=1,Type=Integer,Description="Total Depth">
##INFO=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">
##INFO=<ID=AA,Number=1,Type=String,Description="Ancestral Allele">
##INFO=<ID=DB,Number=0,Type=Flag,Description="dbSNP membership, build 129">
##INFO=<ID=H2,Number=0,Type=Flag,Description="HapMap2 membership">
##FILTER=<ID=q10,Description="Quality below 10">
##FILTER=<ID=s50,Description="Less than 50% of samples have data">
##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
##FORMAT=<ID=GQ,Number=1,Type=Integer,Description="Genotype Quality">
##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read Depth">
##FORMAT=<ID=HQ,Number=2,Type=Integer,Description="Haplotype Quality">
#CHROM POS      ID         REF   ALT    QUAL  FILTER   INFO                             FORMAT       NA00001         NA00002          NA00003
20     14370    rs6054257  G     A      29    PASS    NS=3;DP=14;AF=0.5;DB;H2           GT:GQ:DP:HQ  0|0:48:1:51,51  1|0:48:8:51,51   1/1:43:5:.,.
20     17330    .          T     A      3     q10     NS=3;DP=11;AF=0.017               GT:GQ:DP:HQ  0|0:49:3:58,50  0|1:3:5:65,3     0/0:41:3
20     1110696  rs6040355  A     G,T    67    PASS    NS=2;DP=10;AF=0.333,0.667;AA=T;DB GT:GQ:DP:HQ  1|2:21:6:23,27  2|1:2:0:18,2     2/2:35:4
20     1230237  .          T     .      47    PASS    NS=3;DP=13;AA=T                   GT:GQ:DP:HQ  0|0:54:7:56,60  0|0:48:4:51,51   0/0:61:2
20     1234567  microsat1  GTC   G,GTCT 50    PASS    NS=3;DP=9;AA=G                    GT:GQ:DP     0/1:35:4        0/2:17:2         1/1:40:3
</pre>

### 6. SAM : 

SAM stands for Sequence Alignment Map format. It is a TAB-delimited text format consisting of a header section, which is optional, and an alignment section. If present, the header must be prior to the alignments. The SAM Format is a text format for storing sequence data in a series of tab delimited ASCII columns. 

<pre>
HWI-ST865:416:C6CG0ACXX:1:1313:9073:43827 0 I 2 1 99M * 0 0 CCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCT @C@DFDEFFHDFFIIJIGIIGIGGIIIIJGHGIJJEEIAHHGGIGFH@HGCFGGGJJIIGDAFG@DGIHHHHHFFBB@CACEC6;?CDD?CDCAD>>AA AS:i:0 XS:i:0 XN:i:0 XM:i:0 XO:i:0 XG:i:0 NM:i:0 MD:Z:99 YT:Z:UU
HWI-ST865:416:C6CG0ACXX:1:1215:16359:6484 16 I 9 1 85M * 0 0 CTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCC EEEEFFFFDAGHHHIJJIIJJJJJIJJJJIJIJJIGIIJJJJJJJIJJJJJJJIIJJJIIJGJJIJJJJJJJHFHHHFFFFFCCB AS:i:0 XS:i:0 XN:i:0 XM:i:0 XO:i:0 XG:i:0 NM:i:0 MD:Z:85 YT:Z:UU
HWI-ST865:416:C6CG0ACXX:1:1113:14118:89232 16 I 15 1 100M * 0 0 CTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAA CAC@A>C@AADCAC@ACEEC@@BD?E;@CEHGCEIGIHAFHGGF;FCHBHFBHIGIIIJJJJJJJJJJJJJJJJJJJJJIJJJJJJJHHHHHFFFFFCCC AS:i:0 XS:i:0 XN:i:0 XM:i:0 XO:i:0 XG:i:0 NM:i:0 MD:Z:100 YT:Z:UU
HWI-ST865:412:C6CLLACXX:1:2315:12173:84819 16 I 49 1 70M * 0 0 GCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCT @7)3CC=)CA;EBC>DAEDBDCDDDCDD@B?<DEDE399CBC<+>EAE<BDCEAE3DADDD<ABDD;1?? AS:i:0 XS:i:0 XN:i:0 XM:i:0 XO:i:0 XG:i:0 NM:i:0 MD:Z:70 YT:Z:UU HWI-ST865:412:C6CLLACXX:1:1201:19323:33842 16 I 71 0 100M * 0 0 AAGCCTAAGCCTAAGCCTAAGCCTAAGCCAAATCCCAAGCCTAAGCCTAAGCCTAAGCCTAAGCCAGAGCCTAAGCCTAAGCCTTAGCCTAAGCCTGATC DDDCCDCCACCCDCCCC>CAA@D@;BDHA3A7(@5/IIHFIIGEIIIIHEIIIIIGGIGIIIIIFDCIIIIIIIIGGIIGIHFFEIHDDBHFFDDDB@@@ AS:i:-33 XS:i:-33 XN:i:0 XM:i:8 XO:i:0 XG:i:0 NM:i:8 MD:Z:29T2G2T29T0A17A11A1G1 YT:Z:UU
HWI-ST865:412:C6CLLACXX:1:1215:19021:78287 16 I 93 1 66M * 0 0 CTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGCCTAAGC @=87=3GF=.:CFE;D@B3?3?BD9BC<>CJJJJJJJJJJJJJJJJIJJJJJIHHHHHFFEDAC@B AS:i:0 XS:i:0 XN:i:0 XM:i:0 XO:i:0 XG:i:0 NM:i:0 MD:Z:66 YT:Z:UU
</pre>

### 7. BAM : 

A Binary Alignment Map (BAM) file format is the compressed binary version of a SAM file that is used to represent aligned sequences up to 128 Mb. A BAM file contains two sections viz. Header and Alignment. Header—Contains information about the entire file, such as sample name, sample length, and alignment method. Alignments in the alignments section are associated with specific information in the header section. Alignments—Contains read name, read sequence, read quality, alignment information, and custom tags. 

<pre>
@HD VN:1.3  SO:coordinate
@SQ SN:ref  LN:45
@SQ SN:ref2 LN:40
r001    163 ref 7   30  8M4I4M1D3M  =   37  39  TTAGATAAAGAGGATACTG *   XX:B:S,12561,2,20,112
r002    0   ref 9   30  1S2I6M1P1I1P1I4M2I  *   0   0   AAAAGATAAGGGATAAA   *
r003    0   ref 9   30  5H6M    *   0   0   AGCTAA  *
r004    0   ref 16  30  6M14N1I5M   *   0   0   ATAGCTCTCAGC    *
r003    16  ref 29  30  6H5M    *   0   0   TAGGC   *
r001    83  ref 37  30  9M  =   7   -39 CAGCGCCAT   *
</pre>


Submitted by -
@prashikkk
