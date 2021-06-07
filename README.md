# Short variant discovery in RNAseq data on Azure
This repository is an example of running the RNAseq short variant discovery pipeline, based on [Best Practices RNAseq Short Variant Discovery Pipeline by Broad Institute of MIT and Harvard](https://gatk.broadinstitute.org/hc/en-us/articles/360035531192-RNAseq-short-variant-discovery-SNPs-Indels-), on Cromwell on Azure.<br/> 

Learn more about using Azure for your Cromwell WDL workflows on our GitHub repo! - [Cromwell on Azure](https://github.com/microsoft/CromwellOnAzure).<br/>

This repository is a fork from [the original](https://github.com/gatk-workflows/gatk4-rnaseq-germline-snps-indels) and has all the required changes to run the WDL workflow on Cromwell on Azure.<br/>

Here, you can find the WDL file and an example inputs JSON file with links to data hosted on a public Azure Storage account. You can use the "datasettestinputs" storage account directly as a relative path, like in the inputs JSON file.

The `gatk4-rna-germline-variant-calling.trigger.json` trigger file is ready to use. You can start the workflow on your instance of Cromwell on Azure, using [these instructions](https://github.com/microsoft/CromwellOnAzure/blob/master/docs/managing-your-workflow.md/#Start-your-workflow).


## gatk4-rnaseq-germline-snps-indels
### Purpose : 
Workflows for processing RNA data for germline short variant discovery with GATK v4 and related tools

### Requirements/expectations :
 - uBAM 

### Output :
 - A BAM file and its index.
 - A VCF file and its index. 
 - A Filtered VCF file and its index. 

### Software version :
 For program versions, see docker containers.

### Important Notes :
- The provided JSON is meant to be a ready to use example JSON template of the workflow. It is the user’s responsibility to correctly set the reference and resource input variables. 
- The following material is provided by the Data Science Platforum group at the Broad Institute. Please direct any questions or concerns to one of our forum sites : [GATK](https://gatk.broadinstitute.org/hc/en-us/community/topics) or [Terra](https://support.terra.bio/hc/en-us/community/topics/360000500432).

### LICENSING :
 This script is released under the WDL source code license (BSD-3) (see LICENSE in
 https://github.com/broadinstitute/wdl). Note however that the programs it calls may
 be subject to different licenses. Users are responsible for checking that they are
 authorized to run all programs before running this script. Please see the docker
 page at https://hub.docker.com/r/broadinstitute/genomes-in-the-cloud/ for detailed
 licensing information pertaining to the included programs. 
