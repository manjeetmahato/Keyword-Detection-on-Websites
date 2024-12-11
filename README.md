# Keyword Detection on Websites - Tumor Board Detection

This project involves developing an algorithm that takes an HTML page as input and determines whether the page contains information about cancer tumor boards. A tumor board is a group of doctors from different disciplines discussing cancer cases. The task is to predict whether the page discusses tumor boards and, if so, to classify the level of detail about the tumor board and potentially identify the type and schedule.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Feature Engineering](#feature-engineering)
- [Model](#model)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
The project takes HTML files and classifies them into one of three categories based on the presence and detail of tumor board information:
1. **No Evidence (1)**: No mention of tumor boards.
2. **Medium Confidence (2)**: Tumor boards are mentioned, but not the focus of the page.
3. **High Confidence (3)**: The page is dedicated to tumor board details, including types and schedules.

Additionally, the project explores detecting tumor board types (e.g., interdisciplinary, breast) and their schedules (e.g., days, frequency, time).

## Dataset
The dataset includes the following files:

- **train.csv**: Contains columns `url`, `doc_id`, and `label` for training.
- **test.csv**: Contains columns `url` and `doc_id` for testing.
- **htmls**: Folder containing `.html` files with the content corresponding to `doc_id`.
- **keyword2tumor_type.csv**: Contains keywords for different tumor board types.

**Tumor Board Labels**:
- `1`: No evidence of tumor boards.
- `2`: Medium confidence; tumor boards are mentioned, but not the main focus.
- `3`: High confidence; page is dedicated to tumor board details.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/tumor-board-detection.git
