# capstone-team-29

# Image-to-text Model for Social Media Network Analysis

Code for the image-to-text model to generate captions and entities from social media content.

## Requirements

      <review with Jerry> e.g. AWS requirements and *used libraries*!
  import boto3<br />
  import jsonimport requests<br />
  import nltk<br />
  from nltk.corpus import stopwords<br />
  from PIL import Image<br />
  from transformers import AutoProcessor, AutoModelForVision2Seq<br />
  from PIL import Image<br />
  import requests<br />
  from transformers import Blip2Processor, Blip2ForConditionalGeneration<br />
  import torch<br />
  import pandas as pd<br />
  import networkx as nx<br />
  from itertools import combinations<br />
  
## Files

  * > review ```amazon-rekognition.ipynb``` -- code to send images to Amazon cloud-based image and video analysis service.
  * > review ```amazon_rekognition_on_nodexl_query.ipynb``` -- code to extract image-to-text labels from NodeXL sample file.
  * ```blip2-opt-2_7b.ipynb``` -- code to run BLIP  (Bootstrapping Language Image Pre-training) model for visual question answering.
  * ```kosmos-2-patch14-224.ipynb``` -- code to run image processor and tokenizer.
  * ```network_analysis_on_nodexl_data.ipynb``` -- code for generating networks from image-to-text data

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
  * ```NodeXLWorkbook-294548.xlsz``` --link to download the [social media sample dataset from X (former Twitter)](https://nodexlgraphgallery.org/Pages/Workbook.ashx?graphID=294548) from the Node XL Graph gallery from the Social Media Research Foundation.

## Usage

Guidance on how to use the project, including examples or code snippets.

## Credits

We extend our sincere appreciation to the [Social Media Research Foundation](https://www.smrfoundation.org/) and [Nodel XL Team](https://nodexl.com/) for their invaluable support and resources.

## References 

- [VizWiz Project](http://vizwiz.org)
- PTBTokenizer: We use the [Stanford Tokenizer](http://nlp.stanford.edu/software/tokenizer.shtml) which is included in [Stanford CoreNLP 3.4.1](http://nlp.stanford.edu/software/corenlp.shtml).
- BLEU: [BLEU: a Method for Automatic Evaluation of Machine Translation](http://www.aclweb.org/anthology/P02-1040.pdf)
- Meteor: [Project page](http://www.cs.cmu.edu/~alavie/METEOR/) with related publications. We use the latest version (1.5) of the [Code](https://github.com/mjdenkowski/meteor). Changes have been made to the source code to properly aggreate the statistics for the entire corpus.
- Rouge-L: [ROUGE: A Package for Automatic Evaluation of Summaries](http://anthology.aclweb.org/W/W04/W04-1013.pdf)
- SPICE: [SPICE: Semantic Propositional Image Caption Evaluation](https://arxiv.org/abs/1607.08822)
