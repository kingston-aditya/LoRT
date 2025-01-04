# LoRT: Logical Reasoning Evaluation Suite for Transformers

This repository contains the LoRT dataset that was created for CMSC 828J course offered at University of Maryland, Colege Park. It was developed by Wenshan Wu, Aditya Sarkar and Jenny Yarmovsky. 

Full details about the project can be found in our technical report: [LoRT: Logical Reasoning Evaluation Suite for Transformers](https://github.com/ws500981/LoRT/tree/main/report)

## Introduction
**LoRT** is a large, manually-curated set of CommonsenseQA-style questions for probing logical reasoning capabilities in Language models especially the transformer based models. 

All questions were written in **English**.

## Dataset
The dataset is released in both `JSON` and `CSV` formats. It can be found in `~/LoRT/data/` directory. LoRT contains around `110K` CommmonsenseQA-style questions. 

The following is an example entry from LoRT:
```
{
  "Given {A} contradicts {B}, does {A} forward entail {B}?",
    "No"
}
```
A description of the fields is given below:
* `A`: the first word. It can be real or synthetic.
* `B`: the second word. It can be real or synthetic.
* `No`: the answer to the entailment question asked.

## How to run the scripts
```
    git clone https://github.com/ws500981/LoRT.git
    pip install requirements.txt
    cd ~/LoRT/scripts
    # for SynLoRT - numbers
    python get_data.py 25000 4 4 0 0 
```

## License
This project is licensed under the MIT License.

## Citation
If you use this dataset, please cite the following paper:
```
@inproceedings{wu-sarkar-yarmovsky-2024-lort,
    title = "{LoRT}: Logical Reasoning Evaluation Suite for Transformers",
    author = "Wu, Wenshan, Sarkar, Aditya  and Yarmovsky, Jenny",
    booktitle = "Course Project for CMSC 828J",
    month = dec,
    year = "2024",
    address = "College Park, US"
}
```
PS: This repo will be legend - wait for it - ary.. legendary!
