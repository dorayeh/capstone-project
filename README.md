# capstone-team-29

# Image-to-text Model for Social Media Network Analysis

Code for the image-to-text model to generate captions and entities from social media content.
  
## Files

  * ```amazon-rekognition.ipynb``` -- code to send images to Amazon cloud-based image and video analysis service.
  * ```amazon_rekognition_on_nodexl_query.ipynb``` -- code to extract image-to-text labels from NodeXL sample file.
  * ```blip2-opt-2_7b.ipynb``` -- code to run BLIP  (Bootstrapping Language Image Pre-training) model for visual question answering.
  * ```kosmos-2-patch14-224.ipynb``` -- code to run image processor and tokenizer.
  * ```network_analysis_on_nodexl_data.ipynb``` -- code for generating networks from image-to-text data
  * ```model_evaluation_kosmos.ipynb``` -- code for generating networks from image-to-text data
  * ```model_evaluation_blip2.ipynb``` -- code for generating networks from image-to-text data
  * ```model_evaluation_AWS.ipynb``` -- code for generating networks from image-to-text data
    
## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [References](#references)

## Installation

Instructions on how to install and set up the project.

  * ```annotations.zip``` -- link to download the [annotations file](https://vizwiz.cs.colorado.edu/VizWiz_final/caption/annotations.zip) with 117,155 training captions; 40,000 test captions; and 38,750 validation captions in JSON format.
  * ```train.zip``` -- link to download the [train dataset](https://vizwiz.cs.colorado.edu/VizWiz_final/images/train.zip) with 23,431 images in .jpg format. 
  * ```test.zip```  -- link to download the [test dataset](https://vizwiz.cs.colorado.edu/VizWiz_final/images/test.zip) with 8,000 images .jpg format. 
  * ```val.zip``` -- link to download the [validations dataset](https://vizwiz.cs.colorado.edu/VizWiz_final/images/val.zip) with 7,750 images .jpg format.
  * ```NodeXLWorkbook-294548.xlsx``` --link to download the [social media sample dataset from X (former Twitter)](https://nodexlgraphgallery.org/Pages/Workbook.ashx?graphID=294548) from the Node XL Graph gallery from the Social Media Research Foundation.

## Usage

Clone the Repository:
git clone https://github.com/yourusername/capstone-team-29.git

Open the Notebook:Navigate to the cloned repository on your local machine.
    Open the .ipynb file in Google Colab.

Run the Notebook:

    Follow the instructions within the notebook to execute the code.
    Make sure to install any required dependencies specified in the notebook.

## Credits

We extend our sincere appreciation to the [Social Media Research Foundation](https://www.smrfoundation.org/) and [Nodel XL Team](https://nodexl.com/) for their invaluable support and resources.

## References 

- [VizWiz Project](http://vizwiz.org)
- BLEU: [BLEU: a Method for Automatic Evaluation of Machine Translation](http://www.aclweb.org/anthology/P02-1040.pdf)
