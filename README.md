# Remote Sensing Research for Disasters

A curated collection of papers, datasets, and resources on remote sensing research for disaster monitoring, assessment, response, and recovery.

## Overview

Remote sensing provides large-scale and timely observations for disaster monitoring, damage assessment, change detection, emergency response, and post-disaster recovery. This repository collects related papers, datasets, and open resources covering natural and human-made disasters.

## Papers

### 2025

- **BRIGHT: A Globally Distributed Multimodal Building Damage Assessment Dataset with Very-High-Resolution for All-Weather Disaster Response** \[[ESSD](https://doi.org/10.5194/essd-17-6217-2025)\] \[[Code](https://github.com/ChenHongruixuan/BRIGHT)\] \[[Data](https://doi.org/10.5281/zenodo.14619797)\] ![Disaster](https://img.shields.io/badge/Task-Damage_Assessment-red) ![Optical SAR](https://img.shields.io/badge/Modality-Optical%2BSAR-purple)
  - Provides very-high-resolution optical and SAR imagery for building damage assessment across natural and human-made disasters.

### 2023

- **Domain-Incremental Learning for Fire Detection in Space-Air-Ground Integrated Observation Network** \[[International Journal of Applied Earth Observation and Geoinformation](https://www.sciencedirect.com/science/article/pii/S1569843223001012)\] ![Fire](https://img.shields.io/badge/Disaster-Wildfire-FF4500) ![Continual Learning](https://img.shields.io/badge/Method-Domain--Incremental-yellow)
  - Studies domain-incremental fire detection using observations from space, aerial, and ground platforms.

- **RescueNet: A High Resolution UAV Semantic Segmentation Dataset for Natural Disaster Damage Assessment** \[[Scientific Data](https://www.nature.com/articles/s41597-023-02799-4)\] \[[Code and Data](https://github.com/BinaLab/RescueNet)\] ![Hurricane](https://img.shields.io/badge/Disaster-Hurricane-4169E1) ![UAV](https://img.shields.io/badge/Modality-UAV-purple)
  - Supports post-hurricane semantic segmentation and damage assessment using high-resolution UAV imagery.

- **Rapid Identification of Damaged Buildings Using Incremental Learning with Transferred Data from Historical Natural Disaster Cases** \[[ISPRS Journal](https://www.sciencedirect.com/science/article/pii/S0924271622003033)\] ![Damage](https://img.shields.io/badge/Task-Building_Damage-red) ![Incremental Learning](https://img.shields.io/badge/Method-Incremental_Learning-yellow)
  - Transfers information from historical disaster cases to identify damaged buildings after a new event.

### 2021

- **FloodNet: A High Resolution Aerial Imagery Dataset for Post Flood Scene Understanding** \[[CVPR Workshops](https://openaccess.thecvf.com/content/CVPR2021W/UG2/html/Rahnemoonfar_FloodNet_A_High_Resolution_Aerial_Imagery_Dataset_for_Post_Flood_CVPRW_2021_paper.html)\] \[[Code and Data](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021)\] ![Flood](https://img.shields.io/badge/Disaster-Flood-1E90FF) ![UAV](https://img.shields.io/badge/Modality-UAV-purple)
  - Provides high-resolution post-flood UAV imagery for classification, semantic segmentation, and visual question answering.

### 2019

- **xBD: A Dataset for Assessing Building Damage** \[[CVPR Workshops](https://openaccess.thecvf.com/content_CVPRW_2019/html/cv4gc/Gupta_xBD_A_Dataset_for_Assessing_Building_Damage_CVPRW_2019_paper.html)\] \[[Data](https://xview2.org/dataset)\] ![Multi Disaster](https://img.shields.io/badge/Disaster-Multi--Disaster-8A2BE2) ![Damage](https://img.shields.io/badge/Task-Building_Damage-red)
  - A large-scale pre- and post-event satellite imagery dataset for building localization and damage classification across multiple disaster types.

## Datasets

- **BRIGHT** — multimodal optical and SAR building-damage data covering earthquakes, storms, wildfires, floods, volcanic eruptions, explosions, and armed conflicts. \[[Data](https://doi.org/10.5281/zenodo.14619797)\] \[[Code](https://github.com/ChenHongruixuan/BRIGHT)\]

- **xBD** — pre- and post-disaster satellite images with building polygons and damage labels. \[[Data](https://xview2.org/dataset)\]

- **FloodNet** — post-flood UAV imagery for scene understanding. \[[Code and Data](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021)\]

- **RescueNet** — post-hurricane UAV imagery for semantic segmentation and damage assessment. \[[Code and Data](https://github.com/BinaLab/RescueNet)\]

## Additional Data Sources

- **ERA5** — global atmospheric reanalysis data. \[[Data](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels)\]
- **CORDEX** — regional climate model and downscaling data. \[[Project](https://cordex.org/)\]
- **WRF** — numerical weather simulation framework for constructing event-specific high-resolution meteorological data. \[[Project](https://www.mmm.ucar.edu/models/wrf)\]
