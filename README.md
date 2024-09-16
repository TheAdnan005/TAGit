
# Product Entity Extraction from Images

## Overview

This project focuses on developing a machine learning model to extract and predict product entity values (e.g., weight, volume, voltage) from product images. This solution is crucial for digital marketplaces, where accurate product information is essential for listing products effectively.

## Problem Statement

The challenge is to create a model that extracts key product details from images and formats these details into a specific format. The output should match the allowed units and format as described in the problem statement.

## Data Description

The dataset includes:

- `dataset/train.csv`: Contains labeled training data with columns:
  - `index`: Unique identifier for each sample.
  - `image_link`: URL of the product image.
  - `group_id`: Category code of the product.
  - `entity_name`: Name of the product entity (e.g., "item_weight").
  - `entity_value`: Value of the product entity (e.g., "34 gram").

- `dataset/test.csv`: Contains test data without `entity_value`. Used for generating predictions.
  - `index`: Unique identifier for each sample.
  - `image_link`: URL of the product image.
  - `group_id`: Category code of the product.
  - `entity_name`: Name of the product entity.

- `dataset/sample_test.csv`: Example test input file for reference.
- `dataset/sample_test_out.csv`: Example output file showing the expected format.

## Setup

### Prerequisites

- Python 3.x
- Required Python packages:
  - `paddlepaddle`
  - `paddleocr`
  - `opencv-python`
  - `numpy`
  - `pandas`
  - `requests`
  - `csv`
  - `logging`

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/your-repository.git
   cd your-repository
