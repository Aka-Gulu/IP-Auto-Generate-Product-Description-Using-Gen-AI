# Leveraging Machine Learning to Generate Product Descriptions in E-Commerce

## Poster, Video, and Slides
[Informs Poster](https://drive.google.com/file/d/1yekXjOYnutCOly8biY2lJDNcpdmfsBSC/view?usp=sharing) 

[Video link](https://www.youtube.com/watch?v=-NZrAbjYpI0)

[Slides link](https://drive.google.com/file/d/116Z8WlMbDiDxIqi1Ipx5Bb_vrOMTbMxJ/view?usp=sharing)

## Introduction
This project aims to tackle the challenge of automating online retail product descriptions using state-of-the-art machine learning models. We collaborated with a nationwide grocery store chain in the US to improve the quality and efficiency of product listings on their online platform. Our solution focuses on two main tasks: capturing information from product images and refining auto-generated product descriptions. The deployment of these models in a scalable Azure pipeline demonstrates significant potential for reducing operational costs and enhancing customer satisfaction.

## Objectives
- **Image-to-Text Task:** Utilize `Optical Character Recognition (OCR)` and image captioning to extract information from product images.
- **Text-to-Text Task:** Refine and enhance auto-generated product descriptions.
- **Scoring:** Measure the generated text based on relevance, completeness, readability, and confidence using a scoring model.

## Data
The dataset provided by a major grocery store chain comprises 309,826 unique products spanning diverse categories. The original datasets cannot be shared because of `Non-Disclosure Agreement`.

## Methodology
### 1. Analytics Problem Framing
Our team identified the need for automating product description generation due to non-compliance and inadequate submissions from vendors. The objective was to enhance the scalability and automation of the process using machine learning.

### 2. Model Building
We evaluated several `image-to-text models (BLIP, Git-Large-Coco, LLAMA 2, Mixtral)` and selected the best-performing model based on human evaluations. Text-to-text models were then used to refine the descriptions.

### 3. Deployment & Life Cycle Management
An `Azure pipeline` was developed to automate the entire process:
- **Blob Storage:** Product information in CSV format is uploaded.
- **Functions:** File triggers feed data into machine learning models for action.
- **Machine Learning:** Generates product descriptions and scores.
- **Blob Storage:** Generated content and scores are saved in CSV files.

### 4. Scoring
We utilized `Large Language Models (LLMs)` to score the generated results based on relevance, completeness, readability, and confidence. The scoring algorithm demonstrated an increase in average quality score by more than 76% compared to vendor-provided descriptions.

## Results
- **100% high-quality product descriptions**
- **99% reduction in original labor time and costs**
- **76% average quality score for generated descriptions**

## Impact
Our project has shown promising results in reducing operational costs, enhancing customer satisfaction, and boosting profitability for the retailer. The methodology and pipeline have potential applications across various industries, such as consumer goods.

## Team
- Goutham Kumar Vemasani
- Harish Datta Chitneni
- Harthik Miriyala
- Jinxin Ren
- Srujana Kalyadapu
- Yu-hui Lin
- Dr. Matthew A. Lanham
- Dr. Mark Tabladillo

## Acknowledgements
We would like to thank Professor Matthew Lanham and Dr. Mark Tabladillo from Microsoft for their guidance and support on this project.
