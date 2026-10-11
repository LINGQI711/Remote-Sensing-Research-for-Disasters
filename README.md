# Remote Sensing Research for Disasters

Papers, models, datasets, and benchmarks for disaster monitoring, assessment, response, and recovery.

**62 unique papers · 2017–2026.** Papers with multiple contributions appear in multiple sections.

## Contents

- [Disaster Agents & Workflow Systems](#agents)
- [Disaster VLM/LLM Methods & Applications](#vlm-llm)
- [Task-Specific Methods & Models](#task-models)
- [Disaster Task Datasets & Benchmarks](#task-datasets)
- [Disaster QA, Instruction & Semantic Benchmarks](#qa-semantic)
- [Agent Planning & Execution Benchmarks](#agent-benchmarks)
- [Surveys](#surveys)
- [General-Purpose Supporting Resources](#supporting)
- [Environmental & Geospatial Resources](#environmental-resources)

<a id="agents"></a>

## Disaster Agents & Workflow Systems

### Multi-Agent Systems

- **MAS-LAND: A multi-agent system for landslide detection and rapid response** — **[International Journal of Disaster Risk Reduction (IJDRR) 2026](https://doi.org/10.1016/j.ijdrr.2026.106263)**
  - Framework: **MAS-LAND**. Combines post-event landslide segmentation, building and road exposure assessment, and automated operational reporting. Evaluated on the May 2023 Emilia–Romagna disaster using very-high-resolution orthophotos, SegFormer, RT-DETR building extraction, and OpenStreetMap roads; outputs interactive maps with landslide-specific reports.

- **Integration of large vision language models for efficient post-disaster damage assessment and reporting (DisasTeller)** — **[Nature Communications 2026](https://www.nature.com/articles/s41467-025-68216-z)** [[Code](https://github.com/zche3016/DisasTeller)] [[Output data](https://doi.org/10.5281/zenodo.17785783)]
  - Framework: **DisasTeller**. Coordinates multiple large vision-language model agents for post-disaster damage assessment, emergency alerts, resource allocation, recovery planning, and report generation. Evaluated using crisis imagery and flood/bushfire case studies; code and synthetic data are released by the authors.

- **GeoDisaster: Benchmarking Orchestrated Agents for Operational Disaster Geo-Intelligence** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2606.17246)] [[Code](https://github.com/VIMAGE-IITB/GeoDisaster)]
  - Benchmark: **GeoDisaster**. Contains 2,921 verified instances across five operational geospatial task families. Includes an orchestrated multi-agent framework with 18 tools and **Role-Contract Expectation Alignment (RCEA)** for tool use and execution consistency.

### Geospatially Grounded Agents

- **Empowering LLM Agents with Geospatial Awareness: Toward Grounded Reasoning for Wildfire Response** — **[ACL 2026 Findings (author-confirmed acceptance)](https://missa7481.github.io/publications/)** [[arXiv](https://arxiv.org/abs/2510.12061)]
  - Agent framework: **Geospatial Awareness Layer (GAL)**. Retrieves and integrates infrastructure, demographic, terrain, and weather data with wildfire detections to support LLM agents' personnel and budget recommendations, using historical analogs and daily changes.

<a id="vlm-llm"></a>

## Disaster VLM/LLM Methods & Applications

### Risk Prediction & Spatial Reasoning

- **Decoding the Disaster: Multi-Task Geospatial Reasoning with Vision-Language Models and Crowdsourced Imagery for Disaster Mapping** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2610.00302)]
  - Framework: **GRDisaster**. Uses a PhotoMappers-derived benchmark of 26,340 images arranged into human-validated VGI, street-view, and remote-sensing triplets spanning disaster events from 2018 to 2024. Combines cross-view geolocalization, multi-view fusion, spatial reasoning, and damage-severity assessment to interpret crowdsourced disaster imagery.

- **FireScope: Wildfire Risk Prediction with a Chain-of-Thought Oracle** — **[CVPR 2026](https://firescope.ai/research/)** [[arXiv](https://arxiv.org/abs/2511.17171)] [[Code](https://github.com/insait-institute/FireScope)] [[Data](https://huggingface.co/datasets/INSAIT-Institute/FireScope-Bench)]
  - Model: **FireScope**; dataset: **FireScope-Bench**. Uses VLM reasoning and visual supervision to generate wildfire-risk rasters from satellite imagery and climate data, with cross-continental evaluation in Europe.

### Recovery Assessment

- **Recov-Vision: Linking street view imagery and vision-language models for post-disaster recovery** — **[International Journal of Disaster Risk Reduction (IJDRR) 2026](https://doi.org/10.1016/j.ijdrr.2026.106388)** [[arXiv](https://arxiv.org/abs/2509.20628)] [[Code](https://github.com/YimingXiao98/RecovVision)] [[Data](https://huggingface.co/datasets/Ymx1025/FacadeTrack)]
  - Framework: **Recov-Vision**; data: **FacadeTrack**. Links panoramic street-view video to parcels and rectifies facade views for building-occupancy and recovery assessment. Compares rule-based and LLM-based decision policies across two post-Hurricane Helene surveys.

### UAV Disaster Understanding

- **DisasterBench: A Multimodal Benchmark for UAV-Based Disaster Response in Complex Environments** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2606.06217)]
  - Benchmark: **DisasterBench (UAV multimodal)**; model: **DisasterVL**. Covers 14 disaster scene types and nine tasks across pre-, during-, and post-disaster analysis. Introduces a lightweight multimodal model with instruction tuning, reasoning alignment, and reinforcement learning.

<a id="task-models"></a>

## Task-Specific Methods & Models

### Disaster Geolocalization

- **Triple-objective cross-view geolocalization of disaster-related VGI: the case of Hurricane Ian** — **[International Journal of Geographical Information Science (IJGIS) 2026](https://doi.org/10.1080/13658816.2025.2524857)** [[Code and Data](https://doi.org/10.6084/m9.figshare.28238375)]
  - Dataset: **MultiIAN (MultiIan)**; methods: **StaGeo / TriGeo**. Links volunteered images and text, street-view imagery, and overhead imagery for disaster geolocalization. Street-view panorama IDs are distributed subject to imagery licensing. Published online in 2025; assigned to volume 40(1), 2026.

- **Towards generative location awareness for disaster response: A probabilistic cross-view geolocalization approach** — **[ISPRS JPRS 2026](https://doi.org/10.1016/j.isprsjprs.2026.03.050)** [[Code and Data](https://github.com/bobleegogogo/ProbGLC)]
  - Method: **ProbGLC**. Combines probabilistic location prediction with cross-view retrieval, evaluated on **MultiIAN** and **SAGAINDisaster**. Provides location distributions and localizability scores rather than only a single coordinate.

- **SAGINGeo: A Space–Aerial–Ground Integrated Framework for VGI Geolocalization in Multidisaster Scenarios** — **[IEEE JSTARS 2026](https://doi.org/10.1109/JSTARS.2026.3712316)**
  - Framework: **SAGINGeo**; related dataset: **SAGINDisaster / SAGAINDisaster**. Studies disaster VGI geolocalization across space, aerial, and ground imagery in multiple disaster scenarios.

- **Cross-view geolocalization and disaster mapping with street-view and VHR satellite imagery: A case study of Hurricane IAN** — **[ISPRS JPRS 2025](https://doi.org/10.1016/j.isprsjprs.2025.01.003)** [[arXiv](https://arxiv.org/abs/2408.06761)] [[Code](https://github.com/tum-bgd/CVDisaster)] [[Data](https://doi.org/10.14459/2024mp1749324)]
  - Dataset: **CVIAN**; framework: **CVDisaster**. Contains 4,121 paired street-view and overhead images after Hurricane Ian, with three damage-severity classes. Supports both cross-view geolocalization and disaster damage assessment.

### Landslide Detection & Change Analysis

- **Guided diffusion-based image editing for landslide image synthesis in remote sensing change detection** — **[ISPRS JPRS 2026](https://doi.org/10.1016/j.isprsjprs.2026.08.007)** [[Code and Data](https://github.com/yixin28/HHDL-Dataset)]
  - Method: **Guided Landslide Generator (GLG)**. Uses landslide-specific prompts, spatio-temporal metadata, and DEM-informed masks to edit non-landslide samples into realistic landslide-change samples for change detection. Evaluated on **GVLM** and the newly constructed **HHDL** dataset.

- **Enhancing Sentinel-2 landslide change detection by integrating multispectral, deformation, and topographic information** — **[IJAEOG 2026](https://doi.org/10.1016/j.jag.2026.105116)** [[Code and Data](https://github.com/Trifurs/DMLCDNet)]
  - Method: **DMLCDNet**. Fuses bi-temporal Sentinel-2 multispectral features with Sentinel-1 deformation and ALOS DEM topographic information for landslide change detection, evaluated across Jiuzhaigou, Luding, Longyan, and additional generalization cases.

- **Cross-domain landslide mapping from large-scale remote sensing images using prototype-guided domain-aware progressive representation learning** — **[ISPRS JPRS 2023](https://doi.org/10.1016/j.isprsjprs.2023.01.018)** [[Code and Data](https://github.com/zxk688/GVLM)]
  - Dataset: **GVLM (Global Very-High-Resolution Landslide Mapping)**. Covers 17 landslide sites with bi-temporal imagery and pixel annotations, accompanied by prototype-guided cross-domain representation learning.

- **The Outcome of the 2022 Landslide4Sense Competition: Advanced Landslide Detection From Multisource Satellite Imagery** — **[IEEE JSTARS 2022](https://doi.org/10.1109/JSTARS.2022.3220845)** [[arXiv](https://arxiv.org/abs/2209.02556)]
  - Reports the **Landslide4Sense 2022** competition protocol and submitted landslide-segmentation methods.

### Wildfire Detection, Mapping & Forecasting

- **FireSentry: A Multi-Modal Spatio-temporal Benchmark Dataset for Fine-Grained Wildfire Spread Forecasting** — **[KDD 2026 · Datasets and Benchmarks Track (author-confirmed acceptance)](https://github.com/Munan222/FireSentry-Benchmark-Dataset)** [[arXiv](https://arxiv.org/abs/2512.03369)]
  - Dataset: **FireSentry**; paradigm: **FiReDiff**. Integrates UAV RGB/infrared video, fire masks, environmental measurements, and vegetation information for fine-grained spread forecasting. Acceptance is announced in the official repository; access conditions vary by region and modality.

- **Robust Burned Area Delineation Through Multitask Learning** — **[ECML PKDD 2023 Workshop · MACLEAN (revised proceedings 2025)](https://doi.org/10.1007/978-3-031-74633-8_32)** [[arXiv](https://arxiv.org/abs/2309.08368)] [[Code](https://github.com/links-ads/burned-area-seg)] [[Data](https://huggingface.co/datasets/links-ads/wildfires-cems)]
  - Dataset: **Wildfires-CEMS**. Pairs Sentinel-2 imagery with burned-area and land-cover labels, using multitask learning for burned-area delineation. Presented at the 2023 MACLEAN workshop; revised proceedings published in 2025.

- **FLOGA: A Machine-Learning-Ready Dataset, a Benchmark, and a Novel Deep Learning Model for Burnt Area Mapping With Sentinel-2** — **[IEEE JSTARS 2024](https://doi.org/10.1109/JSTARS.2024.3381737)** [[Code](https://github.com/Orion-AI-Lab/FLOGA)] [[Data](https://huggingface.co/datasets/orion-ai-lab/FLOGA-GeoTIFFs)]
  - Dataset: **FLOGA**; model: **BAM-CD**. Contains aligned pre/post-fire Sentinel-2 and MODIS imagery for 326 wildfire events in Greece, with burned-area annotations and a change-detection model.

- **Domain-Incremental Learning for Fire Detection in Space-Air-Ground Integrated Observation Network** — **[International Journal of Applied Earth Observation and Geoinformation (JAG) 2023](https://www.sciencedirect.com/science/article/pii/S1569843223001012)**
  - Studies domain-incremental fire detection using observations from space, aerial, and ground platforms.

- **An automatic fire detection system based on deep convolutional neural networks for low-power, resource-constrained devices** — **[Neural Computing and Applications 2022](https://doi.org/10.1007/s00521-022-07467-z)** [[Code and Data](https://github.com/gaia-solutions-on-demand/DFireDataset)]
  - Dataset: **D-Fire**. Provides fire/smoke imagery associated with a CNN-based detection system for low-power, resource-constrained devices.

### Building Damage & Change Analysis

- **Change3D: Revisiting Change Detection and Captioning from A Video Modeling Perspective** — **[CVPR 2025](https://openaccess.thecvf.com/content/CVPR2025/papers/Zhu_Change3D_Revisiting_Change_Detection_and_Captioning_from_A_Video_Modeling_CVPR_2025_paper.pdf)** [[arXiv](https://arxiv.org/abs/2503.18803)] [[Project](https://zhuduowang.github.io/Change3D)]
  - Method: **Change3D**. Treats bi-temporal imagery as a short video for change detection, building damage assessment, and change captioning, including xBD-based damage assessment.

- **Rapid Identification of Damaged Buildings Using Incremental Learning with Transferred Data from Historical Natural Disaster Cases** — **[ISPRS JPRS 2023](https://www.sciencedirect.com/science/article/pii/S0924271622003033)**
  - Transfers information from historical disaster cases to identify damaged buildings after a new event.

### Social-Media Damage Assessment

- **Damage Identification in Social Media Posts using Multimodal Deep Learning** — **[ISCRAM 2018](https://idl.iscram.org/files/husseinmouzannar/2018/2129_HusseinMouzannar_etal2018.pdf)**
  - Dataset: **Damage Multimodal Dataset (DMD)**. Combines text and images for disaster-related damage identification in social-media posts.

- **Damage Assessment from Social Media Imagery Data During Disasters** — **[IEEE/ACM ASONAM 2017](https://doi.org/10.1145/3110025.3110109)**
  - An early disaster-image damage-severity study using deep visual features and event-specific/cross-event evaluation. The associated damage-image collection is one of the sources documented in MEDIC.

<a id="task-datasets"></a>

## Disaster Task Datasets & Benchmarks

### Building Damage & Scene Segmentation

- **BRIGHT: A Globally Distributed Multimodal Building Damage Assessment Dataset with Very-High-Resolution for All-Weather Disaster Response** — **[Earth System Science Data (ESSD) 2025](https://doi.org/10.5194/essd-17-6217-2025)** [[Code](https://github.com/ChenHongruixuan/BRIGHT)] [[Data](https://doi.org/10.5281/zenodo.14619797)]
  - Provides very-high-resolution optical and SAR imagery for building damage assessment across natural and human-made disasters.

- **RescueNet: A High Resolution UAV Semantic Segmentation Dataset for Natural Disaster Damage Assessment** — **[Scientific Data 2023](https://www.nature.com/articles/s41597-023-02799-4)** [[Code and Data](https://github.com/BinaLab/RescueNet)]
  - Supports post-hurricane semantic segmentation and damage assessment using high-resolution UAV imagery.

- **SpaceNet 8: The Detection of Flooded Roads and Buildings** — **[CVPR 2022 Workshops · EarthVision](https://openaccess.thecvf.com/content/CVPR2022W/EarthVision/html/Hansch_SpaceNet_8_-_The_Detection_of_Flooded_Roads_and_Buildings_CVPRW_2022_paper.html)** [[Challenge](https://spacenet.ai/space8/)] [[Code](https://github.com/SpaceNetChallenge/SpaceNet8)]
  - Provides satellite imagery and labels for flooded-road and building detection in large-scale disaster scenes.

- **Creating xBD: A Dataset for Assessing Building Damage from Satellite Imagery** — **[CVPR 2019 Workshops](https://openaccess.thecvf.com/content_CVPRW_2019/html/cv4gc/Gupta_Creating_xBD_A_Dataset_for_Assessing_Building_Damage_from_Satellite_CVPRW_2019_paper.html)** [[Data](https://xview2.org/dataset)]
  - A large-scale pre- and post-event satellite imagery dataset for building localization and damage classification across multiple disaster types.

### Flood Mapping

- **GEOID-Flood: A Large-Scale Multi-Modal Benchmark Dataset for Flood Segmentation** — **[ECCV 2026 Workshop · Terrabytes II (accepted)](https://arxiv.org/abs/2608.02315)** [[arXiv](https://arxiv.org/abs/2608.02315)]
  - Provides event-level flood segmentation data from Sentinel-1, Sentinel-2, and DEM observations across 219 events and 65 countries.

- **FloodNet: A High Resolution Aerial Imagery Dataset for Post Flood Scene Understanding** — **[IEEE Access 2021](https://doi.org/10.1109/ACCESS.2021.3090981)** [[Code and Data](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021)]
  - Provides high-resolution post-flood UAV imagery for classification, semantic segmentation, and visual question answering.

- **Sen1Floods11: A Georeferenced Dataset to Train and Test Deep Learning Flood Algorithms for Sentinel-1** — **[CVPR 2020 Workshops](https://openaccess.thecvf.com/content_CVPRW_2020/html/w11/Bonafilia_Sen1Floods11_A_Georeferenced_Dataset_to_Train_and_Test_Deep_Learning_Flood_CVPRW_2020_paper.html)**
  - A georeferenced Sentinel-1 dataset for flood-water segmentation and cross-region evaluation.

### Landslide Mapping

- **Guided diffusion-based image editing for landslide image synthesis in remote sensing change detection** — **[ISPRS JPRS 2026](https://doi.org/10.1016/j.isprsjprs.2026.08.007)** [[Code and Data](https://github.com/yixin28/HHDL-Dataset)]
  - Method: **Guided Landslide Generator (GLG)**. Uses landslide-specific prompts, spatio-temporal metadata, and DEM-informed masks to edit non-landslide samples into realistic landslide-change samples for change detection. Evaluated on **GVLM** and the newly constructed **HHDL** dataset.

- **A globally distributed dataset of coseismic landslide mapping via multi-source high-resolution remote sensing images** — **[Earth System Science Data (ESSD) 2024](https://essd.copernicus.org/articles/16/4817/2024/)**
  - Dataset: **GDCLD**. Provides multi-source high-resolution imagery for earthquake-triggered landslide mapping and geographic transfer evaluation.

- **Cross-domain landslide mapping from large-scale remote sensing images using prototype-guided domain-aware progressive representation learning** — **[ISPRS JPRS 2023](https://doi.org/10.1016/j.isprsjprs.2023.01.018)** [[Code and Data](https://github.com/zxk688/GVLM)]
  - Dataset: **GVLM (Global Very-High-Resolution Landslide Mapping)**. Covers 17 landslide sites with bi-temporal imagery and pixel annotations, accompanied by prototype-guided cross-domain representation learning.

- **HR-GLDD: a globally distributed dataset using generalized deep learning (DL) for rapid landslide mapping on high-resolution (HR) satellite imagery** — **[Earth System Science Data (ESSD) 2023](https://essd.copernicus.org/articles/15/3283/2023/)** [[Data](https://doi.org/10.5281/zenodo.7189381)]
  - Dataset: **HR-GLDD**. Provides four-band PlanetScope imagery and landslide masks from ten rainfall- or earthquake-triggered events for cross-region evaluation.

- **Landslide4Sense: Reference Benchmark Data and Deep Learning Models for Landslide Detection** — **[IEEE TGRS 2022](https://doi.org/10.1109/TGRS.2022.3215209)** [[arXiv](https://arxiv.org/abs/2206.00515)] [[Data](https://zenodo.org/records/10463239)]
  - Dataset: **Landslide4Sense (L4S)**. Combines Sentinel-2 bands with elevation and slope for pixel-level landslide detection across four event regions. The released challenge splits contain 3,799 training, 245 validation, and 800 test patches.

### Wildfire Detection, Risk & Spread

- **FireScope: Wildfire Risk Prediction with a Chain-of-Thought Oracle** — **[CVPR 2026](https://firescope.ai/research/)** [[arXiv](https://arxiv.org/abs/2511.17171)] [[Code](https://github.com/insait-institute/FireScope)] [[Data](https://huggingface.co/datasets/INSAIT-Institute/FireScope-Bench)]
  - Model: **FireScope**; dataset: **FireScope-Bench**. Uses VLM reasoning and visual supervision to generate wildfire-risk rasters from satellite imagery and climate data, with cross-continental evaluation in Europe.

- **FireSentry: A Multi-Modal Spatio-temporal Benchmark Dataset for Fine-Grained Wildfire Spread Forecasting** — **[KDD 2026 · Datasets and Benchmarks Track (author-confirmed acceptance)](https://github.com/Munan222/FireSentry-Benchmark-Dataset)** [[arXiv](https://arxiv.org/abs/2512.03369)]
  - Dataset: **FireSentry**; paradigm: **FiReDiff**. Integrates UAV RGB/infrared video, fire masks, environmental measurements, and vegetation information for fine-grained spread forecasting. Acceptance is announced in the official repository; access conditions vary by region and modality.

- **TS-SatFire: A Multi-Task Satellite Image Time-Series Dataset for Wildfire Detection and Prediction** — **[Scientific Data 2025](https://www.nature.com/articles/s41597-025-06271-3)** [[Code](https://github.com/zhaoyutim/TS-SatFire)]
  - Dataset: **TS-SatFire**. Provides satellite image sequences with weather, terrain, and fuel information for active-fire detection, burned-area mapping, and next-day wildfire progression prediction.

- **Robust Burned Area Delineation Through Multitask Learning** — **[ECML PKDD 2023 Workshop · MACLEAN (revised proceedings 2025)](https://doi.org/10.1007/978-3-031-74633-8_32)** [[arXiv](https://arxiv.org/abs/2309.08368)] [[Code](https://github.com/links-ads/burned-area-seg)] [[Data](https://huggingface.co/datasets/links-ads/wildfires-cems)]
  - Dataset: **Wildfires-CEMS**. Pairs Sentinel-2 imagery with burned-area and land-cover labels, using multitask learning for burned-area delineation. Presented at the 2023 MACLEAN workshop; revised proceedings published in 2025.

- **FLOGA: A Machine-Learning-Ready Dataset, a Benchmark, and a Novel Deep Learning Model for Burnt Area Mapping With Sentinel-2** — **[IEEE JSTARS 2024](https://doi.org/10.1109/JSTARS.2024.3381737)** [[Code](https://github.com/Orion-AI-Lab/FLOGA)] [[Data](https://huggingface.co/datasets/orion-ai-lab/FLOGA-GeoTIFFs)]
  - Dataset: **FLOGA**; model: **BAM-CD**. Contains aligned pre/post-fire Sentinel-2 and MODIS imagery for 326 wildfire events in Greece, with burned-area annotations and a change-detection model.

- **Burned area semantic segmentation: A novel dataset and evaluation using convolutional networks** — **[ISPRS JPRS 2023](https://doi.org/10.1016/j.isprsjprs.2023.07.002)** [[Code](https://github.com/ipleiria-ciic/ees-datalab)] [[Data](https://zenodo.org/records/7944963)]
  - Dataset: **BurnedAreaUAV**. Provides 249 annotated UAV video frames for burned-area segmentation, with convolutional baselines and temporal-consistency evaluation.

- **An automatic fire detection system based on deep convolutional neural networks for low-power, resource-constrained devices** — **[Neural Computing and Applications 2022](https://doi.org/10.1007/s00521-022-07467-z)** [[Code and Data](https://github.com/gaia-solutions-on-demand/DFireDataset)]
  - Dataset: **D-Fire**. Provides fire/smoke imagery associated with a CNN-based detection system for low-power, resource-constrained devices.

- **Aerial imagery pile burn detection using deep learning: The FLAME dataset** — **[Computer Networks 2021](https://www.sciencedirect.com/science/article/pii/S1389128621001201)** [[arXiv](https://arxiv.org/abs/2012.14036)] [[Data](https://doi.org/10.21227/qad6-r683)]
  - Dataset: **FLAME**. Supports UAV-based fire/no-fire classification and fire segmentation. The full data may require IEEE DataPort access.

### Cross-View Disaster Geolocalization

- **Decoding the Disaster: Multi-Task Geospatial Reasoning with Vision-Language Models and Crowdsourced Imagery for Disaster Mapping** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2610.00302)]
  - Framework: **GRDisaster**. Uses a PhotoMappers-derived benchmark of 26,340 images arranged into human-validated VGI, street-view, and remote-sensing triplets spanning disaster events from 2018 to 2024. Combines cross-view geolocalization, multi-view fusion, spatial reasoning, and damage-severity assessment to interpret crowdsourced disaster imagery.

- **Triple-objective cross-view geolocalization of disaster-related VGI: the case of Hurricane Ian** — **[International Journal of Geographical Information Science (IJGIS) 2026](https://doi.org/10.1080/13658816.2025.2524857)** [[Code and Data](https://doi.org/10.6084/m9.figshare.28238375)]
  - Dataset: **MultiIAN (MultiIan)**; methods: **StaGeo / TriGeo**. Links volunteered images and text, street-view imagery, and overhead imagery for disaster geolocalization. Street-view panorama IDs are distributed subject to imagery licensing. Published online in 2025; assigned to volume 40(1), 2026.

- **SAGINGeo: A Space–Aerial–Ground Integrated Framework for VGI Geolocalization in Multidisaster Scenarios** — **[IEEE JSTARS 2026](https://doi.org/10.1109/JSTARS.2026.3712316)**
  - Framework: **SAGINGeo**; related dataset: **SAGINDisaster / SAGAINDisaster**. Studies disaster VGI geolocalization across space, aerial, and ground imagery in multiple disaster scenarios.

- **Cross-view geolocalization and disaster mapping with street-view and VHR satellite imagery: A case study of Hurricane IAN** — **[ISPRS JPRS 2025](https://doi.org/10.1016/j.isprsjprs.2025.01.003)** [[arXiv](https://arxiv.org/abs/2408.06761)] [[Code](https://github.com/tum-bgd/CVDisaster)] [[Data](https://doi.org/10.14459/2024mp1749324)]
  - Dataset: **CVIAN**; framework: **CVDisaster**. Contains 4,121 paired street-view and overhead images after Hurricane Ian, with three damage-severity classes. Supports both cross-view geolocalization and disaster damage assessment.

### Location Mentions in Disaster Text

- **IDRISI-RE: A generalizable dataset with benchmarks for location mention recognition on disaster tweets** — **[Information Processing & Management 2023](https://doi.org/10.1016/j.ipm.2023.103340)** [[Code and Data](https://github.com/rsuwaileh/IDRISI)]
  - Dataset: **IDRISI-RE**. Supports recognition of location mentions in English disaster tweets. Complements image-based cross-view localization with textual geographic evidence.

- **IDRISI-RA: The First Arabic Location Mention Recognition Dataset of Disaster Tweets** — **[ACL 2023 · Main Conference](https://aclanthology.org/2023.acl-long.901/)** [[Code and Data](https://github.com/rsuwaileh/IDRISI)]
  - Dataset: **IDRISI-RA**. Provides Arabic disaster-tweet annotations for location mention recognition, enabling multilingual disaster geolocation research.

- **IDRISI-D: Arabic and English Datasets and Benchmarks for Location Mention Disambiguation over Disaster Microblogs** — **[ArabicNLP 2023](https://aclanthology.org/2023.arabicnlp-1.14/)** [[Code and Data](https://github.com/rsuwaileh/IDRISI)]
  - Dataset: **IDRISI-D**. Links ambiguous location mentions in English and Arabic disaster microblogs to geographic entities.

### Disaster Image & Social-Media Classification

- **LADI v2: Multi-label Dataset and Classifiers for Low-Altitude Disaster Imagery** — **[CVPR 2025 Workshops · EarthVision](https://openaccess.thecvf.com/content/CVPR2025W/EarthVision/papers/Scheele_LADI_v2_Multi-label_Dataset_and_Classifiers_for_Low-Altitude_Disaster_Imagery_CVPRW_2025_paper.pdf)** [[Code](https://github.com/LADI-Dataset/ladi-overview)] [[Data](https://huggingface.co/datasets/MITLL/LADI-v2-dataset)]
  - Dataset: **LADI v2**. Provides roughly 10,000 low-altitude disaster photographs annotated by trained Civil Air Patrol volunteers for multi-label classification, with baseline classifiers. The release identifies this as version 2.

- **MEDIC: a multi-task learning dataset for disaster image classification** — **[Neural Computing and Applications 2023](https://doi.org/10.1007/s00521-022-07717-0)** [[arXiv](https://arxiv.org/abs/2108.12828)] [[Data](https://crisisnlp.qcri.org/medic/)]
  - Dataset: **MEDIC**. Consolidates 71,198 images for disaster type, informativeness, humanitarian category, and damage severity classification. Includes CrisisMMD and other source collections; these are overlapping resources, not disjoint datasets. Published online in 2022; journal issue year 2023.

- **Deep Learning Benchmarks and Datasets for Social Media Image Classification for Disaster Response** — **[IEEE/ACM ASONAM 2020](https://doi.org/10.1109/ASONAM49781.2020.9381294)** [[arXiv](https://arxiv.org/abs/2011.08916)]
  - Consolidates disaster-image resources and benchmarks disaster type, informativeness, and damage severity classification, with duplicate-aware data splits. Also cited as an upstream reference for MEDIC.

- **Damage Identification in Social Media Posts using Multimodal Deep Learning** — **[ISCRAM 2018](https://idl.iscram.org/files/husseinmouzannar/2018/2129_HusseinMouzannar_etal2018.pdf)**
  - Dataset: **Damage Multimodal Dataset (DMD)**. Combines text and images for disaster-related damage identification in social-media posts.

- **CrisisMMD: Multimodal Twitter Datasets from Natural Disasters** — **[ICWSM 2018](https://ojs.aaai.org/index.php/ICWSM/article/view/14983)** [[arXiv](https://arxiv.org/abs/1805.00713)] [[Data](https://crisisnlp.qcri.org/crisismmd)]
  - A multimodal Twitter dataset with image-text annotations from seven major 2017 disasters, supporting humanitarian information classification and response analysis.

- **Damage Assessment from Social Media Imagery Data During Disasters** — **[IEEE/ACM ASONAM 2017](https://doi.org/10.1145/3110025.3110109)**
  - An early disaster-image damage-severity study using deep visual features and event-specific/cross-event evaluation. The associated damage-image collection is one of the sources documented in MEDIC.

### Post-Disaster Recovery

- **Recov-Vision: Linking street view imagery and vision-language models for post-disaster recovery** — **[International Journal of Disaster Risk Reduction (IJDRR) 2026](https://doi.org/10.1016/j.ijdrr.2026.106388)** [[arXiv](https://arxiv.org/abs/2509.20628)] [[Code](https://github.com/YimingXiao98/RecovVision)] [[Data](https://huggingface.co/datasets/Ymx1025/FacadeTrack)]
  - Framework: **Recov-Vision**; data: **FacadeTrack**. Links panoramic street-view video to parcels and rectifies facade views for building-occupancy and recovery assessment. Compares rule-based and LLM-based decision policies across two post-Hurricane Helene surveys.

<a id="qa-semantic"></a>

## Disaster QA, Instruction & Semantic Benchmarks

### Visual Question Answering

- **DisasterVQA: A Visual Question Answering Benchmark Dataset for Disaster Scenes** — **[ICWSM 2026](https://ojs.aaai.org/index.php/ICWSM/article/view/42776)** [[arXiv](https://arxiv.org/abs/2601.13839)] [[Data](https://zenodo.org/records/18267770)]
  - Contains 1,395 real-world images and 4,405 expert-curated questions covering floods, wildfires, earthquakes, hurricanes, fires, and other crisis scenes.

- **VQA-AID: Visual Question Answering for Post-Disaster Damage Assessment and Analysis** — **[IGARSS 2021](https://igarss2021.com/view_paper.php?PaperNum=4387)** [[arXiv](https://arxiv.org/abs/2106.10548)]
  - Introduces the HurMic-VQA dataset collected after Hurricane Michael for UAV-based post-disaster scene understanding.

- **FloodNet: A High Resolution Aerial Imagery Dataset for Post Flood Scene Understanding** — **[IEEE Access 2021](https://doi.org/10.1109/ACCESS.2021.3090981)** [[Code and Data](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021)]
  - Provides high-resolution post-flood UAV imagery for classification, semantic segmentation, and visual question answering.

### Text-Based Question Answering

- **DisastQA: A Comprehensive Benchmark for Evaluating Question Answering in Disaster Management** — **[ACL 2026 Findings](https://aclanthology.org/2026.findings-acl.756/)** [[arXiv](https://arxiv.org/abs/2601.03670)] [[Code](https://github.com/TamuChen18/DisastQA_open)] [[Data](https://huggingface.co/datasets/tamuzc/DisastQA)]
  - Provides 3,000 verified text-based questions (2,000 multiple-choice and 1,000 open-ended) across eight disaster types, constructed from DisastIR. Evaluates 20 models under closed-book, noisy-evidence, and oracle-evidence settings, with keypoint-based scoring for factual completeness.

### Multimodal Instructions & Reasoning

- **DisasterInsight: A Building-Centric Benchmark for Evaluating Vision-Language Models in Disaster Response** — **[ECCV 2026 Workshop · TerraBytes (presented)](https://arxiv.org/abs/2601.18493)** [[Code](https://github.com/sara2227/DisasterInsight-benchmark)]
  - Benchmark: **DisasterInsight**. Enriches xBD building instances with OpenStreetMap functional labels and provides 134,108 instruction records across 15 task types, including building assessment, counting, multi-instance reasoning, and structured reporting. The current release provides code and prompts; benchmark instruction records are planned for a separate release. Earlier versions used the subtitle “A Multimodal Benchmark for Function-Aware and Grounded Disaster Assessment.”

- **Decoding the Disaster: Multi-Task Geospatial Reasoning with Vision-Language Models and Crowdsourced Imagery for Disaster Mapping** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2610.00302)]
  - Framework: **GRDisaster**. Uses a PhotoMappers-derived benchmark of 26,340 images arranged into human-validated VGI, street-view, and remote-sensing triplets spanning disaster events from 2018 to 2024. Combines cross-view geolocalization, multi-view fusion, spatial reasoning, and damage-severity assessment to interpret crowdsourced disaster imagery.

- **DisasterBench: A Multimodal Benchmark for UAV-Based Disaster Response in Complex Environments** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2606.06217)]
  - Benchmark: **DisasterBench (UAV multimodal)**; model: **DisasterVL**. Covers 14 disaster scene types and nine tasks across pre-, during-, and post-disaster analysis. Introduces a lightweight multimodal model with instruction tuning, reasoning alignment, and reinforcement learning.

- **DisasterM3: A Remote Sensing Vision-Language Dataset for Disaster Damage Assessment and Response** — **[NeurIPS 2025 · Datasets and Benchmarks Track](https://proceedings.neurips.cc/paper_files/paper/2025/hash/ec80d18205e39d42a27192d5f3ddd688-Abstract-Datasets_and_Benchmarks_Track.html)** [[Code](https://github.com/Junjue-Wang/DisasterM3)]
  - Offers 26,988 bi-temporal satellite images and 123k instruction pairs from 36 historical events, covering optical/SAR damage assessment and response.

### Change Captioning

- **RSCC: A Large-Scale Remote Sensing Change Caption Dataset for Disaster Events** — **[NeurIPS 2025 · Datasets and Benchmarks Track](https://papers.neurips.cc/paper_files/paper/2025/file/62867024377cac4233195949b9db0ebd-Paper-Datasets_and_Benchmarks_Track.pdf)** [[arXiv](https://arxiv.org/abs/2509.01907)]
  - Contains 62,351 pre/post-event image pairs with human-written change captions for disaster-event interpretation.

### Information Retrieval

- **DisastIR: A Comprehensive Information Retrieval Benchmark for Disaster Management** — **[EMNLP 2025 Findings](https://aclanthology.org/2025.findings-emnlp.97/)** [[arXiv](https://arxiv.org/abs/2505.15856)] [[Code](https://github.com/KaiYin97/Disaster_IR)]
  - Provides 9,600 queries and more than 1.3 million labeled query-passage pairs across 48 retrieval tasks, six search intents, and 301 event types.

<a id="agent-benchmarks"></a>

## Agent Planning & Execution Benchmarks

### Typed-Tool Workflow Planning

- **DisasterBench: Benchmarking LLM Planning under Typed Tool Interface Constraints** — **[EMNLP 2026 Findings (author-confirmed acceptance)](https://yimingxiao98.github.io/)** [[arXiv](https://arxiv.org/abs/2605.27957)] [[Code](https://github.com/TamuChen18/DisasterBench_Open)] [[Data](https://huggingface.co/datasets/tamuzc/DisasterBench)]
  - Benchmark: **DisasterBench (typed-tool planning)**. Contains 233 expert-verified planning tasks, 26 task-interface agents, and 81 typed compatibility edges. Evaluates tool selection, parameter binding, and dependency propagation across five planning paradigms, with **First-Point-of-Failure (FPoF)** diagnostics.

### Operational Geospatial Agents

- **Can LLM Agents Respond to Disasters? Benchmarking Heterogeneous Geospatial Reasoning in Emergency Operations (DORA)** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2605.11633)]
  - Benchmark: **DORA**. Provides 515 expert-authored tasks across 45 events and 10 disaster types, with 3,500 gold tool-call steps and a 108-tool MCP library for geospatial analysis, evacuation planning, and report synthesis.

- **GeoDisaster: Benchmarking Orchestrated Agents for Operational Disaster Geo-Intelligence** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2606.17246)] [[Code](https://github.com/VIMAGE-IITB/GeoDisaster)]
  - Benchmark: **GeoDisaster**. Contains 2,921 verified instances across five operational geospatial task families. Includes an orchestrated multi-agent framework with 18 tools and **Role-Contract Expectation Alignment (RCEA)** for tool use and execution consistency.

<a id="surveys"></a>

## Surveys

- **Survey on Disaster Management Datasets for Remote Sensing-Based Emergency Applications** — **[IEEE TGRS 2026](https://doi.org/10.1109/TGRS.2026.3692760)** [[arXiv](https://arxiv.org/abs/2605.08196)]
  - Reviews image-based datasets for disaster mitigation, preparedness, detection, response, and recovery, covering data accessibility, annotation quality, modalities, and research gaps.

<a id="supporting"></a>

## General-Purpose Supporting Resources

### Remote-Sensing Visual Question Answering

- **RSVLM-QA: A Benchmark Dataset for Remote Sensing Vision Language Model-based Question Answering** — **[ACM MM 2025](https://doi.org/10.1145/3746027.3758235)** [[arXiv](https://arxiv.org/abs/2508.07918)] [[Code](https://github.com/StarZi0213/RSVLM-QA)]
  - Includes 13,820 remote-sensing images and 162,373 VQA pairs with captions, spatial relations, semantic tags, and counting questions.

- **HRVQA: A Visual Question Answering Benchmark for High-Resolution Aerial Images** — **[ISPRS JPRS 2024](https://doi.org/10.1016/j.isprsjprs.2024.06.002)** [[arXiv](https://arxiv.org/abs/2301.09460)] [[Data](https://hrvqa.nl/)]
  - Provides 53,512 aerial images and 1,070,240 question-answer pairs across ten question types; disaster monitoring is one of the target applications.

- **RSVQA: Visual Question Answering for Remote Sensing Data** — **[IEEE TGRS 2020](https://doi.org/10.1109/TGRS.2020.2988782)** [[arXiv](https://arxiv.org/abs/2003.07333)]
  - Establishes an early remote-sensing VQA setting for natural-language interaction with Earth-observation images.

### Geolocation & Cross-View Learning

- **Around the World in 80 Timesteps: A Generative Approach to Global Visual Geolocation** — **[CVPR 2025](https://openaccess.thecvf.com/content/CVPR2025/html/Dufour_Around_the_World_in_80_Timesteps_A_Generative_Approach_to_CVPR_2025_paper.html)** [[Code](https://github.com/nicolas-dufour/plonk)]
  - Method: **PLONK**. Uses generative modeling to estimate global location distributions; supports probabilistic cross-view geolocalization.

- **OpenStreetView-5M: The Many Roads to Global Visual Geolocation** — **[CVPR 2024](https://openaccess.thecvf.com/content/CVPR2024/papers/Astruc_OpenStreetView-5M_The_Many_Roads_to_Global_Visual_Geolocation_CVPR_2024_paper.pdf)** [[Project and Data](https://osv5m.github.io/)]
  - Dataset: **OSV-5M**. Contains over 5.1 million georeferenced street-view images for general visual geolocation.

- **Sample4Geo: Hard Negative Sampling For Cross-View Geo-Localisation** — **[ICCV 2023](https://openaccess.thecvf.com/content/ICCV2023/html/Deuser_Sample4Geo_Hard_Negative_Sampling_For_Cross-View_Geo-Localisation_ICCV_2023_paper.html)** [[Code](https://github.com/Skyy93/Sample4Geo)]
  - Method: **Sample4Geo**. Uses contrastive learning and hard-negative sampling for cross-view retrieval; serves as a geolocalization backbone in CVDisaster.

- **Predicting Ground-Level Scene Layout From Aerial Imagery** — **[CVPR 2017](https://openaccess.thecvf.com/content_cvpr_2017/html/Zhai_Predicting_Ground-Level_Scene_CVPR_2017_paper.html)**
  - Cross-view research associated with **CVUSA**. Learns ground-view semantic layout from co-located overhead imagery and evaluates geolocation and orientation.

<a id="environmental-resources"></a>

## Environmental & Geospatial Resources

- **ERA5** — global atmospheric reanalysis data. [[Data](https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels)]
- **CORDEX** — regional climate model and downscaling data. [[Project](https://cordex.org/)]
- **WRF** — numerical weather simulation framework for event-specific high-resolution meteorological data. [[Project](https://www.mmm.ucar.edu/models/wrf)]
- **WorldPop** — high-resolution gridded population and demographic estimates for population exposure, affected-population estimation, and humanitarian planning. [[Data and project](https://www.worldpop.org/)]
- **MODIS** — Moderate Resolution Imaging Spectroradiometer products for active-fire evidence and burned-area mapping. **MYD14A1** (Aqua daily active-fire product) provides `FireMask` and `MaxFRP`; **MCD64A1** (Terra+Aqua monthly burned-area product) provides `Burn_Date` and `QA`. Download through [NASA Earthdata Search](https://search.earthdata.nasa.gov/search?q=MYD14A1) or search for [MCD64A1](https://search.earthdata.nasa.gov/search?q=MCD64A1) after creating an Earthdata Login; use [AppEEARS](https://appeears.earthdatacloud.nasa.gov/) for spatial/temporal subsetting and selected bands/layers, and the [MODIS data-access tools](https://www.earthdata.nasa.gov/data/instruments/modis/data-access-tools) (including LP DAAC/LAADS direct access) for bulk granule downloads. Product documentation: [MYD14A1 Active Fire User Guide](https://www.earthdata.nasa.gov/s3fs-public/imported/MODIS_Fire_Users_Guide_2.5.pdf) and [MCD64A1 Burned Area User Guide](https://www.earthdata.nasa.gov/s3fs-public/2025-04/MCD64_User_Guide_V61.pdf).
