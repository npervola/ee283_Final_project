# ee283_Final_project
Output of Kundaje Lab Pipeline on Merged scATAC seq .fastq.gz files

The pipeline was executed with the following code ran interactivly, as the README specified to not qsub it:

bds atac.bds -species hg38_ENCODE -species_file /bio/npervola/ATACseq/kundaje_refs_data/hg38_ENCODE/ -nth 8 -bwt2_idx /bio/npervola/ATACseq/kundaje_refs_data/hg38_ENCODE/bowtie2_index/GRCh38_no_alt_analysis_set_GCA_000001405.15.fasta -fastq1_1 /bio/npervola/ATACseq/scATAC/raw_data/original_basal_luminal/scATAC.Combined_R1_Sequences.fastq.gz -fastq1_2 /bio/npervola/ATACseq/scATAC/raw_data/original_basal_luminal/scATAC.Combined_R2_Sequences.fastq.gz -out_dir /bio/npervola/ATACseq/scATAC/processed_data/original_basal_luminal/COMBINED_TEST/ -gensz hs -chrsz /bio/npervola/ATACseq/kundaje_refs_data/hg38_ENCODE/hg38_ENCODE.chrom.sizes -no_ataqc TRUE -title COMBINED_TEST