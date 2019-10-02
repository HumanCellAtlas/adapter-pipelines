# adapter-pipelines

![GitHub](https://img.shields.io/github/license/HumanCellAtlas/adapter-pipelines.svg?style=flat-square&colorB=blue)

This repo contains the (adapter) pipelines and other static files used by the HCA DCP Pipelines Execution Service to interface the other services in the DCP, such as Data Store or Ingest. 

## File Structure

### [pipelines](./pipelines)

This directory hosts the adapter pipelines for all of the scientific pipelines
supported by the DCP Pipelines Execution Serivce. 

The pipelines wrap analysis pipelines from the Skylab repository and provide some glue to interface with the DCP. The adapters take bundle ids as inputs, query the Data Storage Service to find the input files needed by the analysis pipelines, then run the analysis pipelines and submit the results to the Ingest Service. This helps us keep the analysis pipelines themselves free of dependencies on the DCP.

Note: 
- The adapter pipelines can only run in Cromwell instances that use SAM for Identity and Access Management (IAM), such as Cromwell-as-a-Service.
- A corresponding adapter must be implemented here before the scientific pipeline can run in DCP.

### [shared](./shared)

This directory hosts the shared static files and the submission WDL that are 
used across different pipelines.

## Development

This repo will need to be updated whenever you make a change to the corresponding scientific pipelines or want to use a newer release of the [pipeline-tools](https://github.com/HumanCellAtlas/pipeline-tools).

## Contribute

Coming soon...
