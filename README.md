# mitochondria-pipeline

### Purpose :
Workflow for SNP and INDEL variant calling on mitochondria.

### Requirements/expectations :
 - BAM or CRAM file
 - Median of the coverage over the autosome (if available, another central statistic would work too)
 - Reference fasta (along with its index and dictionary) is only required when input is a BAM
 - Default for `max_read_length` is 151, this is purely an optimization parameter and won't effect the results.

### Output :
 - A VCF file and its index
 - Addtional Metrics 
 - Optional realigned to chrM BAM

### Software version notes :
- GATK 4.1 
- Cromwell version support 
  - Successfully tested on v37 
  - Does not work on versions < v23 due to output syntax

### Important Notes :
- Runtime parameters are optimized for Broad's Google Cloud Platform implementation.
- The provided JSON is a ready to use example JSON template of the workflow. Users are responsible for reviewing the [GATK Tool and Tutorial Documentations](https://gatk.broadinstitute.org/hc/en-us/categories/360002310591) to properly set the reference and resource variables. 
- For help running workflows on the Google Cloud Platform or locally please
view the following tutorial [(How to) Execute Workflows from the gatk-workflows Git Organization](https://gatk.broadinstitute.org/hc/en-us/articles/360035530952).
- Please visit the [User Guide](https://gatk.broadinstitute.org/hc/en-us/categories/360002310591) site for further documentation on our workflows and tools.
- Relevant reference and resources bundles can be accessed in [Resource Bundle](https://gatk.broadinstitute.org/hc/en-us/articles/360036212652).

### Contact Us :
- The following material is provided by the Data Science Platforum group at the Broad Institute. Please direct any questions or concerns to one of our forum sites : [GATK](https://gatk.broadinstitute.org/hc/en-us/community/topics) or [Terra](https://support.terra.bio/hc/en-us/community/topics/360000500432).

### LICENSING :
Copyright Broad Institute, 2020 | BSD-3
This script is released under the WDL open source code license (BSD-3) (full license text at https://github.com/openwdl/wdl/blob/master/LICENSE). Note however that the programs it calls may be subject to different licenses. Users are responsible for checking that they are authorized to run all programs before running this script.
