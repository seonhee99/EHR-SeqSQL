# EHR-SeqSQL : A Sequential Text-to-SQL Dataset For Interactively Exploring Electronic Health Records
Official repository of [EHR-SeqSQL : A Sequential Text-to-SQL Dataset For Interactively Exploring Electronic Health Records](https://arxiv.org/abs/2406.00019) (ACL 2024 Findings)


## Overview
We introduce EHR-SeqSQL, a novel sequential text-to-SQL dataset for Electronic Health Record (EHR) databases. EHR-SeqSQL is designed to address critical yet underexplored aspects in text-to-SQL parsing: interactivity, compositionality, and efficiency. 
To the best of our knowledge, EHR-SeqSQL is not only the largest but also the first medical text-to-SQL dataset benchmark to include sequential and contextual questions. We provide a data split and the new test set designed to assess compositional generalization ability. With EHR-SeqSQL, we aim to bridge the gap between practical needs and academic research in the text-to-SQL domain.


## Dataset
The `data.json` file contains the following fields:

- `seed_question` : The original question from EHRSQL dataset.
- `value` : Sampled values from the database.
- `question` : Paraphrased version of the question sequences.
- `question_template` : The original template question sequences.
- `seqsql` : Our version of SQL query sequences with special tokens.
- `sql` : Executable SQL query sequences without special tokens.
- `random_split` : Whether the sample is for 'train' or 'test' in the random split.
- `compositional_split` : Whether the sample is for 'train' or 'test' in the compositional split.

`id`, `department`, and `importance` fields keeps the same value with the corresponding EHRSQL data sample.


## Citation
When you use the this dataset, we would appreciate it if you cite our paper:
```
@article{ryu2024ehr,
  title={EHR-SeqSQL: A Sequential Text-to-SQL Dataset For Interactively Exploring Electronic Health Records},
  author={Ryu, Jaehee and Cho, Seonhee and Lee, Gyubok and Choi, Edward},
  journal={arXiv preprint arXiv:2406.00019},
  year={2024}
}
```
