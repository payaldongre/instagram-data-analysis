# Coders of Bangalore – Instagram Data Pipeline

A Python-based data processing pipeline developed using **Jupyter Notebook**. This project parses unstructured Instagram profile data, converts it into structured JSON format, and performs basic exploratory data analysis (EDA) on the processed dataset.

---

## Project Objectives

- Build a pipeline to process raw Instagram profile data.
- Parse unstructured text into structured records.
- Convert follower and following counts (K/M) into numeric values.
- Generate a structured JSON dataset from the parsed data.
- Perform exploratory data analysis on the generated dataset.

---

## Technologies Used

- Python
- Jupyter Notebook
- JSON

---
## Dependencies

This project uses only Python's standard library (`json`) and does not require any additional Python packages.

## Project Structure

```text
02_coders-of-bangalore/
│
├── coders-of-bangalore-pipeline.ipynb   # Data parsing and JSON generation
├── coders-of-bangalore.ipynb            # Exploratory data analysis
│
├── initialdata.txt                      # Dataset used during pipeline development
├── finaldata.txt                        # Final dataset processed by the pipeline
├── data.json                            # Generated structured JSON dataset
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Workflow

### Phase 1 – Pipeline Development

The parsing pipeline was initially developed using **`initialdata.txt`** to understand the structure of raw Instagram profile data.

---

### Phase 2 – Pipeline Integration

The same parsing pipeline was then applied to **`finaldata.txt`**, which contains the complete dataset.

For each Instagram profile, the following information is extracted:

- Username
- Number of Posts
- Number of Followers
- Number of Following
- Name
- Page Category (Type of Page)
- Bio

Follower and following counts containing **K (thousand)** and **M (million)** suffixes are automatically converted into integer values.

---

### Phase 3 – JSON Generation

After parsing all profiles, the extracted records are converted into structured JSON format and stored in:

```text
data.json
```

---

### Phase 4 – Exploratory Data Analysis

The generated JSON dataset is analyzed to identify:

- User with the maximum number of posts
- User with the maximum number of followers
- User with the maximum number of following
- Total number of unique page categories
- List of all page categories

---

## Running the Project

1. Open a terminal (or Anaconda Prompt).

2. Navigate to the project directory:

```bash
cd /d "D:\DataScience_Notes\DS_PR\02_coders-of-bangalore"
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Run the notebooks in the following order:

1. `coders-of-bangalore-pipeline.ipynb`
2. `coders-of-bangalore.ipynb`

---

## Files

| File | Description |
|------|-------------|
| `initialdata.txt` | Raw dataset used during initial pipeline development |
| `finaldata.txt` | Final dataset processed through the pipeline |
| `data.json` | Generated structured JSON dataset |
| `coders-of-bangalore-pipeline.ipynb` | Parses raw Instagram profile data and generates `data.json` |
| `coders-of-bangalore.ipynb` | Performs exploratory data analysis on the generated dataset |

---

## Features

- Raw text parsing
- Structured JSON generation
- Automatic conversion of K/M values to integers
- Data serialization using JSON
- Basic exploratory data analysis (EDA)

---

## Future Enhancements

- Export processed data to CSV
- Data visualization using Matplotlib or Seaborn
- Interactive dashboard for profile analytics
- Additional statistical analysis on user engagement

---

## Author

**Payal Dongre**  
B.Tech Computer Science & Engineering