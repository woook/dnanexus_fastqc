# FastQC Reads Quality Control Github release v1.1.1

## What does this app do?

This app generates a QC report on reads data.

## What are typical use cases for this app?

This app is typically used after sequencing, to generate a QC report on the reads. As the FastQC manual says, "before analysing
reads to draw biological conclusions, you should always perform some simple quality control checks to ensure
that the raw data looks good and there are no problems or biases in your data which may affect how you can usefully use it."

## What data are required for this app to run?

This app requires reads data, in any of the following formats:

- Gzipped FASTQ files (`*.fq.gz` or `*.fastq.gz`)
- BAM files (`*.bam`)

## What does this app output?

This app outputs an HTML report that illustrates several metrics. For detailed information about the analysis modules included
in the report, consult the FastQC manual at:

http://www.bioinformatics.babraham.ac.uk/projects/fastqc/Help/

The QC stats are also output as a machine-readable text file.

## How does this app work?

This app runs FastQC, which analyzes the read data using various modules. The app returns the QC stats text file, exactly as
generated by FastQC.


## Custom modifications
Output files are saved to a subfolder 'QC' within any specified output folder