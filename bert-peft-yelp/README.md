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
`   learning_rate=1e-3,
    per_device_train_batch_size=16,
    per_device_eval_batch_size=16,
    num_train_epochs=2,
    weight_decay=0.01,
    evaluation_strategy="steps",
    save_strategy= 'steps',
    push_to_hub= True,
    resume_from_checkpoint=True,
    load_best_model_at_end=True`


### Compute Infrastructure

#### Hardware
GPU: RTX3060Ti


## Model Card Contact

[More Information Needed]
### Framework versions

- PEFT 0.12.0
