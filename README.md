# SwahBERT
Is a pretrained monolingual language model for Swahili. <br>
The model was trained for 800K steps using a corpus of 105MB that was collected from news sites, online discussion, and Wikipedia. <br>
The evaluation was perfomed on several downstream tasks such as emotion classification, news classification, and Named entity recognition.


## Pre-training Corpus
The text was extracted from different sorces;<br>
 - News sites: `United Nations news, Voice of America (VoA), Deutsche Welle (DW) and taifaleo`<br>
 - Forums: `JaiiForum`<br>
 - ``Wikipedia``.

## Pre-trained Models
`SwahBERT-Base, Uncased` <br>
`SwahBERT-Base, Cased`

Steps | vocab size | MLM acc | NSP acc | loss |
--- | --- | --- | --- | --- |
800K | 32K (uncased) | 73.37 | 99.50 | 1.1822 | 
**800K** | **50K (uncased)** | **76.54** | **99.67** | **1.0667** |
800K | 70K (uncased) | 73.38 | 100.0 | 1.2131 | 
**800K** | **32K (cased)** | **76.94** | **99.33** | **1.0562** | 
1M | 32K (cased) | 73.81 | 98.17 | 1.2732 |


## Evaluation
The model was tested on four downstream tasks including our new emotion dataset                                                                                                                                                                                         

F1-score of language models on downstream tasks 
Tasks | SwahBERT | SwahBERT_cased | mBERT |                        
--- | --- | --- | --- |
Emotion | 64.46 | 64.77 | 60.52 | 
News | 90.90 | 89.90 | 89.73 |
Sentiment | 70.94 | 71.12 | 67.20 |
NER | 88.50 | 88.60 | 89.36 |



