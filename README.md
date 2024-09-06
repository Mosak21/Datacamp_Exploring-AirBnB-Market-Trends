# New York City Airbnb Market Analysis

## Project Overview

Welcome to the analysis of Airbnb listings in **New York City**, one of the most popular tourist destinations globally. Given the high demand for short-term rentals, Airbnb listings in NYC play a significant role in providing accommodation for travelers. In this project, we aim to take a closer look at the Airbnb market in NYC, focusing on various aspects such as pricing, location, room type, and host reviews. We will analyze this data using three datasets in different formats (.csv, .xlsx, and .tsv) and combine them to gain deeper insights into the market.

## Datasets Used

This project uses the following three datasets that contain information about Airbnb listings in New York City:

1. **airbnb_price.csv** (CSV File)
   - This file contains data about the pricing and location of Airbnb listings.
   
   | Column Name  | Description                                       |
   |--------------|---------------------------------------------------|
   | `listing_id` | Unique identifier for each Airbnb listing          |
   | `price`      | Nightly price of the listing (in USD)              |
   | `nbhood_full`| Borough and neighborhood where the listing is located |

2. **airbnb_room_type.xlsx** (Excel File)
   - This file provides descriptions and room type information for Airbnb listings.
   
   | Column Name  | Description                                        |
   |--------------|----------------------------------------------------|
   | `listing_id` | Unique identifier for each Airbnb listing          |
   | `description`| A brief description of the listing                 |
   | `room_type`  | Type of room offered: shared, private, or entire home/apartment |

3. **airbnb_last_review.tsv** (TSV File)
   - This file includes data about the host names and the last review date for each Airbnb listing.
   
   | Column Name  | Description                                       |
   |--------------|---------------------------------------------------|
   | `listing_id` | Unique identifier for each Airbnb listing          |
   | `host_name`  | Name of the host managing the listing              |
   | `last_review`| Date when the listing was last reviewed by a guest |

## Objectives

The goal of this project is to combine the data from these three files and answer key questions about the Airbnb market in New York City. By analyzing data on listing prices, room types, descriptions, and reviews, we will gain insights that could help Airbnb hosts and potential guests make informed decisions.

### Key Questions:
- How do Airbnb prices vary across different neighborhoods and boroughs in NYC?
- What types of rooms are most common, and how do they influence pricing?
- How frequently are Airbnb listings being reviewed by guests?

## Installation

To run this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/nyc-airbnb-market-analysis.git
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

Once you have the necessary packages installed, you can start exploring the data using the provided Jupyter notebook (`airbnb_analysis.ipynb`).

### Example Usage:
```python
import pandas as pd

# Load the datasets
price_data = pd.read_csv('data/airbnb_price.csv')
room_data = pd.read_excel('data/airbnb_room_type.xlsx')
review_data = pd.read_csv('data/airbnb_last_review.tsv', sep='\t')

# Example: Display the first few rows of the price data
print(price_data.head())
```

## Conclusion

This project combines multiple file types to analyze the NYC Airbnb market and answer questions about pricing, room types, and reviews. The insights drawn from this analysis can inform both hosts and guests about trends and patterns in the market.

---

Feel free to explore further and contribute to the project.
