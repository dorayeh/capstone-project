# capstone-team-29

# Image-to-text Model for Social Media Network Analysis

Code for the image-to-text model to generate captions, entities, and/or labels from social media content to enhance network analysis applications.
  
## Files

  <!-- * ```amazon-rekognition.ipynb``` -- send images to Amazon cloud-based image and video analysis service <update> -->
  * ```blip2-opt-2_7b.ipynb``` -- run BLIP (Bootstrapping Language Image Pre-training) model for visual captioning
  * ```kosmos-2-patch14-224.ipynb``` -- run visual captioning and entities extraction tasks using Kosmos-2
  * ```model_evaluation_kosmos.ipynb``` -- generate the evaluation scores against the groundtruth captions from VizWiz for Kosmos-2 model
  * ```model_evaluation_blip2.ipynb``` -- generate the evaluation scores against the groundtruth captions from VizWiz for BLIP-2 model
  * ```model_evaluation_AWS.ipynb``` -- send images to Amazon cloud-based image and video analysis service and generate the evaluation scores against the groundtruth captions from VizWiz for Rekognition model
  * ```amazon_rekognition_on_nodexl_query.ipynb``` -- code to extract image-to-text labels from NodeXL sample file
  * ```network_analysis_on_nodexl_data.ipynb``` -- code for generating networks from image-to-text data
  * ```blip2_val_outputs.csv``` -- .csv file with the outputs from BLIP-2 model on each image ID from the VizWiz validation dataset (val.zip)
  * ```kosmos_val_outputs.csv``` -- .csv file with the outputs from Kosmos-2 model on each image ID from the VizWiz validation dataset (val.zip)
  * ```rekognition_val_outputs.csv``` -- .csv file with the outputs from Amazon Rekognition model on each image ID from the VizWiz validation dataset (val.zip)
  * ```BLEU_val_baseline_scores.json``` -- baseline results for the tokenized captions from VizWiz using BLEU score
  * ```NodeXL_tweets_labels.csv``` -- .csv file with the outputs from Amazon Rekognition on a sample file for application purposes
    
## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [References](#references)

## Installation

All the files necessary for running the codes are within the repository. Ensure that you have access to the repository containing the code files. The code provided assumes that you have the necessary permissions to access the specified directory (/content/drive/My Drive/Colab Notebooks). Modify the folder_path variable if your directory structure is different.

In case you encounter difficulty in extracting or accessing the files in the repository, direct download links are provided for your convenience. Simply use these links to download the required files directly to your system. This ensures that you can access the necessary files without relying on repository access.

  * ```annotations.zip``` -- link to download the [annotations file](https://vizwiz.cs.colorado.edu/VizWiz_final/caption/annotations.zip) with 117,155 training captions; 40,000 test captions; and 38,750 validation captions in JSON format.
  * ```val.zip``` -- link to download the [validations dataset](https://vizwiz.cs.colorado.edu/VizWiz_final/images/val.zip) with 7,750 images .jpg format.
  * ```NodeXLWorkbook-294548.xlsx``` --link to download the [social media sample dataset from X (former Twitter)](https://nodexlgraphgallery.org/Pages/Workbook.ashx?graphID=294548) from the Node XL Graph gallery from the Social Media Research Foundation.
  <!---* ```train.zip``` -- link to download the [train dataset](https://vizwiz.cs.colorado.edu/VizWiz_final/images/train.zip) with 23,431 images in .jpg format. 
  * ```test.zip```  -- link to download the [test dataset](https://vizwiz.cs.colorado.edu/VizWiz_final/images/test.zip) with 8,000 images .jpg format.--->

## Usage

1. Clone the Repository:
    ```git clone https://github.com/vgaquino/capstone-team-29.git```

2. Open the Notebook and navigate to the cloned repository on your local machine.
    Open the respective .ipynb files in Google Colab.

3. Check if the default directory exists for the file paths. You may create it running the ```'requirements.txt'```:

4. Follow the instructions within the notebooks to execute the code.

## Credits

We extend our sincere appreciation to the [Social Media Research Foundation](https://www.smrfoundation.org/) and [Nodel XL Team](https://nodexl.com/) for their invaluable support and resources.

## References 

- [VizWiz Project](http://vizwiz.org)
- [BLEU: a Method for Automatic Evaluation of Machine Translation](http://www.aclweb.org/anthology/P02-1040.pdf)
- [Kosmos-2: Grounding Multimodal Large Language Models to the World paper](https://arxiv.org/abs/2306.14824)
