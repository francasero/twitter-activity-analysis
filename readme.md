# Twitter Activity and Engagement Analysis with MongoDB and Python

This notebook analyzes Twitter activity data to uncover patterns in user behavior and engagement over time.  
It connects to MongoDB, cleans and enriches tweet and user data, and produces heatmaps that reveal when posting yields the best visibility and interaction.

---

## Project Overview

### Objectives
- Integrate and prepare data from raw tweet and user collections stored in MongoDB.  
- Clean and enrich the dataset by:
  - Converting text-based timestamps into ISODate format.
  - Calculating derived fields such as engagement rate and posting frequency.  
- Validate data quality by checking for missing, null, or inconsistent values.  
- Analyze patterns in posting and engagement by weekday, hour, and month.  
- Visualize activity and engagement through clear, comparative heatmaps.  

---

## Setup Instructions

### 1. Clone this repository
```bash
git clone https://github.com/francasero/twitter-activity-analysis.git
cd twitter-activity-analysis
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Dataset
The full MongoDB dataset (approximately 60 MB) is not included in this repository due to file size limits.
You can download it from the following link:
https://e.pcloud.link/publink/show?code=VZXBGUZlvEiJygSRGRc9JDoCtxFb4uomVRy

### 4. Prepare your MongoDB database
- Import the .json data files into MongoDB Compass or the Mongo shell.  
- Verify you have two collections:
  - tweets  
  - twitterAccounts  

### 5. Set your connection string
Before running the notebook, export your MongoDB connection string as an environment variable:
```bash
dbStringConnection="mongodb+srv://<user>:<password>@<cluster>/<dbname>"
```

### 6. Launch Jupyter Notebook
```bash
main.ipynb
```

### 7. License

MIT License

Copyright (c) 2025 Fran

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
