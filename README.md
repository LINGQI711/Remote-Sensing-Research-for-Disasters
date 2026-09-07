# Remote Sensing Research for Disasters

A year-organized collection of papers, datasets, and open resources for disaster monitoring, damage assessment, visual question answering, information retrieval, response, and recovery.

## Overview

Remote sensing and crisis-media data provide complementary evidence before, during, and after disasters. This repository tracks disaster-focused work across floods, wildfires, landslides, earthquakes, storms, and cascading hazards, with emphasis on reusable imagery, labels, question-answer pairs, retrieval corpora, and geospatial layers. Disaster geolocalization is also covered through cross-view imagery and location mentions in crisis text; general-purpose geolocation work is explicitly marked as supporting material.

## Papers

Venue labels distinguish conference proceedings, Findings, workshops, journal articles, and preprints. Papers are grouped by the formal publication year when available, otherwise by the preprint year. **arXiv preprint** means no conference or journal acceptance was verified; it does not imply rejection. Venue information last checked: **2026-09-06**. Journal entries use the issue year when assigned; online-first dates and delayed workshop-proceedings dates are noted where they differ.

**52 papers · 2017–2026.** [2026](#2026) · [2025](#2025) · [2024](#2024) · [2023](#2023) · [2022](#2022) · [2021](#2021) · [2020](#2020) · [2019](#2019) · [2018](#2018) · [2017](#2017)

### 2026

- **Triple-objective cross-view geolocalization of disaster-related VGI: the case of Hurricane Ian** — **[International Journal of Geographical Information Science (IJGIS) 2026](https://doi.org/10.1080/13658816.2025.2524857)** [[Code and Data](https://doi.org/10.6084/m9.figshare.28238375)]
  - Dataset: **MultiIAN (MultiIan)**; methods: **StaGeo / TriGeo**. Links volunteered images and text, street-view imagery, and overhead imagery for disaster geolocalization. Street-view panorama IDs are distributed subject to imagery licensing. Published online in 2025; assigned to volume 40(1), 2026.

- **Towards generative location awareness for disaster response: A probabilistic cross-view geolocalization approach** — **[ISPRS JPRS 2026](https://doi.org/10.1016/j.isprsjprs.2026.03.050)** [[Code and Data](https://github.com/bobleegogogo/ProbGLC)]
  - Method: **ProbGLC**. Combines probabilistic location prediction with cross-view retrieval, evaluated on **MultiIAN** and **SAGAINDisaster**. Provides location distributions and localizability scores rather than only a single coordinate.

- **SAGINGeo: A Space–Aerial–Ground Integrated Framework for VGI Geolocalization in Multidisaster Scenarios** — **[IEEE JSTARS 2026](https://doi.org/10.1109/JSTARS.2026.3712316)**
  - Related dataset: **SAGINDisaster**. Studies disaster-related VGI geolocalization across space, aerial, and ground views in multiple disaster scenarios. Published code and data packages use both `SAGAINDisaster` and `SAGINDisaster`; these spellings are recorded as aliases, not counted as independent datasets.

- **FireScope: Wildfire Risk Prediction with a Chain-of-Thought Oracle** — **[CVPR 2026](https://firescope.ai/research/)** [[arXiv](https://arxiv.org/abs/2511.17171)] [[Code](https://github.com/insait-institute/FireScope)] [[Data](https://huggingface.co/datasets/INSAIT-Institute/FireScope-Bench)]
  - Dataset: **FireScope-Bench**. Combines satellite imagery, climate inputs, risk rasters, and observed fire events for wildfire-risk prediction and explanation; includes European evaluation data. Earlier materials include “Raster” in the paper title.

- **FireSentry: A Multi-Modal Spatio-temporal Benchmark Dataset for Fine-Grained Wildfire Spread Forecasting** — **[KDD 2026 · Datasets and Benchmarks Track (author-confirmed acceptance)](https://github.com/Munan222/FireSentry-Benchmark-Dataset)** [[arXiv](https://arxiv.org/abs/2512.03369)]
  - Dataset: **FireSentry**; paradigm: **FiReDiff**. Integrates UAV RGB/infrared video, fire masks, environmental measurements, and vegetation information for fine-grained spread forecasting. Acceptance is announced in the official repository; access conditions vary by region and modality.

- **DisastQA: A Comprehensive Benchmark for Evaluating Question Answering in Disaster Management** — **[ACL 2026 Findings](https://aclanthology.org/2026.findings-acl.756/)** [[arXiv](https://arxiv.org/abs/2601.03670)] [[Code](https://github.com/TamuChen18/DisastQA_open)] [[Data](https://huggingface.co/datasets/tamuzc/DisastQA)]
  - Provides 3,000 verified text-based questions (2,000 multiple-choice and 1,000 open-ended) across eight disaster types, constructed from DisastIR. Evaluates 20 models under closed-book, noisy-evidence, and oracle-evidence settings, with keypoint-based scoring for factual completeness.

- **DisasterBench: A Multimodal Benchmark for UAV-Based Disaster Response in Complex Environments** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2606.06217)]
  - Covers 14 disaster scene types and nine response-critical tasks spanning pre-, during-, and post-disaster analysis.

- **Can LLM Agents Respond to Disasters? Benchmarking Heterogeneous Geospatial Reasoning in Emergency Operations (DORA)** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2605.11633)]
  - Introduces 515 expert-authored tasks across 45 events and 10 disaster types with multimodal geospatial evidence.

- **DisasterVQA: A Visual Question Answering Benchmark Dataset for Disaster Scenes** — **[ICWSM 2026](https://ojs.aaai.org/index.php/ICWSM/article/view/42776)** [[arXiv](https://arxiv.org/abs/2601.13839)] [[Data](https://zenodo.org/records/18267770)]
  - Contains 1,395 real-world images and 4,405 expert-curated questions covering floods, wildfires, earthquakes, hurricanes, fires, and other crisis scenes.

- **GEOID-Flood: A Large-Scale Multi-Modal Benchmark Dataset for Flood Segmentation** — **[ECCV 2026 Workshop · Terrabytes II (accepted)](https://arxiv.org/abs/2608.02315)** [[arXiv](https://arxiv.org/abs/2608.02315)]
  - Provides event-level flood segmentation data from Sentinel-1, Sentinel-2, and DEM observations across 219 events and 65 countries.

- **GeoDisaster: Benchmarking Orchestrated Agents for Operational Disaster Geo-Intelligence** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2606.17246)] [[Code](https://github.com/VIMAGE-IITB/GeoDisaster)]
  - Contains 2,921 verified instances for multi-hazard analysis, building-damage assessment, flood-safe routing, Sentinel-1 flood monitoring, and forest-change monitoring.

### 2025

- **Cross-view geolocalization and disaster mapping with street-view and VHR satellite imagery: A case study of Hurricane IAN** — **[ISPRS JPRS 2025](https://doi.org/10.1016/j.isprsjprs.2025.01.003)** [[arXiv](https://arxiv.org/abs/2408.06761)] [[Code](https://github.com/tum-bgd/CVDisaster)] [[Data](https://doi.org/10.14459/2024mp1749324)]
  - Dataset: **CVIAN**; framework: **CVDisaster**. Contains 4,121 paired street-view and overhead images after Hurricane Ian, with three damage-severity classes. Supports both cross-view geolocalization and disaster damage assessment.

- **Around the World in 80 Timesteps: A Generative Approach to Global Visual Geolocation** — **[CVPR 2025](https://openaccess.thecvf.com/content/CVPR2025/html/Dufour_Around_the_World_in_80_Timesteps_A_Generative_Approach_to_CVPR_2025_paper.html)** [[Code](https://github.com/nicolas-dufour/plonk)]
  - Method: **PLONK**. Uses generative modeling to estimate global location distributions. **Supporting method:** a foundation for the probabilistic component of ProbGLC, rather than a disaster-specific dataset.

- **TS-SatFire: A Multi-Task Satellite Image Time-Series Dataset for Wildfire Detection and Prediction** — **[Scientific Data 2025](https://www.nature.com/articles/s41597-025-06271-3)** [[Code](https://github.com/zhaoyutim/TS-SatFire)]
  - Dataset: **TS-SatFire**. Provides satellite image sequences with weather, terrain, and fuel information for active-fire detection, burned-area mapping, and next-day wildfire progression prediction.

- **Robust Burned Area Delineation Through Multitask Learning** — **[ECML PKDD 2023 Workshop · MACLEAN (revised proceedings 2025)](https://doi.org/10.1007/978-3-031-74633-8_32)** [[arXiv](https://arxiv.org/abs/2309.08368)] [[Code](https://github.com/links-ads/burned-area-seg)] [[Data](https://huggingface.co/datasets/links-ads/wildfires-cems)]
  - Dataset: **Wildfires-CEMS**. Pairs Sentinel-2 imagery with burned-area and land-cover labels, using multitask learning to improve burned-area delineation. Presented at the 2023 workshop; grouped here by the 2025 revised-proceedings publication.

- **LADI v2: Multi-label Dataset and Classifiers for Low-Altitude Disaster Imagery** — **[CVPR 2025 Workshops · EarthVision](https://openaccess.thecvf.com/content/CVPR2025W/EarthVision/papers/Scheele_LADI_v2_Multi-label_Dataset_and_Classifiers_for_Low-Altitude_Disaster_Imagery_CVPRW_2025_paper.pdf)** [[Code](https://github.com/LADI-Dataset/ladi-overview)] [[Data](https://huggingface.co/datasets/MITLL/LADI-v2-dataset)]
  - Dataset: **LADI v2**. Provides roughly 10,000 low-altitude disaster photographs annotated by trained Civil Air Patrol volunteers for multi-label classification, with baseline classifiers. The release identifies this as version 2.

- **Change3D: Revisiting Change Detection and Captioning from A Video Modeling Perspective** — **[CVPR 2025](https://openaccess.thecvf.com/content/CVPR2025/papers/Zhu_Change3D_Revisiting_Change_Detection_and_Captioning_from_A_Video_Modeling_CVPR_2025_paper.pdf)** [[arXiv](https://arxiv.org/abs/2503.18803)] [[Project](https://zhuduowang.github.io/Change3D)]
  - Method: **Change3D**. Treats bi-temporal imagery as a short video for change detection, building damage assessment, and change captioning. Its xBD-based building-damage implementation is a method example; the paper is not a new disaster dataset.

- **DisastIR: A Comprehensive Information Retrieval Benchmark for Disaster Management** — **[EMNLP 2025 Findings](https://aclanthology.org/2025.findings-emnlp.97/)** [[arXiv](https://arxiv.org/abs/2505.15856)] [[Code](https://github.com/KaiYin97/Disaster_IR)]
  - Provides 9,600 queries and more than 1.3 million labeled query-passage pairs across 48 retrieval tasks, six search intents, and 301 event types.

- **RSCC: A Large-Scale Remote Sensing Change Caption Dataset for Disaster Events** — **[NeurIPS 2025 · Datasets and Benchmarks Track](https://papers.neurips.cc/paper_files/paper/2025/file/62867024377cac4233195949b9db0ebd-Paper-Datasets_and_Benchmarks_Track.pdf)** [[arXiv](https://arxiv.org/abs/2509.01907)]
  - Contains 62,351 pre/post-event image pairs with human-written change captions for disaster-event interpretation.

- **DisasterM3: A Remote Sensing Vision-Language Dataset for Disaster Damage Assessment and Response** — **[NeurIPS 2025 · Datasets and Benchmarks Track](https://proceedings.neurips.cc/paper_files/paper/2025/hash/ec80d18205e39d42a27192d5f3ddd688-Abstract-Datasets_and_Benchmarks_Track.html)** [[Code](https://github.com/Junjue-Wang/DisasterM3)]
  - Offers 26,988 bi-temporal satellite images and 123k instruction pairs from 36 historical events, covering optical/SAR damage assessment and response.

- **RSVLM-QA: A Benchmark Dataset for Remote Sensing Vision Language Model-based Question Answering** — **[ACM MM 2025](https://doi.org/10.1145/3746027.3758235)** [[arXiv](https://arxiv.org/abs/2508.07918)] [[Code](https://github.com/StarZi0213/RSVLM-QA)]
  - Includes 13,820 remote-sensing images and 162,373 VQA pairs with captions, spatial relations, semantic tags, and counting questions.

- **BRIGHT: A Globally Distributed Multimodal Building Damage Assessment Dataset with Very-High-Resolution for All-Weather Disaster Response** — **[Earth System Science Data (ESSD) 2025](https://doi.org/10.5194/essd-17-6217-2025)** [[Code](https://github.com/ChenHongruixuan/BRIGHT)] [[Data](https://doi.org/10.5281/zenodo.14619797)]
  - Provides very-high-resolution optical and SAR imagery for building damage assessment across natural and human-made disasters.

### 2024

- **A globally distributed dataset of coseismic landslide mapping via multi-source high-resolution remote sensing images** — **[Earth System Science Data (ESSD) 2024](https://essd.copernicus.org/articles/16/4817/2024/)**
  - Dataset: **GDCLD**. Focuses on earthquake-triggered landslide mapping using multiple high-resolution remote-sensing sources, complementing GVLM and Landslide4Sense for evaluating geographic and sensor transfer. **Additional literature:** the linked paper and data release should be consulted for access details.

- **OpenStreetView-5M: The Many Roads to Global Visual Geolocation** — **[CVPR 2024](https://openaccess.thecvf.com/content/CVPR2024/papers/Astruc_OpenStreetView-5M_The_Many_Roads_to_Global_Visual_Geolocation_CVPR_2024_paper.pdf)** [[Project and Data](https://osv5m.github.io/)]
  - Dataset: **OSV-5M**. A general visual-geolocation resource with over 5.1 million georeferenced street-view images. **Supporting dataset:** referenced by the ProbGLC pipeline; this does not establish that the full dataset is downloaded or that it contains disaster labels.

- **FLOGA: A Machine-Learning-Ready Dataset, a Benchmark, and a Novel Deep Learning Model for Burnt Area Mapping With Sentinel-2** — **[IEEE JSTARS 2024](https://doi.org/10.1109/JSTARS.2024.3381737)** [[Code](https://github.com/Orion-AI-Lab/FLOGA)] [[Data](https://huggingface.co/datasets/orion-ai-lab/FLOGA-GeoTIFFs)]
  - Dataset: **FLOGA**; model: **BAM-CD**. Contains aligned pre/post-fire Sentinel-2 and MODIS imagery for 326 wildfire events in Greece with burned-area annotations. The paper and its release provide both a dataset and the BAM-CD model; it should be cited as a dataset-and-method contribution.

- **HRVQA: A Visual Question Answering Benchmark for High-Resolution Aerial Images** — **[ISPRS JPRS 2024](https://doi.org/10.1016/j.isprsjprs.2024.06.002)** [[arXiv](https://arxiv.org/abs/2301.09460)] [[Data](https://hrvqa.nl/)]
  - Provides 53,512 aerial images and 1,070,240 question-answer pairs across ten question types; disaster monitoring is one of the target applications.

### 2023

- **Cross-domain landslide mapping from large-scale remote sensing images using prototype-guided domain-aware progressive representation learning** — **[ISPRS JPRS 2023](https://doi.org/10.1016/j.isprsjprs.2023.01.018)** [[Code and Data](https://github.com/zxk688/GVLM)]
  - Dataset: **GVLM (Global Very-High-Resolution Landslide Mapping)**. Introduces a benchmark spanning 17 landslide sites with bi-temporal imagery and pixel annotations, together with a cross-domain mapping method. A cropped 256-pixel version is a derived data preparation, not a separate paper.

- **HR-GLDD: a globally distributed dataset using generalized deep learning (DL) for rapid landslide mapping on high-resolution (HR) satellite imagery** — **[Earth System Science Data (ESSD) 2023](https://essd.copernicus.org/articles/15/3283/2023/)** [[Data](https://doi.org/10.5281/zenodo.7189381)]
  - Dataset: **HR-GLDD**. Provides four-band PlanetScope imagery and landslide masks from ten rainfall- or earthquake-triggered events for cross-region generalization studies. **Additional literature:** the linked paper and data release should be consulted for access details.

- **Sample4Geo: Hard Negative Sampling For Cross-View Geo-Localisation** — **[ICCV 2023](https://openaccess.thecvf.com/content/ICCV2023/html/Deuser_Sample4Geo_Hard_Negative_Sampling_For_Cross-View_Geo-Localisation_ICCV_2023_paper.html)** [[Code](https://github.com/Skyy93/Sample4Geo)]
  - **Supporting method, not a disaster dataset.** Contrastive cross-view retrieval with hard-negative sampling; explicitly used as the geolocalization backbone in CVDisaster and relevant to CVIAN retrieval implementations.

- **IDRISI-RE: A generalizable dataset with benchmarks for location mention recognition on disaster tweets** — **[Information Processing & Management 2023](https://doi.org/10.1016/j.ipm.2023.103340)** [[Code and Data](https://github.com/rsuwaileh/IDRISI)]
  - Dataset: **IDRISI-RE**. Supports recognition of location mentions in English disaster tweets. Complements image-based cross-view localization with textual geographic evidence.

- **IDRISI-RA: The First Arabic Location Mention Recognition Dataset of Disaster Tweets** — **[ACL 2023 · Main Conference](https://aclanthology.org/2023.acl-long.901/)** [[Code and Data](https://github.com/rsuwaileh/IDRISI)]
  - Dataset: **IDRISI-RA**. Provides Arabic disaster-tweet annotations for location mention recognition, enabling multilingual disaster geolocation research.

- **IDRISI-D: Arabic and English Datasets and Benchmarks for Location Mention Disambiguation over Disaster Microblogs** — **[ArabicNLP 2023](https://aclanthology.org/2023.arabicnlp-1.14/)** [[Code and Data](https://github.com/rsuwaileh/IDRISI)]
  - Dataset: **IDRISI-D**. Resolves ambiguous location mentions in English and Arabic disaster microblogs to geographic entities. This is text-based location disambiguation, distinct from cross-view image retrieval.

- **Burned area semantic segmentation: A novel dataset and evaluation using convolutional networks** — **[ISPRS JPRS 2023](https://doi.org/10.1016/j.isprsjprs.2023.07.002)** [[Code](https://github.com/ipleiria-ciic/ees-datalab)] [[Data](https://zenodo.org/records/7944963)]
  - Dataset: **BurnedAreaUAV**. Provides 249 annotated UAV video frames for burned-area segmentation, with convolutional baselines and temporal-consistency evaluation.

- **MEDIC: a multi-task learning dataset for disaster image classification** — **[Neural Computing and Applications 2023](https://doi.org/10.1007/s00521-022-07717-0)** [[arXiv](https://arxiv.org/abs/2108.12828)] [[Data](https://crisisnlp.qcri.org/medic/)]
  - Dataset: **MEDIC**. Consolidates 71,198 images for disaster type, informativeness, humanitarian category, and damage severity classification. Includes CrisisMMD and other source collections; these are overlapping resources, not disjoint datasets. Published online in 2022; journal issue year 2023.

- **RescueNet: A High Resolution UAV Semantic Segmentation Dataset for Natural Disaster Damage Assessment** — **[Scientific Data 2023](https://www.nature.com/articles/s41597-023-02799-4)** [[Code and Data](https://github.com/BinaLab/RescueNet)]
  - Supports post-hurricane semantic segmentation and damage assessment using high-resolution UAV imagery.

- **Domain-Incremental Learning for Fire Detection in Space-Air-Ground Integrated Observation Network** — **[International Journal of Applied Earth Observation and Geoinformation (JAG) 2023](https://www.sciencedirect.com/science/article/pii/S1569843223001012)**
  - Studies domain-incremental fire detection using observations from space, aerial, and ground platforms.

- **Rapid Identification of Damaged Buildings Using Incremental Learning with Transferred Data from Historical Natural Disaster Cases** — **[ISPRS JPRS 2023](https://www.sciencedirect.com/science/article/pii/S0924271622003033)**
  - Transfers information from historical disaster cases to identify damaged buildings after a new event.

### 2022

- **Landslide4Sense: Reference Benchmark Data and Deep Learning Models for Landslide Detection** — **[IEEE TGRS 2022](https://doi.org/10.1109/TGRS.2022.3215209)** [[arXiv](https://arxiv.org/abs/2206.00515)] [[Data](https://zenodo.org/records/10463239)]
  - Dataset: **Landslide4Sense (L4S)**. Combines Sentinel-2 bands with elevation and slope for pixel-level landslide detection across four event regions. The released challenge splits contain 3,799 training, 245 validation, and 800 test patches.

- **The Outcome of the 2022 Landslide4Sense Competition: Advanced Landslide Detection From Multisource Satellite Imagery** — **[IEEE JSTARS 2022](https://doi.org/10.1109/JSTARS.2022.3220845)** [[arXiv](https://arxiv.org/abs/2209.02556)]
  - Companion study of the **Landslide4Sense** challenge, documenting the competition protocol and submitted landslide-segmentation approaches. Useful for selecting baselines; this is not a separate dataset.

- **An automatic fire detection system based on deep convolutional neural networks for low-power, resource-constrained devices** — **[Neural Computing and Applications 2022](https://doi.org/10.1007/s00521-022-07467-z)** [[Code and Data](https://github.com/gaia-solutions-on-demand/DFireDataset)]
  - Dataset: **D-Fire**. The official dataset repository requests this citation for its fire/smoke image collection. Relevant to ground-level fire detection and corresponding fire/smoke detection models.

- **SpaceNet 8: The Detection of Flooded Roads and Buildings** — **[CVPR 2022 Workshops · EarthVision](https://openaccess.thecvf.com/content/CVPR2022W/EarthVision/html/Hansch_SpaceNet_8_-_The_Detection_of_Flooded_Roads_and_Buildings_CVPRW_2022_paper.html)** [[Challenge](https://spacenet.ai/space8/)] [[Code](https://github.com/SpaceNetChallenge/SpaceNet8)]
  - Provides satellite imagery and labels for flooded-road and building detection in large-scale disaster scenes.

### 2021

- **Aerial imagery pile burn detection using deep learning: The FLAME dataset** — **[Computer Networks 2021](https://www.sciencedirect.com/science/article/pii/S1389128621001201)** [[arXiv](https://arxiv.org/abs/2012.14036)] [[Data](https://doi.org/10.21227/qad6-r683)]
  - Dataset: **FLAME**. Supports UAV-based fire/no-fire classification and fire segmentation. The full data may require IEEE DataPort access.

- **VQA-AID: Visual Question Answering for Post-Disaster Damage Assessment and Analysis** — **[IGARSS 2021](https://igarss2021.com/view_paper.php?PaperNum=4387)** [[arXiv](https://arxiv.org/abs/2106.10548)]
  - Introduces the HurMic-VQA dataset collected after Hurricane Michael for UAV-based post-disaster scene understanding.

- **FloodNet: A High Resolution Aerial Imagery Dataset for Post Flood Scene Understanding** — **[IEEE Access 2021](https://doi.org/10.1109/ACCESS.2021.3090981)** [[Code and Data](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021)]
  - Provides high-resolution post-flood UAV imagery for classification, semantic segmentation, and visual question answering.

### 2020

- **Deep Learning Benchmarks and Datasets for Social Media Image Classification for Disaster Response** — **[IEEE/ACM ASONAM 2020](https://doi.org/10.1109/ASONAM49781.2020.9381294)** [[arXiv](https://arxiv.org/abs/2011.08916)]
  - Consolidates disaster-image resources and benchmarks disaster type, informativeness, and damage severity classification, with duplicate-aware data splits. Also cited as an upstream reference for MEDIC.

- **Sen1Floods11: A Georeferenced Dataset to Train and Test Deep Learning Flood Algorithms for Sentinel-1** — **[CVPR 2020 Workshops](https://openaccess.thecvf.com/content_CVPRW_2020/html/w11/Bonafilia_Sen1Floods11_A_Georeferenced_Dataset_to_Train_and_Test_Deep_Learning_Flood_CVPRW_2020_paper.html)**
  - A georeferenced Sentinel-1 dataset for flood-water segmentation and cross-region evaluation.

- **RSVQA: Visual Question Answering for Remote Sensing Data** — **[IEEE TGRS 2020](https://doi.org/10.1109/TGRS.2020.2988782)** [[arXiv](https://arxiv.org/abs/2003.07333)]
  - Establishes an early remote-sensing VQA setting for natural-language interaction with Earth-observation images.

### 2019

- **Creating xBD: A Dataset for Assessing Building Damage from Satellite Imagery** — **[CVPR 2019 Workshops](https://openaccess.thecvf.com/content_CVPRW_2019/html/cv4gc/Gupta_Creating_xBD_A_Dataset_for_Assessing_Building_Damage_from_Satellite_CVPRW_2019_paper.html)** [[Data](https://xview2.org/dataset)]
  - A large-scale pre- and post-event satellite imagery dataset for building localization and damage classification across multiple disaster types.

### 2018

- **Damage Identification in Social Media Posts using Multimodal Deep Learning** — **[ISCRAM 2018](https://idl.iscram.org/files/husseinmouzannar/2018/2129_HusseinMouzannar_etal2018.pdf)**
  - Dataset connection: **Damage Multimodal Dataset (DMD)**. Uses text and images for damage-related information identification in social media. The corresponding source collection and citation are listed in MEDIC.

- **CrisisMMD: Multimodal Twitter Datasets from Natural Disasters** — **[ICWSM 2018](https://ojs.aaai.org/index.php/ICWSM/article/view/14983)** [[arXiv](https://arxiv.org/abs/1805.00713)] [[Data](https://crisisnlp.qcri.org/crisismmd)]
  - A multimodal Twitter dataset with image-text annotations from seven major 2017 disasters, supporting humanitarian information classification and response analysis.

### 2017

- **Predicting Ground-Level Scene Layout From Aerial Imagery** — **[CVPR 2017](https://openaccess.thecvf.com/content_cvpr_2017/html/Zhai_Predicting_Ground-Level_Scene_CVPR_2017_paper.html)**
  - **Supporting cross-view reference associated with the CVUSA panorama benchmark.** Learns ground-view semantic layout from co-located overhead imagery and evaluates geolocation and orientation. Cited as a supporting reference for MultiIAN; full CVUSA access should be checked at the source.

- **Damage Assessment from Social Media Imagery Data During Disasters** — **[IEEE/ACM ASONAM 2017](https://doi.org/10.1145/3110025.3110109)**
  - An early disaster-image damage-severity study using deep visual features and event-specific/cross-event evaluation. The associated damage-image collection is one of the sources documented in MEDIC.

## Resource Taxonomy

This repository is a literature and resource index. The categories below describe the role of each paper or dataset in disaster research; they are not intended to represent one specific implementation or data inventory. A paper may appear in more than one category when it contributes both a dataset and a method.

### 1. Task-Specific Datasets

These datasets are organized by the concrete task they support.

| Task | Representative datasets and papers | Typical inputs / outputs |
| --- | --- | --- |
| Building damage assessment and change analysis | [xBD](https://openaccess.thecvf.com/content_CVPRW_2019/html/cv4gc/Gupta_Creating_xBD_A_Dataset_for_Assessing_Building_Damage_from_Satellite_CVPRW_2019_paper.html), [BRIGHT](https://doi.org/10.5194/essd-17-6217-2025), [DisasterM3](https://github.com/Junjue-Wang/DisasterM3), [RescueNet](https://www.nature.com/articles/s41597-023-02799-4), [SpaceNet 8](https://spacenet.ai/space8/) | Bi-temporal satellite/UAV imagery → building masks, damage grades, flooded roads/buildings |
| Flood segmentation and water mapping | [FloodNet](https://doi.org/10.1109/ACCESS.2021.3090981), [Sen1Floods11](https://openaccess.thecvf.com/content_CVPRW_2020/html/w11/Bonafilia_Sen1Floods11_A_Georeferenced_Dataset_to_Train_and_Test_Deep_Learning_Flood_CVPRW_2020_paper.html), [GEOID-Flood](https://arxiv.org/abs/2608.02315), [SpaceNet 8](https://spacenet.ai/space8/) | UAV/SAR/optical/DEM imagery → water or flood-impact masks |
| Landslide mapping and change detection | [Landslide4Sense](https://doi.org/10.1109/TGRS.2022.3215209), [Landslide4Sense competition report](https://doi.org/10.1109/JSTARS.2022.3220845), [GVLM](https://doi.org/10.1016/j.isprsjprs.2023.01.018), [HR-GLDD](https://essd.copernicus.org/articles/15/3283/2023/), [GDCLD](https://essd.copernicus.org/articles/16/4817/2024/) | Multisource or very-high-resolution imagery → landslide masks and cross-region evaluation |
| Cross-view disaster geolocation | [CVIAN / CVDisaster](https://doi.org/10.1016/j.isprsjprs.2025.01.003), [MultiIAN](https://doi.org/10.1080/13658816.2025.2524857), [SAGINDisaster / SAGINGeo](https://doi.org/10.1109/JSTARS.2026.3712316), [ProbGLC](https://doi.org/10.1016/j.isprsjprs.2026.03.050) | VGI, street-view, ground and overhead imagery → candidate locations, rankings, uncertainty |
| Wildfire detection, burned-area mapping and spread forecasting | [FireSentry](https://arxiv.org/abs/2512.03369), [FireScope-Bench](https://huggingface.co/datasets/INSAIT-Institute/FireScope-Bench), [TS-SatFire](https://www.nature.com/articles/s41597-025-06271-3), [FLOGA](https://doi.org/10.1109/JSTARS.2024.3381737), [BurnedAreaUAV](https://doi.org/10.1016/j.isprsjprs.2023.07.002), [FLAME](https://doi.org/10.1016/j.comnet.2021.108001), [D-Fire](https://github.com/gaia-solutions-on-demand/DFireDataset), [Wildfires-CEMS](https://doi.org/10.1007/978-3-031-74633-8_32) | UAV/video/satellite/environmental data → fire masks, risk rasters, burned areas and future spread |
| Disaster image and social-media classification | [CrisisMMD](https://ojs.aaai.org/index.php/ICWSM/article/view/14983), [MEDIC](https://doi.org/10.1007/s00521-022-07717-0), [LADI v2](https://openaccess.thecvf.com/content/CVPR2025W/EarthVision/papers/Scheele_LADI_v2_Multi-label_Dataset_and_Classifiers_for_Low-Altitude_Disaster_Imagery_CVPRW_2025_paper.pdf), [DMD](https://idl.iscram.org/files/husseinmouzannar/2018/2129_HusseinMouzannar_etal2018.pdf) | Crisis images/text → disaster type, informativeness, humanitarian category and damage severity |
| Visual question answering and information retrieval | [RSVQA](https://doi.org/10.1109/TGRS.2020.2988782), [HRVQA](https://doi.org/10.1016/j.isprsjprs.2024.06.002), [RSVLM-QA](https://doi.org/10.1145/3746027.3758235), [DisasterVQA](https://ojs.aaai.org/index.php/ICWSM/article/view/42776), [DisastIR](https://aclanthology.org/2025.findings-emnlp.97/) | Images or disaster text → answers, captions, retrieval rankings and evidence |

### 2. Disaster VLM/Agent and Multimodal Benchmarks

This category focuses on evaluation suites for VLMs, LLM agents, multimodal reasoning and disaster-management QA. It is intentionally separate from ordinary segmentation or detection datasets.

| Benchmark | Evaluation focus | Paper / source |
| --- | --- | --- |
| **DisasterBench** | Multimodal UAV disaster response across pre-, during- and post-disaster tasks | [DisasterBench (arXiv 2026)](https://arxiv.org/abs/2606.06217) |
| **DORA** | Heterogeneous geospatial reasoning for emergency-operation agents | [Can LLM Agents Respond to Disasters? (arXiv 2026)](https://arxiv.org/abs/2605.11633) |
| **GeoDisaster** | Orchestrated agents for operational disaster geo-intelligence | [GeoDisaster (arXiv 2026)](https://arxiv.org/abs/2606.17246) |
| **DisastQA** | Disaster-management question answering with clean, noisy and absent evidence | [DisastQA (ACL 2026 Findings)](https://aclanthology.org/2026.findings-acl.756/) |
| **DisasterVQA** | Visual question answering over real-world disaster scenes | [DisasterVQA (ICWSM 2026)](https://ojs.aaai.org/index.php/ICWSM/article/view/42776) |
| **DisasterM3** | Remote-sensing vision-language instruction following for damage assessment and response | [DisasterM3 (NeurIPS 2025 Datasets and Benchmarks)](https://proceedings.neurips.cc/paper_files/paper/2025/hash/ec80d18205e39d42a27192d5f3ddd688-Abstract-Datasets_and_Benchmarks_Track.html) |
| **RSVLM-QA** | Remote-sensing VLM question answering, counting and spatial reasoning | [RSVLM-QA (ACM MM 2025)](https://doi.org/10.1145/3746027.3758235) |
| **DisastIR** | Disaster-management information retrieval and query-passage ranking | [DisastIR (EMNLP 2025 Findings)](https://aclanthology.org/2025.findings-emnlp.97/) |
| **GEOID-Flood** | Multimodal flood-segmentation benchmark; included here as a task benchmark, not a VLM/Agent benchmark | [GEOID-Flood (ECCV 2026 Workshop)](https://arxiv.org/abs/2608.02315) |

### 3. Task Methods and Models

These papers describe reusable methods, model architectures or inference strategies for the tasks above. Dataset papers may reappear when their method is an important baseline.

| Method family | Representative methods and papers | Main role |
| --- | --- | --- |
| Segmentation and change detection | [GVLM cross-domain mapping](https://doi.org/10.1016/j.isprsjprs.2023.01.018), [Change3D](https://openaccess.thecvf.com/content/CVPR2025/papers/Zhu_Change3D_Revisiting_Change_Detection_and_Captioning_from_A_Video_Modeling_CVPR_2025_paper.pdf), [BAM-CD/FLOGA](https://doi.org/10.1109/JSTARS.2024.3381737), domain-incremental fire detection ([JAG 2023](https://www.sciencedirect.com/science/article/pii/S1569843223001012)) | Pixel segmentation, bi-temporal change, building damage and domain generalization |
| Cross-view retrieval and geolocation | [Sample4Geo](https://openaccess.thecvf.com/content/ICCV2023/html/Deuser_Sample4Geo_Hard_Negative_Sampling_For_Cross-View_Geo-Localisation_ICCV_2023_paper.html), [CVDisaster-Geoloc](https://doi.org/10.1016/j.isprsjprs.2025.01.003), [StaGeo/TriGeo](https://doi.org/10.1080/13658816.2025.2524857), [ProbGLC](https://doi.org/10.1016/j.isprsjprs.2026.03.050), [SAGINGeo](https://doi.org/10.1109/JSTARS.2026.3712316) | Ground/street/overhead matching, candidate ranking, probabilistic location prediction |
| Generative geolocation and location uncertainty | [PLONK / Around the World in 80 Timesteps](https://openaccess.thecvf.com/content/CVPR2025/html/Dufour_Around_the_World_in_80_Timesteps_A_Generative_Approach_to_CVPR_2025_paper.html), [OpenStreetView-5M](https://openaccess.thecvf.com/content/CVPR2024/papers/Astruc_OpenStreetView-5M_The_Many_Roads_to_Global_Visual_Geolocation_CVPR_2024_paper.pdf) | Generative global geolocation, density estimation and geolocation pretraining |
| Disaster VQA and vision-language reasoning | [RSVQA](https://doi.org/10.1109/TGRS.2020.2988782), [HRVQA](https://doi.org/10.1016/j.isprsjprs.2024.06.002), [RSVLM-QA](https://doi.org/10.1145/3746027.3758235), [DisasterVQA](https://ojs.aaai.org/index.php/ICWSM/article/view/42776) | Visual question answering, counting, spatial relations and image-grounded answers |
| Retrieval and crisis-text geolocation | [IDRISI-RE](https://doi.org/10.1016/j.ipm.2023.103340), [IDRISI-RA](https://aclanthology.org/2023.acl-long.901/), [IDRISI-D](https://aclanthology.org/2023.arabicnlp-1.14/), [DisastIR](https://aclanthology.org/2025.findings-emnlp.97/) | Location mention recognition, disambiguation, multilingual retrieval and evidence discovery |
| Wildfire temporal prediction | [FiReDiff / FireSentry](https://arxiv.org/abs/2512.03369), [TS-SatFire](https://www.nature.com/articles/s41597-025-06271-3), [FireScope](https://firescope.ai/research/) | Video prediction, active-fire/burned-area mapping and wildfire-risk forecasting |
| Multimodal disaster classification | [MEDIC](https://doi.org/10.1007/s00521-022-07717-0), [LADI v2](https://openaccess.thecvf.com/content/CVPR2025W/EarthVision/papers/Scheele_LADI_v2_Multi-label_Dataset_and_Classifiers_for_Low-Altitude_Disaster_Imagery_CVPRW_2025_paper.pdf), [CrisisMMD](https://ojs.aaai.org/index.php/ICWSM/article/view/14983) | Multi-label image classification, humanitarian information extraction and damage assessment |

### Cross-Category Notes

- The same work may appear in multiple categories: for example, **DisasterM3** is both a task dataset and a vision-language benchmark, while **ProbGLC** is both a cross-view dataset paper and a geolocation method.
- **MEDIC** incorporates CrisisMMD, DMD and other source collections; these should not be added together as independent sample counts.
- Dataset names and paper titles are not always identical: GVLM, CVIAN, MultiIAN, SAGINDisaster, D-Fire and Wildfires-CEMS are indexed through their associated papers.
- A benchmark label describes an evaluation protocol or task suite; it does not by itself imply a VLM/Agent contribution.
- FireSR, Blaze and Corsican are retained only as uncategorized resource names in the search notes because a unique paper/version mapping was not established.

## Compact QA, VQA and Information-Retrieval Index

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
- **WorldPop** — high-resolution gridded population and demographic estimates for population exposure, affected-population estimation, and humanitarian planning. [[Data and project](https://www.worldpop.org/)]

### Remote-Sensing and Fire-Event Fields

| 数据字段 | 数据来源及用途 |
| --- | --- |
| `S2_B02/B03/B04/B08/B11`、`S2_SCL` | Sentinel-2 L2A 多光谱影像及地表分类，作为光学背景 |
| `FireMask`、`MaxFRP` | MODIS MYD14A1 活跃火点与火辐射功率，作为火情证据 |
| 隐藏的 `Burn_Date`、`QA` | MODIS MCD64A1 烧毁日期和质量标记，用于工具返回标签及真值计算 |

