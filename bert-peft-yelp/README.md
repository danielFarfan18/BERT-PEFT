---
base_model: nlptown/bert-base-multilingual-uncased-sentiment
library_name: peft
---

# Model Card for Model ID

<!-- Provide a quick summary of what the model is/does. -->



## Model Details

### Model Description

<!-- Provide a longer summary of what this model is. -->



- **Developed by:** Marcos Daniel Rodríguez Farfán
- **Model type:** BERT
- **Language(s) (NLP):** English


## Training Details

### Training Data
#### **Dataset summary**
**Source Data:**  
The [Yelp reviews dataset](https://huggingface.co/datasets/Yelp/yelp_review_full) consists of reviews from Yelp. It is extracted from the Yelp Dataset Challenge 2015 data.

**Languages**  
The reviews were mainly written in english.

#### **Dataset Structure**

**Data Instances**
A typical data point, comprises of a text and the corresponding label.

**Data Fields**
The simplified configuration includes:

- `text`: The review texts are escaped using double quotes ("), and any internal double quote is escaped by 2 double quotes (""). New lines are escaped by a backslash followed with an "n" character, that is "\n".
- `labels`: Corresponds to the score associated with the review (between 1 and 5).

### Training Procedure

<!-- This relates heavily to the Technical Specifications. Content here should link to that section when it is relevant to the training procedure. -->

#### Preprocessing [optional]

[More Information Needed]


#### Training Hyperparameters

- **Training regime:** [More Information Needed] <!--fp32, fp16 mixed precision, bf16 mixed precision, bf16 non-mixed precision, fp16 non-mixed precision, fp8 mixed precision -->


## Evaluation

<!-- This section describes the evaluation protocols and provides the results. -->

### Testing Data, Factors & Metrics

#### Testing Data

<!-- This should link to a Dataset Card if possible. -->

[More Information Needed]

#### Factors

<!-- These are the things the evaluation is disaggregating by, e.g., subpopulations or domains. -->

[More Information Needed]

#### Metrics

<!-- These are the evaluation metrics being used, ideally with a description of why. -->

[More Information Needed]


### Compute Infrastructure

[More Information Needed]

#### Hardware
RTX3060Ti


## Model Card Contact

[More Information Needed]
### Framework versions

- PEFT 0.12.0
