# Pooled Cell Painting: Data Pipeline Welding Template :hammer_and_wrench:

This repository was derived from a [template repository](https://github.blog/2019-06-06-generate-new-repositories-with-repository-templates/) located at https://github.com/broadinstitute/pooled-cell-painting-profiling-template.
The purpose of the repository is to weld together a versioned data processing pipeline with versioned processed output data for a single Pooled Cell Painting experiment.

<p align="center">
<figure>
<img src="https://raw.githubusercontent.com/broadinstitute/pooled-cp-profiling-template/a57cb7f9e36b89ff56acf094f18ca06b1a53b719/media/pipeline_weld.png" width="500">
<figcaption>Data Pipeline Welding is the process of creating a new repository for each dataset within a Pooled Cell Painting project. The pooled-cell-painting-profiling-recipe contains the data processing pipeline. The user forks the recipe and can then edit their fork in a versioned manner. The pooled-cell-painting-profiling-template (this repo) contains the config files that must be edited for each dataset and therefore also need to be versioned. The fork of the recipe is added to the dataset-specific repo as a submodule. The code in the recipe can then be run and output morphology profiles that are completely versioned. </figcaption>
</figure>
</p>

A note about terminology:  
A `batch` is the data pipeline welding unit.
As the pipeline is currently written, a `batch` is a single plate of data and may also be referred to as a `dataset`.
An `experiment` is designed around a specific question and may contain single or multiple batches, depending on the experimental design.
A `project` is an encompassing term and may contain any number of experiments (and therefore any number of batches).
