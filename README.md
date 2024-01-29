Epigenome analysis pipeline review

1) Whole Genomoe Bisulfite Sequencing
2) miRNA analysis pipeline

# Step1
Raw sequencing quality check
Methods
1) FastQC Report
2) MultiQC Report

# Step2
Trimming raw sequencing datasets
1) TrimGalore
2) Cutadapt

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
