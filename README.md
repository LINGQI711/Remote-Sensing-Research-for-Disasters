# Remote Sensing Research for Disasters

A year-organized collection of papers, datasets, and open resources for disaster monitoring, damage assessment, visual question answering, information retrieval, response, and recovery.

## Overview

Remote sensing and crisis-media data provide complementary evidence before, during, and after disasters. This repository tracks disaster-focused work across floods, wildfires, landslides, earthquakes, storms, and cascading hazards, with emphasis on reusable imagery, labels, question-answer pairs, retrieval corpora, and geospatial layers.

## Papers

### 2026

- **DisastQA: A Comprehensive Benchmark for Evaluating Question Answering in Disaster Management** [[arXiv](https://arxiv.org/abs/2601.03670)] [[Code](https://github.com/TamuChen18/DisastQA_open)] [[Data](https://huggingface.co/datasets/tamuzc/DisastQA)]
  - Provides 3,000 verified text-based questions (2,000 multiple-choice and 1,000 open-ended) across eight disaster types, constructed from DisastIR. Evaluates 20 models under closed-book, noisy-evidence, and oracle-evidence settings, with keypoint-based scoring for factual completeness.

- **DisasterBench: A Multimodal Benchmark for UAV-Based Disaster Response in Complex Environments** [[arXiv](https://arxiv.org/abs/2606.06217)]
  - Covers 14 disaster scene types and nine response-critical tasks spanning pre-, during-, and post-disaster analysis.

- **Can LLM Agents Respond to Disasters? Benchmarking Heterogeneous Geospatial Reasoning in Emergency Operations (DORA)** [[arXiv](https://arxiv.org/abs/2605.11633)]
  - Introduces 515 expert-authored tasks across 45 events and 10 disaster types with multimodal geospatial evidence.

- **DisasterVQA: A Visual Question Answering Benchmark Dataset for Disaster Scenes** [[arXiv](https://arxiv.org/abs/2601.13839)] [[ICWSM 2026](https://ojs.aaai.org/index.php/ICWSM/article/view/42776)] [[Data](https://zenodo.org/records/18267770)]
  - Contains 1,395 real-world images and 4,405 expert-curated questions covering floods, wildfires, earthquakes, hurricanes, fires, and other crisis scenes.

- **GEOID-Flood: A Large-Scale Multi-Modal Benchmark Dataset for Flood Segmentation** [[arXiv](https://arxiv.org/abs/2608.02315)]
  - Provides event-level flood segmentation data from Sentinel-1, Sentinel-2, and DEM observations across 219 events and 65 countries.

- **GeoDisaster: Benchmarking Orchestrated Agents for Operational Disaster Geo-Intelligence** [[arXiv](https://arxiv.org/abs/2606.17246)] [[Code](https://github.com/VIMAGE-IITB/GeoDisaster)]
  - Contains 2,921 verified instances for multi-hazard analysis, building-damage assessment, flood-safe routing, Sentinel-1 flood monitoring, and forest-change monitoring.

### 2025

- **DisastIR: A Comprehensive Information Retrieval Benchmark for Disaster Management** [[arXiv](https://arxiv.org/abs/2505.15856)] [[Code](https://github.com/KaiYin97/Disaster_IR)]
  - Provides 9,600 queries and more than 1.3 million labeled query-passage pairs across 48 retrieval tasks, six search intents, and 301 event types.

- **RSCC: A Large-Scale Remote Sensing Change Caption Dataset for Disaster Events** [[arXiv](https://arxiv.org/abs/2509.01907)]
  - Contains 62,351 pre/post-event image pairs with human-written change captions for disaster-event interpretation.

- **DisasterM3: A Remote Sensing Vision-Language Dataset for Disaster Damage Assessment and Response** [[Code](https://github.com/Junjue-Wang/DisasterM3)]
  - Offers 26,988 bi-temporal satellite images and 123k instruction pairs from 36 historical events, covering optical/SAR damage assessment and response.

- **RSVLM-QA: A Benchmark Dataset for Remote Sensing Vision Language Model-based Question Answering** [[arXiv](https://arxiv.org/abs/2508.07918)] [[Code](https://github.com/StarZi0213/RSVLM-QA)]
  - Includes 13,820 remote-sensing images and 162,373 VQA pairs with captions, spatial relations, semantic tags, and counting questions.

- **BRIGHT: A Globally Distributed Multimodal Building Damage Assessment Dataset with Very-High-Resolution for All-Weather Disaster Response** [[ESSD](https://doi.org/10.5194/essd-17-6217-2025)] [[Code](https://github.com/ChenHongruixuan/BRIGHT)] [[Data](https://doi.org/10.5281/zenodo.14619797)]
  - Provides very-high-resolution optical and SAR imagery for building damage assessment across natural and human-made disasters.

### 2024

- **HRVQA: A Visual Question Answering Benchmark for High-Resolution Aerial Images** [[ISPRS JPRS](https://doi.org/10.1016/j.isprsjprs.2024.06.002)] [[arXiv](https://arxiv.org/abs/2301.09460)] [[Data](https://hrvqa.nl/)]
  - Provides 53,512 aerial images and 1,070,240 question-answer pairs across ten question types; disaster monitoring is one of the target applications.

### 2023

- **RescueNet: A High Resolution UAV Semantic Segmentation Dataset for Natural Disaster Damage Assessment** [[Scientific Data](https://www.nature.com/articles/s41597-023-02799-4)] [[Code and Data](https://github.com/BinaLab/RescueNet)]
  - Supports post-hurricane semantic segmentation and damage assessment using high-resolution UAV imagery.

- **Domain-Incremental Learning for Fire Detection in Space-Air-Ground Integrated Observation Network** [[International Journal of Applied Earth Observation and Geoinformation](https://www.sciencedirect.com/science/article/pii/S1569843223001012)]
  - Studies domain-incremental fire detection using observations from space, aerial, and ground platforms.

### 2022

- **SpaceNet 8: The Detection of Flooded Roads and Buildings** [[Challenge](https://spacenet.ai/space8/)] [[Code](https://github.com/SpaceNetChallenge/SpaceNet8)]
  - Provides satellite imagery and labels for flooded-road and building detection in large-scale disaster scenes.

- **Rapid Identification of Damaged Buildings Using Incremental Learning with Transferred Data from Historical Natural Disaster Cases** [[ISPRS Journal](https://www.sciencedirect.com/science/article/pii/S0924271622003033)]
  - Transfers information from historical disaster cases to identify damaged buildings after a new event.

### 2021

- **VQA-AID: Visual Question Answering for Post-Disaster Damage Assessment and Analysis** [[arXiv](https://arxiv.org/abs/2106.10548)]
  - Introduces the HurMic-VQA dataset collected after Hurricane Michael for UAV-based post-disaster scene understanding.

- **FloodNet: A High Resolution Aerial Imagery Dataset for Post Flood Scene Understanding** [[CVPR Workshops](https://openaccess.thecvf.com/content/CVPR2021W/UG2/html/Rahnemoonfar_FloodNet_A_High_Resolution_Aerial_Imagery_Dataset_for_Post_Flood_CVPRW_2021_paper.html)] [[Code and Data](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021)]
  - Provides high-resolution post-flood UAV imagery for classification, semantic segmentation, and visual question answering.

### 2020

- **Sen1Floods11: A Georeferenced Dataset to Train and Test Deep Learning Flood Algorithms for Sentinel-1** [[CVPR Workshops](https://openaccess.thecvf.com/content_CVPRW_2020/html/w11/Bonafilia_Sen1Floods11_A_Georeferenced_Dataset_to_Train_and_Test_Deep_Learning_Flood_CVPRW_2020_paper.html)]
  - A georeferenced Sentinel-1 dataset for flood-water segmentation and cross-region evaluation.

- **RSVQA: Visual Question Answering for Remote Sensing Data** [[arXiv](https://arxiv.org/abs/2003.07333)]
  - Establishes an early remote-sensing VQA setting for natural-language interaction with Earth-observation images.

### 2019

- **xBD: A Dataset for Assessing Building Damage from Satellite Imagery** [[CVPR Workshops](https://openaccess.thecvf.com/content_CVPRW_2019/html/cv4gc/Gupta_xBD_A_Dataset_for_Assessing_Building_Damage_CVPRW_2019_paper.html)] [[Data](https://xview2.org/dataset)]
  - A large-scale pre- and post-event satellite imagery dataset for building localization and damage classification across multiple disaster types.

### 2018

- **CrisisMMD: Multimodal Twitter Datasets from Natural Disasters** [[ICWSM paper](https://ojs.aaai.org/index.php/ICWSM/article/download/14983/14833/18502)] [[arXiv](https://arxiv.org/abs/1805.00713)] [[Data](https://crisisnlp.qcri.org/crisismmd)]
  - A multimodal Twitter dataset with image-text annotations from seven major 2017 disasters, supporting humanitarian information classification and response analysis.

## Datasets and Resources Used in the Server Workspace

The inventory below is based on manifests, task files, source notes, and tool implementations in `Disaster_Benchmark_Workspace`, together with the disaster datasets explicitly mentioned in the server setup.

| Area | Datasets / sources | Typical use |
| --- | --- | --- |
| Building damage and change | xBD / xView2, BRIGHT, DisasterM3, RescueNet | Pre/post comparison, building localization, damage grading, UAV scene segmentation |
| Flood mapping and hydrology | FloodNet, FloodNet-VQA, Sen1Floods11, GEOID-Flood, SpaceNet 8, GloFAS, CHIRPS, JRC Global Surface Water | Flood extent, water segmentation, rainfall and river-flood context, flooded-road extraction, flood-safe routing |
| Landslide and terrain | GVLM cropped imagery, Landslide4Sense (server-provided instance) | Landslide detection, change interpretation, terrain-aware assessment |
| Wildfire and smoke | Dixie wildfire samples, FireSentry, MODIS/FIRMS-style fixtures | Burned-area and smoke monitoring, fire-event trend analysis |
| Humanitarian and social-media evidence | CrisisMMD, LADI, DisasterVQA, CrisisNLP-style labels | Damage reports, humanitarian categories, social-media situational awareness, image-text reasoning |
| Visual question answering | FloodNet-VQA, HurMic-VQA/VQA-AID, HRVQA, RSVLM-QA, DisasterVQA, RSVQA | Scene understanding, counting, spatial reasoning, damage and response questions |
| Information retrieval | DisastIR, CrisisMMD text, official alerts, news and humanitarian reports | Query-passage retrieval, fact checking, event and needs discovery |
| EO and GIS context layers | Sentinel-1, Sentinel-2, MODIS, OSM/OSMnx, WorldPop, GHSL, Dynamic World, WorldCover, Hansen Global Forest Change, TMF, RADD, Sentinel-5P, CAMS | SAR/optical evidence, population exposure, roads and shelters, land cover, air quality, forest change |

The benchmark workspace currently contains 222 task instances organized into four phases: mitigation (32), preparedness (45), response (115), and recovery (30). The manifests combine real imagery with frozen geospatial fixtures and synthetic operational tables for facilities, shelters, roads, resources, communications, and recovery monitoring.

## QA, VQA and Information-Retrieval Dataset Summary

| Resource | Modality | Scale / coverage | Disaster relevance |
| --- | --- | --- | --- |
| CrisisMMD | Twitter image + text | Seven 2017 disasters; roughly 18k multimodal samples | Humanitarian information, damage, needs, and infrastructure labels |
| DisasterVQA | Social-media images + QA | 1,395 images and 4,405 expert QA pairs | Disaster-scene perception and operational reasoning |
| DisastIR | Text queries + passages | 9,600 queries, 1.3M+ labeled pairs, 48 tasks | Disaster-management search and evidence retrieval |
| [DisastQA](https://arxiv.org/abs/2601.03670) | Text questions + evidence | 3,000 questions (2,000 multiple-choice + 1,000 open-ended); eight disaster types | Disaster QA under clean, noisy, or absent evidence; factual completeness |
| FloodNet-VQA | UAV image + QA | Post-flood scene understanding | Flood scene classification and visual questions |
| HurMic-VQA / VQA-AID | UAV image + QA | Hurricane Michael damage scenes | Post-disaster damage assessment |
| HRVQA | Aerial image + QA | 53,512 images and 1.07M QA pairs | High-resolution aerial reasoning with disaster-monitoring applications |
| RSVLM-QA | Remote-sensing image + QA | 13,820 images and 162,373 VQA pairs | Spatial, semantic, and counting reasoning for EO images |

## Additional Climate Data

- **ERA5** — global atmospheric reanalysis data. [[Data](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels)]
- **CORDEX** — regional climate model and downscaling data. [[Project](https://cordex.org/)]
- **WRF** — numerical weather simulation framework for event-specific high-resolution meteorological data. [[Project](https://www.mmm.ucar.edu/models/wrf)]
