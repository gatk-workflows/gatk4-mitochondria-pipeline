# mitochondria-pipeline

### Purpose :
Workflow for SNP and INDEL variant calling on mitochondria.

### Requirements/expectations :
 - BAM or CRAM file
 - Median of the coverage over the autosome (if available, another central statistic would work too)

### Output :
 - A VCF file and its index
 - Addtional Metrics 
 - Optional realigned to chrM BAM

### Software version notes :
- GATK 4 or later 
- Cromwell version support 
  - Successfully tested on v37 
  - Does not work on versions < v23 due to output syntax

### Important Note :
- Runtime parameters are optimized for Broad's Google Cloud Platform implementation.
- For help running workflows on the Google Cloud Platform or locally please
view the following tutorial [(How to) Execute Workflows from the gatk-workflows Git Organization](https://software.broadinstitute.org/gatk/documentation/article?id=12521).
- The following material is provided by the GATK Team. Please post any questions or concerns to one of our forum sites : [GATK](https://gatkforums.broadinstitute.org/gatk/categories/ask-the-team/) , [FireCloud](https://gatkforums.broadinstitute.org/firecloud/categories/ask-the-firecloud-team) , [WDL/Cromwell](https://gatkforums.broadinstitute.org/wdl/categories/ask-the-wdl-team).
- Please visit the [User Guide](https://software.broadinstitute.org/gatk/documentation/) site for further documentation on our workflows and tools.

### LICENSING :
Copyright Broad Institute, 2018 | BSD-3
This script is released under the WDL open source code license (BSD-3) (full license text at https://github.com/openwdl/wdl/blob/master/LICENSE). Note however that the programs it calls may be subject to different licenses. Users are responsible for checking that they are authorized to run all programs before running this script.
