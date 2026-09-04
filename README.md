# Remote Sensing Research for Disasters

A year-organized collection of papers, datasets, and open resources for remote-sensing-based disaster monitoring, damage assessment, response, and recovery.

## Overview

Remote sensing provides timely, large-scale observations before, during, and after disasters. This repository tracks disaster-focused research across floods, wildfires, landslides, earthquakes, storms, and cascading hazards, with emphasis on reusable imagery, labels, geospatial layers, and evaluation resources.

## Papers

### 2026

- **DisasterBench: A Multimodal Benchmark for UAV-Based Disaster Response in Complex Environments** [[arXiv](https://arxiv.org/abs/2606.06217)]
  - Covers 14 disaster scene types and nine response-critical tasks spanning pre-, during-, and post-disaster analysis, including causal attribution, propagation prediction, damage assessment, and decision reasoning.

- **Can LLM Agents Respond to Disasters? Benchmarking Heterogeneous Geospatial Reasoning in Emergency Operations (DORA)** [[arXiv](https://arxiv.org/abs/2605.11633)]
  - Introduces 515 expert-authored tasks across 45 events and 10 disaster types, with multimodal geospatial evidence and tool-grounded emergency-operation scenarios.

- **GEOID-Flood: A Large-Scale Multi-Modal Benchmark Dataset for Flood Segmentation** [[arXiv](https://arxiv.org/abs/2608.02315)]
  - Provides event-level flood segmentation data from Sentinel-1, Sentinel-2, and DEM observations across 219 events and 65 countries.

- **GeoDisaster: Benchmarking Orchestrated Agents for Operational Disaster Geo-Intelligence** [[arXiv](https://arxiv.org/abs/2606.17246)] [[Code](https://github.com/VIMAGE-IITB/GeoDisaster)]
  - A disaster-oriented geospatial benchmark with 2,921 verified instances covering deforestation monitoring, multi-hazard analysis, building-damage assessment, flood-safe routing, and Sentinel-1 flood monitoring.

### 2025

- **RSCC: A Large-Scale Remote Sensing Change Caption Dataset for Disaster Events** [[arXiv](https://arxiv.org/abs/2509.01907)]
  - Contains 62,351 pre/post-event image pairs with human-written change captions for disaster-event interpretation.

- **DisasterM3: A Remote Sensing Vision-Language Dataset for Disaster Damage Assessment and Response** [[Code](https://github.com/Junjue-Wang/DisasterM3)]
  - Offers 26,988 bi-temporal satellite images and 123k instruction pairs from 36 historical events, spanning optical/SAR damage assessment and response tasks.

- **BRIGHT: A Globally Distributed Multimodal Building Damage Assessment Dataset with Very-High-Resolution for All-Weather Disaster Response** [[ESSD](https://doi.org/10.5194/essd-17-6217-2025)] [[Code](https://github.com/ChenHongruixuan/BRIGHT)] [[Data](https://doi.org/10.5281/zenodo.14619797)]
  - Provides very-high-resolution optical and SAR imagery for building damage assessment across natural and human-made disasters.

### 2023

- **Domain-Incremental Learning for Fire Detection in Space-Air-Ground Integrated Observation Network** [[International Journal of Applied Earth Observation and Geoinformation](https://www.sciencedirect.com/science/article/pii/S1569843223001012)]
  - Studies domain-incremental fire detection using observations from space, aerial, and ground platforms.

- **RescueNet: A High Resolution UAV Semantic Segmentation Dataset for Natural Disaster Damage Assessment** [[Scientific Data](https://www.nature.com/articles/s41597-023-02799-4)] [[Code and Data](https://github.com/BinaLab/RescueNet)]
  - Supports post-hurricane semantic segmentation and damage assessment using high-resolution UAV imagery.

- **Rapid Identification of Damaged Buildings Using Incremental Learning with Transferred Data from Historical Natural Disaster Cases** [[ISPRS Journal](https://www.sciencedirect.com/science/article/pii/S0924271622003033)]
  - Transfers information from historical disaster cases to identify damaged buildings after a new event.

### 2021

- **FloodNet: A High Resolution Aerial Imagery Dataset for Post Flood Scene Understanding** [[CVPR Workshops](https://openaccess.thecvf.com/content/CVPR2021W/UG2/html/Rahnemoonfar_FloodNet_A_High_Resolution_Aerial_Imagery_Dataset_for_Post_Flood_CVPRW_2021_paper.html)] [[Code and Data](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021)]
  - Provides high-resolution post-flood UAV imagery for classification, semantic segmentation, and visual question answering.

### 2020

- **Sen1Floods11: A Georeferenced Dataset to Train and Test Deep Learning Flood Algorithms for Sentinel-1** [[CVPR Workshops](https://openaccess.thecvf.com/content_CVPRW_2020/html/w11/Bonafilia_Sen1Floods11_A_Georeferenced_Dataset_to_Train_and_Test_Deep_Learning_Flood_CVPRW_2020_paper.html)]
  - A georeferenced Sentinel-1 dataset for flood-water segmentation and cross-region evaluation.

### 2019

- **xBD: A Dataset for Assessing Building Damage from Satellite Imagery** [[CVPR Workshops](https://openaccess.thecvf.com/content_CVPRW_2019/html/cv4gc/Gupta_xBD_A_Dataset_for_Assessing_Building_Damage_CVPRW_2019_paper.html)] [[Data](https://xview2.org/dataset)]
  - A large-scale pre- and post-event satellite imagery dataset for building localization and damage classification across multiple disaster types.

## Datasets and Resources Used in the Server Workspace

The inventory below is based on manifests and task files in `Disaster_Benchmark_Workspace`, plus the disaster datasets explicitly mentioned in the server setup.

| Area | Datasets / sources | Typical use |
| --- | --- | --- |
| Building damage and change | xBD / xView2, BRIGHT, DisasterM3, RescueNet | Pre/post comparison, building localization, damage grading, UAV scene segmentation |
| Flood mapping and hydrology | FloodNet, FloodNet-VQA, Sen1Floods11, GEOID-Flood, GloFAS, CHIRPS, JRC Global Surface Water | Flood extent, water segmentation, rainfall and river-flood context, flood-safe routing |
| Landslide and terrain | GVLM cropped imagery, Landslide4Sense (server-provided instance) | Landslide detection, change interpretation, terrain-aware assessment |
| Wildfire and smoke | Dixie wildfire samples, FireSentry, MODIS/FIRMS-style fixtures | Burned-area and smoke monitoring, fire-event trend analysis |
| Humanitarian and multimodal evidence | CrisisMMD, LADI, SpaceNet 8 | Social-media damage understanding, disaster imagery, flooded-road/building extraction |
| EO and GIS context layers | Sentinel-1, Sentinel-2, MODIS, OSM/OSMnx, WorldPop, GHSL, Dynamic World, WorldCover, Hansen Global Forest Change, TMF, RADD, Sentinel-5P, CAMS | SAR/optical evidence, population exposure, roads and shelters, land cover, air quality, forest change |

The benchmark workspace currently contains 222 task instances organized into four phases: mitigation (32), preparedness (45), response (115), and recovery (30). The task manifests combine real imagery with frozen geospatial fixtures and synthetic operational tables for facilities, shelters, roads, resources, communications, and recovery monitoring.

## Additional Climate Data

- **ERA5** — global atmospheric reanalysis data. [[Data](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels)]
- **CORDEX** — regional climate model and downscaling data. [[Project](https://cordex.org/)]
- **WRF** — numerical weather simulation framework for event-specific high-resolution meteorological data. [[Project](https://www.mmm.ucar.edu/models/wrf)]
