# protaxA
PROTAX for aligned sequences

c.zip and scripts.zip contain c-code and Perl scripts required to train a Probabilistic Taxonomic classifier (PROTAX). Instructions are in file readme.txt

c2.zip contains c-code for classification. Sequences are represented as 64-bit integer vectors (representing 16 consecutive nucleotides as one long integer) in order to gain speedup. Speedup can be measured by running classify_v1 (sequences represented as character strings) and classify_v2 (sequences represented as 64-bit int vectors). Both programs measure the time for calculating all pairwise distances between query sequence and reference sequences and the time to convert the sequence distances into taxon probabilities. In addition, there are two programs: classify_rseq to classify reference sequences by not utilizing self-similarity and classify_info to print out information of the nearest and 2nd nearest reference sequence to query sequence in each node.
