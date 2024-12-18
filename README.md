# Setting Up the RNA-Seq Environment with Miniconda

This guide explains how to install Miniconda, set up a conda environment, and install essential tools for RNA-Seq analysis.

---

## Step 1: Install Miniconda

Download the installer from the Miniconda website
   ```bash
 wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
  ```
---

## Step 2: Run the installer:
   ```bash
   bash Miniconda3-latest-Linux-x86_64.sh
  ```
---
Press Enter to continue and view the license agreement.

Use the Up and Down cursor keys to browse through the agreement.

When prompted to accept the license terms, type yes to proceed.

Press Enter to continue and start the installation.

## Step 3: Activate Miniconda
   ```bash
source ~/miniconda3/bin/activate
  ```

---
## Step 4: Verify the installation
```bash
conda --version
  ```
---
## Step 5: Initialize Conda
```bash
conda init
  ```
---

## Step 6: Create a Conda Environment

```bash
conda create --name rnaseq_PPL
  ```
---
## Step 7: Activate the environment
```bash
conda activate rnaseq_PPL
  ```
---
## Step 8: Install Rna-Seq Tools (FastQC,Trimmomatic, Samtools, HISAT2, Stringtie)
### Install the required tools into your conda environment

### Install FastQC

```bash
conda install bioconda::fastqc
  ```
For each installation, type y when prompted to proceed.
### Install Trimmomatic
```bash
conda install bioconda::trimmomatic
  ```
For each installation, type y when prompted to proceed.

### Install SAMtools
```bash
conda install bioconda/label/cf201901::samtools
  ```
For each installation, type y when prompted to proceed.

### Install HISAT2
```bash
conda install bioconda::hisat2
  ```
For each installation, type y when prompted to proceed.

### Install StringTie
```bash
conda install bioconda::stringtie
  ```
For each installation, type y when prompted to proceed.

## Step 9: Verify Installation
### Check the versions of installed tools to ensure everything is set up correctly

## FastQC
```bash
fastqc --version
  ```
## Trimmomatic
```bash
trimmomatic -version
  ```
## SAMtools
```bash
samtools --version
  ```
## HISAT2
```bash
hisat2 --version
  ```
## StringTie
```bash
stringtie --version
  ```
# With all tools installed, you're ready to proceed with your RNA-Seq analysis.














