# adapter-pipelines

![GitHub](https://img.shields.io/github/license/HumanCellAtlas/adapter-pipelines.svg?style=flat-square&colorB=blue)

This repo contains the (adapter) pipelines and other static files used by the HCA DCP Pipelines Execution Service
to interface the other services in the DCP, such as Data Store or Ingest. 

## File Structure

### [pipelines](./pipelines)

This directory hosts the adapter pipelines for all of the scientific pipelines
supported by the DCP Pipelines Execution Serivce. A corresponding adapter must be implemented here before the scientific pipeline can run in DCP.

### [shared](./shared)

This directory hosts the shared static files and the submission WDL that are 
used across different pipelines.

## Development

This repo will need to be updated whenever you make a change to the corresponding scientific pipelines or want to use a newer release of the [pipeline-tools](https://github.com/HumanCellAtlas/pipeline-tools).

## Contribute

Coming soon...
