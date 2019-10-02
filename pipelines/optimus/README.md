# Overview

This directory contains an adapter pipeline used by the Pipelines Execution Service to run the Optimus pipeline.

## Files

### adapter.wdl

The adapter pipeline, which parses a bundle manifest from the Data Storage Service, runs the Optimus analysis pipeline, then runs the submission pipeline to submit the results to the Ingest Service.

### static_inputs.json

The adapter pipeline will use these inputs by default.

### options.json

Default options file to use when running the pipeline with Cromwell workflow execution engine.

### options_no_caching.json

The caching mechanism will be disabled if this options file is used.
