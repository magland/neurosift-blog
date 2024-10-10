# Neurosift blog

## AI assistant developments

2024-10-10

...


## LINDI, Neurosift and Dendro: INCF workshop

2024-09-26

Today I gave a virtual presentation at the INCF Neuroinformatics Assembly, held in Austin. For the talk, I focused on LINDI, but I prepared three documents covering LINDI, Neurosift, and Dendro.

[Leveraging LINDI for efficient and non-redundant NWB access on DANDI](./talks/lindi_INCF_assembly_sep_2024.md)

LINDI is a cloud-friendly format for representing NWB files in a way that separates metadata from large binary data to optimize streaming and reduce redundancy. This presentation covers the various LINDI file formats and highlights the performance improvements in streaming NWB files using precomputed LINDI files. The talk also touches on future integration of LINDI with DANDI and Neurosift.

[Exploring NWB Datasets on DANDI with Neurosift](./talks/neurosift_INCF_assembly_sep_2024.md)

Here I introduce Neurosift, a browser-based tool designed to explore NWB files stored in the DANDI Archive. Neurosift enables users to interactively visualize neurophysiology data by lazy-loading NWB files, offering efficient data streaming even for large files. It integrates seamlessly with DANDI, allowing users to open files directly from the archive and explore them using various visualization plugins. Neurosift leverages the LINDI format to pre-index Dandisets, speeding up metadata loading, and provides an intuitive interface for navigating neurophysiology data.


[Analyzing NWB Datasets on DANDI with Dendro](./talks/dendro_INCF_assembly_sep_2024.md)

Dendro is a framework designed to facilitate the collaborative analysis of NWB files stored on DANDI. Dendro runs containerized jobs on local or remote compute resources, integrating seamlessly with Neurosift and DANDI to provide a streamlined experience. This presentation showcases an example of computing autocorrelograms for neural units. Additionally, it demonstrated the setup and use of custom compute clients for distributed processing and presented early-stage developments in spike sorting and other advanced analyses.

## Exploring and Analyzing NWB Datasets on DANDI with Neurosift and Dendro: MIT workshop

2024-09-13

[In this workshop](./talks/neurosift_dendro_MIT_workshop_sep_2024.md) at the McGovern Institute for Brain Research (MIT), I walked participants through the process of exploring and analyzing NWB datasets on DANDI using Neurosift and Dendro.

## Neurosift: DANDI exploration and NWB visualization in the browser: JOSS paper

2024-05-27

Today we [published a paper](https://joss.theoj.org/papers/10.21105/joss.06590) in the Journal of Open Source Software (JOSS) describing Neurosift.

JOSS reviews are open and transparent. Feel free to check out the [review thread](https://github.com/openjournals/joss-reviews/issues/6590).

**Abstract:** Neurosift, a browser-based visualization tool, is designed for the interactive exploration of Neurodata Without Borders (NWB) files, whether stored locally, on remote servers, or within the Distributed Archives for Neurophysiology Data Integration (DANDI). NWB (Rübel et al., 2022; Teeters et al., 2015) is an open data standard for neurophysiology that enables the sharing, archiving, and analysis of various types of neurophysiology data. DANDI (Rübel et al., 2022) is a cloud-based platform that supports the storage, sharing, and analysis of neurophysiology data including NWB files. With Neurosift integration, users browsing DANDI can easily open any NWB file in the browser and explore its contents, including timeseries data, images, and more. Neurosift can also be used to browse the DANDI database or individual Dandisets. Overall, Neurosift simplifies the visualization and exploration of complex NWB file structures, making it a valuable tool for neuroscientists.

