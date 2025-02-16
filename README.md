# MongoDB Aggregation Queries

This repository contains a collection of MongoDB aggregation queries used for data processing, transformation, and analysis.

## Features
- Various aggregation queries demonstrating filtering, grouping, sorting, and data transformation.
- Optimized MongoDB pipeline operations.
- Examples of `$match`, `$group`, `$sort`, `$lookup`, `$project`, and more.

## Requirements
- MongoDB installed and running.
- A database with sample collections to test the queries.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mongodb-aggregation.git
   ```
2. Navigate to the project directory:
   ```bash
   cd mongodb-aggregation
   ```
3. Open the queries in your MongoDB shell or application (e.g., MongoDB Compass, Node.js, Python driver, etc.).

## Example Queries
### 1. Grouping Data
```json
{
  "$group": {
    "_id": "$category",
    "total": { "$sum": "$price" }
  }
}
```

### 2. Sorting Results
```json
{
  "$sort": { "total": -1 }
}
```

### 3. Filtering Documents
```json
{
  "$match": { "status": "active" }
}
```
