Epigenome analysis pipeline review

1) Whole Genomoe Bisulfite Sequencing
2) miRNA analysis pipeline

# Step1
Raw sequencing quality check
Methods
1) FastQC Report<br>
   https://www.bioinformatics.babraham.ac.uk/projects/fastqc/
2) MultiQC Report<br>
   https://multiqc.info/

# Step2
Trimming raw sequencing datasets
1) TrimGalore<br>
   https://github.com/FelixKrueger/TrimGalore/blob/master/Docs/Trim_Galore_User_Guide.md
   
2) Cutadapt<br>
   pip install cutadapt

# Step3
Sequencing alignment using Bismark
1) Build reference genome
2) Align trimmed reads into the reference genome

# Step4
Extract CpG methylation level
1) Bismark methyl extract
2) Calculate sequencing depth and coverage

# Step5
Differential methylation block and CpG site analysis
1) methylKit package
2) customized block analysis (ratio-based/ count-based)

# Step6
Identification of biomarker
1) Pair-wise comparison
2) Pilot, non-parametric test
