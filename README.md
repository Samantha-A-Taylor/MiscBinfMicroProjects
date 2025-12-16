# Miscellaneous Bioinformatics Micro-Projects | Computational Data Analytics
***
## Repository Overview ☰

This repository contains a collection of graduate-level bioinformatics and phylogenetics micro-projects completed during my Master’s degree. The projects span Bayesian and maximum likelihood inference, coalescent analyses, ancestral state reconstruction, molecular clock dating, gene flow testing, and genetic distance modeling, primarily using R and HPC-based workflows.

***
## The Evolution of Eusociality in Different Hymenopteran Species Using Ancestral State Reconstruction | Ancestral State Reconstruction and Evolutionary Modeling of Eusociality in Hymenoptera

**Objective:** To test whether primitive sociality serves as an evolutionary precursor to full eusociality in Hymenoptera by reconstructing ancestral social states using both discrete and continuous trait models.

       ✓ Designed and executed an independent, student-driven research project using R and R Markdown
       ✓ Compiled multi-gene sequence data from Hymenopteran species spanning solitary, primitively eusocial, and highly eusocial social structures, with Frankliniella occidentalis as an outgroup
       ✓ Selected and analyzed five candidate genes (BRI3, FASN, GRM1, MRJP1, Oamb) with putative links to eusocial behavior
       ✓ Performed gene-wise multiple sequence alignments, concatenation, and partitioning in R using msa and phangorn
       ✓ Generated partitioned maximum likelihood phylogenies in RAxML using a GTR+Γ model and 1,000 bootstrap replicates
       ✓ Assigned sociality character states as both discrete and continuous traits across species
       ✓ Conducted maximum likelihood ancestral state reconstruction using phytools, fitting ARD, stochastic (Markov), and Brownian motion models
       ✓ Visualized evolutionary transitions in eusociality with node-level probability representations across the phylogeny

<p align="center">
  <img width="405" height="315" alt="The Evolution Of Eusociality In Different Hymenopteran Species Using Ancestral State Reconstruction" src="https://github.com/user-attachments/assets/59e96238-6d06-4dac-8a02-497bf263dca8" />
</p>

## Concatenated & Coalescent Analyses | Multi-Gene Phylogenetic Inference and Comparative Tree Analysis in Rose Species

**Objective:** To estimate phylogenetic relationships among wild and cultivated rose species by comparing a partitioned concatenated Bayesian analysis with a coalescent-based species tree approach.

       ✓ Processed multi-gene sequence data (15 loci across 11 rose species plus a strawberry outgroup) using R in an R Markdown workflow
       ✓ Generated individual gene alignments with Clustal-Omega and created a concatenated Nexus alignment and partition file for MrBayes
       ✓ Performed a partitioned Bayesian phylogenetic analysis in MrBayes using a GTR+G+I model, unlinked parameters across loci, and a 1,000,000-iteration MCMC
       ✓ Constructed single-gene maximum likelihood trees with RAxML, including 1,000 bootstrap replicates per locus
       ✓ Conducted a coalescent-based species tree analysis using ASTRAL by combining individual gene trees and bootstrap files
       ✓ Imported, processed, and visualized MrBayes and ASTRAL trees in R, including node support formatting and branch length corrections

<p align="center">
<img width="630" height="315" alt="Concatenated---Coalescent-Analyses" src="https://github.com/user-attachments/assets/711eebc3-de5a-469e-88cd-c665c5e6dc34" />
</p>

## Bayesian Phylogenetic Inference | Bayesian Phylogenetic Analysis and Trait Evolution in Cucurbita Species

**Objective:** To infer evolutionary relationships within the genus Cucurbita using Bayesian phylogenetic methods and to determine how many independent domestication events occurred across pumpkins, squashes, and gourds.

       ✓ Analyzed sequence data from 8 Cucurbita species (wild and domesticated) with Citrullus lanatus as an outgroup using R in an R Markdown workflow
       ✓ Performed multiple sequence alignment in R using MUSCLE and identified the best-fit nucleotide substitution model with model testing
       ✓ Generated a Nexus alignment file and executed a Bayesian phylogenetic analysis in MrBayes with model-informed parameter settings
       ✓ Defined the outgroup and ran MCMC simulations to estimate posterior probabilities for phylogenetic relationships
       ✓ Downloaded and visualized the consensus tree in R with node support values displayed as posterior probabilities
       ✓ Conducted ancestral state reconstruction of domestication using maximum parsimony with an asymmetric transition cost matrix
       ✓ Modeled continuous trait evolution of size using ancestral state reconstruction and visualized results with customized trait-mapped trees

<p align="center">
<img width="441" height="315" alt="Bayesian-Phylogenetic-Inference" src="https://github.com/user-attachments/assets/9d5918b5-7c05-4a35-9dba-6046efc8c9c3" />
</p>

## Divergence Times & Gene Flow | Temporal Modeling and Gene Flow Analysis in Jumping Spiders

