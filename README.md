![Github CI](https://github.com/BimberLab/DISCVRSeq/workflows/Github%20Actions%20CI/badge.svg)

## Overview
DISCVR-seq Toolkit is a diverse collection of tools for working with sequencing data, developed and maintained by the Bimber Lab, built using the GATK4 engine. The set of tools is analogous to GATK or Picard.  A description of all software produced by the Bimber Lab can be found [here](https://bimberlab.github.io).  

## Documentation
[Please view our documentation](https://bimberlab.github.io/DISCVRSeq/) for more information about the set of tools and usage.

## Getting Started
DISCVR-seq Toolkit is a java program distributed as a single JAR.  You can download the latest JAR from our [release page](https://github.com/BimberLab/DISCVRSeq/releases).  Running tools is analogous to GATK4.  

While we recommend [our documentation](https://bimberlab.github.io/DISCVRSeq/) to learn about available tools and options, one can also view a list of tools and/or arguments from the command line:

```

# List available tools:
java -jar DISCVRseq.jar --list 

# View arguments for a specific tool (VariantQC in this example):
java -jar DISCVRseq.jar VariantQC --help

```

## Docker

By popular demand, DISCVR-seq releases are available as docker images, via [GitHub Packages](https://github.com/orgs/BimberLab/packages/container/package/discvrseq).  We recommend using a specific release, which you can do using tags:

```

# Pull specific version:
docker pull ghcr.io/bimberlab/discvrseq:1.20

# Pull latest version:
docker pull ghcr.io/bimberlab/discvrseq:latest
# Or:
docker pull ghcr.io/bimberlab/discvrseq

# Running the container will automatically run DISCVRseq (equivalent to java -jar DISCVRseq.jar ...):
docker run ghcr.io/bimberlab/discvrseq --list

```