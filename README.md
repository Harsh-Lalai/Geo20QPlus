# Geo20Q+

Geo20Q+ is a geographically balanced dataset designed to evaluate implicit geographic biases in Large Language Models (LLMs) through a multi-turn deduction game inspired by *20 Questions*. It includes entities of two types—**Notable People** and **Culturally Significant Things**—from diverse regions across the globe. This dataset is introduced in our paper: The World According to LLMs: How Geographic Origin Influences LLMs' Entity Deduction Capabilities

## File Structure

The repository contains the following directory structure:

```text
├── Notable_People/
│   ├── notable_people_raw.csv
│   └── notable_people_processed.csv
├── Things/
│   ├── things_raw.csv
│   └── things_processed.csv
├── README.md
```

---

## Dataset Contents

### `notable_people_processed.csv`

This file contains structured information about notable individuals with the following columns:

- `name`: Name of the individual  
- `gender`: Gender category (e.g., male, female, other)  
- `primary_occupation`: Profession or domain of notability (e.g., politician, athlete)  
- `century`: Century of primary notability (e.g., 20th, 21st)  
- `country`: Country most associated with the individual  

### `things_processed.csv`

This file includes geographically significant non-human entities with the following columns:

- `name`: Name of the entity  
- `category`: Type or domain (e.g., food, landmark, animal)  
- `country`: Country most associated with the entity  

### `notable_people_raw.csv`

This file contains the raw data for notable people, including additional metadata such as birth dates, death dates, occupations, wikipedia views, biographical details etc.

### `things_raw.csv`

This file contains the raw data for culturally significant things including wikipedia links, views etc.

---

## Citation

If you use this dataset or the associated codebase, please cite the following:

```bibtex
@inproceedings{lalai20q,
  title={The World According to LLMs: How Geographic Origin Influences LLMs' Entity Deduction Capabilities},
  author={Lalai, Harsh Nishant and Shah, Raj Sanjay and Pei, Jiaxin and Varma, Sashank and Wang, Yi-Chia and Emami, Ali},
  booktitle={Second Conference on Language Modeling}
}