**Objective:** To estimate divergence times and diversification dynamics within the jumping spider genus Habronattus using a time-calibrated molecular clock, and to test for ongoing gene flow among closely related species.

       ✓ Analyzed multi-locus sequence data from 15 Habronattus species and one outgroup (Pellenes canadensis) using R and R Markdown
       ✓ Generated concatenated alignments and partition files for 63 noncoding loci using MUSCLE in R
       ✓ Performed a partitioned Bayesian molecular clock analysis in MrBayes with unlinked parameters and a variable-rate relaxed clock
       ✓ Defined multiple node dating constraints using truncated normal priors based on known divergence time estimates
       ✓ Ran a 10-million-iteration MCMC on an HPC cluster to obtain a time-calibrated phylogeny
       ✓ Visualized divergence times and confidence intervals in R using the MCMCtreeR package
       ✓ Evaluated diversification rate constancy using goodness-of-fit tests against null birth–death models
       ✓ Inferred SNP-based phylogenetic topology with SVDQuartets for a subset of closely related species
       ✓ Tested for directional gene flow using the ABBA–BABA (D-statistic) framework implemented in evobiR

<p align="center">
<img width="270" height="315" alt="Divergence-Times---Gene-Flow" src="https://github.com/user-attachments/assets/9a781269-d82c-47a0-a1e8-1f35ef5215a8" />
</p>

## Maximum Likelihood & Combining Trees | Phylogenetic Integration and Comparative Tree Analysis of Reptiles

**Objective:** To evaluate whether limblessness evolved once or multiple times in reptiles by comparing maximum likelihood phylogenies and integrating trees across genes and taxon sets.

       ✓ Analyzed multi-gene sequence data from snakes, lizards, legless lizards, and an outgroup using R, Bash, and R Markdown
       ✓ Performed multiple sequence alignments with Clustal-Omega and formatted data for phylogenetic inference
       ✓ Inferred maximum likelihood phylogenies for two genes (SLC8A1 and R35) using RAxML with a GTR+Γ model and 1,000 bootstrap replicates
       ✓ Visualized gene-specific phylogenies in R with node-level bootstrap support
       ✓ Quantitatively compared gene trees using tree distance metrics implemented in phangorn
       ✓ Incorporated additional legless lizard taxa by generating a separate R35 gene tree
       ✓ Constructed strict consensus trees and maximum agreement subtrees to assess topological concordance
       ✓ Combined partially overlapping taxon sets into a single supertree containing all species

<p align="center">
<img width="390.796875" height="315" alt="Maximum-Likelihood---Combining-Trees" src="https://github.com/user-attachments/assets/5f1f7213-218c-47d3-a95d-8f1ea2b4ce99" />
</p>

## Comparative Phylogenetic Inference & Tree Concordance Analysis | Comparative Phylogenetic Modeling and Topological Concordance Analysis

**Objective:** To infer evolutionary relationships using distance-based and maximum likelihood methods, compare phylogenetic signal across genomic sub-units, and quantify topological discordance between resulting trees.

       ✓ Analyzed a multi-sequence DNA dataset using R, Bash, and R Markdown
       ✓ Performed multiple sequence alignment in R and selected an appropriate nucleotide substitution 
          model for genetic distance estimation
       ✓ Constructed a rooted Neighbor-Joining tree with 100 bootstrap replicates using a model-based 
          distance matrix
       ✓ Inferred rooted maximum likelihood phylogenies for two genomic sub-units using RAxML with 1,000 
          bootstrap replicates each
       ✓ Visualized and annotated phylogenetic trees with node-level bootstrap support values
       ✓ Quantitatively compared sub-unit trees using symmetric difference, branch score distance, and path 
          difference metrics
       ✓ Identified shared phylogenetic structure by computing the maximum agreement subtree
       ✓ Investigated host range shifts by mapping host associations onto phylogenies to interpret patterns 
          of cross-species transmission

<p align="center">
<img width="468.05" height="315.1" alt="Comparative Phylogenetic Inference   Tree Concordance Analysis" src="https://github.com/user-attachments/assets/409cf44e-0e8d-4c3d-ab18-eec715b62d09" />
</p>

## Genetic Distance & Substitution Models | Longitudinal Model Evaluation and Distance-Based Analysis of Influenza (H3N2)

**Objective:** To evaluate nucleotide substitution models and distance-based phylogenetic methods using longitudinal influenza virus data, and to assess tree reliability through parsimony and bootstrapping analyses.

       ✓ Analyzed seasonal influenza (H3N2) sequence data collected over 16 years using R, Bash, and R 
          Markdown
       ✓ Performed multiple sequence alignment with Clustal-Omega using the msa package
       ✓ Compared nucleotide substitution models using likelihood and Bayesian Information Criterion (BIC) 
          scores in phangorn
       ✓ Calculated genetic distances under a best-fit model approximation and constructed UPGMA and 
          Neighbor-Joining trees
       ✓ Visualized and compared distance-based phylogenies to assess temporal clustering patterns
       ✓ Evaluated tree parsimony scores to identify the most parsimonious evolutionary hypothesis
       ✓ Performed bootstrap resampling to assess node-level support for inferred clades
       ✓ Collapsed weakly supported nodes to generate a simplified, confidence-optimized phylogeny

<p align="center">
<img width="346.999" height="315.5" alt="Genetic Distance   Substitution Models" src="https://github.com/user-attachments/assets/53b79d4e-6031-4fa0-8136-a3f720a0bbde" />
</p>

***
