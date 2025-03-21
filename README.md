# MERN Stack Coding Challenge

## Overview

This is a MERN stack application designed to manage and analyze product transactions. The backend fetches data from a third-party API and initializes the database. It also provides several APIs to retrieve transactions, generate statistics, and create charts. The frontend uses these APIs to display transaction data, statistics, and charts.

## Backend Task

### Data Source

- **THIRD PARTY API URL:** `https://s3.amazonaws.com/roxiler.com/product_transaction.json`
- **REQUEST METHOD:** `GET`
- **RESPONSE FORMAT:** `JSON`

### APIs

#### 1. Initialize Database

Fetches JSON data from the third-party API and initializes the database with seed data.

#### 2. List Transactions

- **Endpoint:** `GET /api/transactions`
- **Parameters:** `month`, `search` (optional), `page` (optional), `perPage` (optional)
- **Description:** Lists all transactions for a given month with support for search and pagination.
- **Search:** Matches search text on product title, description, or price.

#### 3. Get Statistics

- **Endpoint:** `GET /api/statistics`
- **Parameters:** `month`
- **Description:** Provides statistics for the selected month including:
  - Total sale amount
  - Total number of sold items
  - Total number of not sold items

#### 4. Bar Chart Data

- **Endpoint:** `GET /api/bar-chart`
- **Parameters:** `month`
- **Description:** Provides data for a bar chart displaying price ranges and the number of items in each range for the selected month.

#### 5. Pie Chart Data

- **Endpoint:** `GET /api/pie-chart`
- **Parameters:** `month`
- **Description:** Provides data for a pie chart displaying unique categories and the number of items in each category for the selected month.

#### 6. Combined Data

- **Endpoint:** `GET /api/combined`
- **Parameters:** `month`
- **Description:** Combines the responses from the transactions, statistics, bar chart, and pie chart APIs into a single response.

## Frontend Task

### Transactions Table

- Uses the transactions listing API to display transactions in a table.
- Includes a month dropdown (Jan to Dec) with March selected by default.
- Displays transactions of the selected month, supports search functionality, and paginated results.

### Transactions Statistics

- Displays total sale amount, total sold items, and total not sold items for the selected month.

### Transactions Bar Chart

- Displays a bar chart showing the price range and the number of items in each range for the selected month.

### Transactions Pie Chart

- Displays a pie chart showing unique categories and the number of items in each category for the selected month.

## Getting Started

### Prerequisites

- Node.js
- MongoDB
# newtonschool_assingment
