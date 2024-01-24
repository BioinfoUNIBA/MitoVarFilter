# MitoVarFilter
<p text-align=center>This repository hosts the main scriptsfor handling variant calling from mtDNA in exome and genome sequencing FASTQ files. 
  The script mapExome_2024.pytakes the lead by automating the alignment process. It ensures that exome reads align accurately to the revised Cambridge Reference Sequence (rCRS) of human mtDNA and further refines the alignment by mapping reads against the complete GRCh38 human reference genometo eliminate nuclear mitochondrial DNA sequences (NUMTs). This automation, facilitated by a custom Python script, streamlines the entire mapping procedure, enhancing efficiency and reproducibility. 
  Moving on to mitochondrial DNA sequence reconstruction, the MToolBox proves instrumental. Specifically, the scripts assembleMTgenome_2024.pyand mtVariantCaller_2024.pyandVCFoutput.pyperformvariant calling and heteroplasmy quantification. 
  These steps are essential for understanding variations in mtDNA and quantifying the proportion of different variants within a mitochondrial population.MitoVarCleaner.pyscript removes variants associated with homopolymeric tracts (nucleotide positions 66-71, 300-316, 513-525, 5892, 3106-3107, 12418-12425, and 16182-16194). It also filters out variants lacking support from both forward and reverse DNA strands, as this absence may indicate sequencing artifacts or bias. 
  Additionally, variants with a Heteroplasmic Fraction (HF) less than 0.01 are excluded due to the challenge in differentiating them from potential technical errors.</p>
