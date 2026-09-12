# Machine Learning Journey

A structured repository documenting my journey into Machine Learning - from Python and numerical computing to data manipulation, analysis, visualization, and eventually machine learning models.

This repository is built as a long-term learning record rather than a collection of isolated code snippets. Each section contains practical notebooks, examples, experiments, and notes developed while progressing through the Machine Learning roadmap.

The goal is to understand not only how to use ML libraries, but also the concepts and workflows behind them.

---

## Repository Overview

The repository is organized progressively so that each folder represents a stage of the learning process.

```text
ML/
│
├── 01_NumPy/
│   ├── notebooks/
│   └── ...
│
├── 02_Pandas/
│   ├── datasets/
│   │   ├── subs.csv
│   │   ├── kohli_ipl.csv
│   │   └── bollywood.csv
│   │
│   ├── 1_Pandas_Introduction.ipynb
│   ├── 2_Pandas_Series_Basics.ipynb
│   ├── 3_Pandas_Series_using_read_csv.ipynb
│   ├── 4_Pandas_Series_Methods_and_Maths.ipynb
│   ├── 5_Pandas_Series_Indexing_and_Editing.ipynb
│   ├── 6_Pandas_Series_with_Python_Functionalities_and_Boolean_Indexing.ipynb
│   └── ...
│
└── README.md
```

The repository will continue to expand as new topics are completed.

---

## Current Progress

### 01. NumPy

The first stage focuses on NumPy, which forms an important foundation for numerical computing and later Machine Learning workflows.

Topics covered include:

* NumPy arrays
* Array creation
* Array attributes
* Array operations
* Mathematical operations
* Array manipulation
* Working with dimensions and shapes
* Practical numerical examples

NumPy provides the foundation for understanding how numerical data is represented and processed efficiently in Python.

---

### 02. Pandas

The current stage focuses on Pandas and working with structured data.

Pandas is being learned from the fundamentals while gradually moving toward practical data analysis workflows.

Current topics include:

#### Pandas fundamentals

* Introduction to Pandas
* Series
* DataFrames
* Creating Series
* Series attributes
* Reading CSV datasets

#### Series operations

* Series methods
* Sorting
* `head()`
* `tail()`
* `sample()`
* `value_counts()`
* Mathematical operations
* Statistical methods
* Descriptive statistics

#### Series indexing and manipulation

* Positive indexing
* Negative positional indexing
* `.iloc`
* `.loc`
* Slicing
* Fancy indexing
* Editing Series values
* Index-based operations

#### Python functionality with Series

* `len()`
* `type()`
* `dir()`
* `sorted()`
* `max()`
* `min()`
* Type conversions
* Membership operators
* Looping through values and indexes
* Arithmetic operators
* Broadcasting
* Relational operators

#### Boolean indexing

* Conditional filtering
* Boolean Series
* Filtering using conditions
* Multiple conditions
* Counting matching values
* Practical data filtering

#### Data visualization

* Plotting Series
* Line graphs
* Bar graphs
* Visualizing trends in data

---

## Datasets

The Pandas section currently uses small real-world datasets to make the learning process more practical.

### `subs.csv`

Contains subscriber growth data.

```text
Subscribers gained
```

Used for practicing Series operations, statistics, and visualization.

### `kohli_ipl.csv`

Contains Virat Kohli's IPL match-wise runs.

```text
match_no
runs
```

Used for indexing, filtering, mathematical operations, Boolean indexing, and visualization.

### `bollywood.csv`

Contains Bollywood movie and lead actor information.

```text
movie
lead
```

Used primarily for working with categorical/string data and Series operations such as `value_counts()`.

---

## Learning Approach

The repository follows a progression from fundamentals to practical Machine Learning workflows.

```text
Python
   │
   ▼
NumPy
   │
   ▼
Pandas
   │
   ▼
Data Cleaning & Analysis
   │
   ▼
Data Visualization
   │
   ▼
Machine Learning
   │
   ▼
Model Evaluation
   │
   ▼
Advanced ML Concepts
```

The focus at each stage is on understanding the underlying concepts before moving to higher-level abstractions.

---

## Notebook Philosophy

The notebooks are intentionally written as personal learning notes.

Each notebook generally follows this structure:

```text
Concept
   ↓
Simple Explanation
   ↓
Code Example
   ↓
Output / Observation
   ↓
Practical Usage
   ↓
ML Relevance
```

Examples are kept practical and readable instead of relying only on theoretical explanations.

Where appropriate, important concepts are highlighted based on their relevance to Machine Learning.

---

## Tech Stack

The repository currently uses:

```text
Python
NumPy
Pandas
Matplotlib
Jupyter Notebook
```

Additional tools and libraries will be introduced as the Machine Learning journey progresses.

---

## Roadmap

The repository is a work in progress.

The broader roadmap is expected to progress through areas such as:

```text
Python Fundamentals
        ↓
NumPy
        ↓
Pandas
        ↓
Data Cleaning
        ↓
Data Analysis
        ↓
Data Visualization
        ↓
Machine Learning Fundamentals
        ↓
Supervised Learning
        ↓
Unsupervised Learning
        ↓
Model Evaluation
        ↓
Feature Engineering
        ↓
Machine Learning Projects
        ↓
Advanced Topics
```

Only the completed portions of the roadmap will be added to the repository as the journey progresses.

---

## Purpose of This Repository

This repository serves three purposes:

1. **Learning** - building a strong conceptual foundation in Machine Learning.

2. **Documentation** - maintaining a structured record of concepts, experiments, and progress.

3. **Reference** - creating a personal knowledge base that can be revisited during projects, interviews, and future learning.

The repository is not intended to represent a finished Machine Learning curriculum. It is an evolving record of the learning process.

---

## Progress

Current focus:

```text
NumPy       → Completed / Practicing
Pandas      → In Progress
Machine Learning → Upcoming
```

Progress will be updated as new sections are completed.

---

## Repository Status

This repository is actively evolving.

New notebooks, datasets, experiments, projects, and concepts will be added progressively as I continue through the Machine Learning roadmap.
