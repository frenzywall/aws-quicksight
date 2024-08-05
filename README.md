# Visualizing Netflix Data with Amazon QuickSight

## Table of Contents
1. [Project Overview](#project-overview)
2. [Getting Started](#getting-started)
3. [Uploading Data to S3](#uploading-data-to-s3)
4. [Creating a QuickSight Account](#creating-a-quicksight-account)
5. [Connecting S3 with QuickSight](#connecting-s3-with-quicksight)
6. [Creating Visualizations](#creating-visualizations)
7. [Using Filters](#using-filters)
8. [Final Dashboard](#final-dashboard)
9. [Key Learnings](#key-learnings)
10. [Author](#author)

---

## Project Overview

This project focuses on visualizing Netflix data using Amazon QuickSight. Amazon QuickSight is an easy-to-use, scalable business intelligence (BI) service that lets you create interactive dashboards, gain insights from your data, and make data-driven decisions. In this project, we utilize QuickSight to create visualizations and dashboards that provide insights into various metrics, including show ratings, user perceptions, and trend analysis.

## Getting Started

### Prerequisites
- An AWS account
- Basic understanding of AWS services, particularly Amazon S3 and QuickSight

## Uploading Data to S3

### 1. Prepare Your Data
You need two files for this project:
- A `.csv` file containing the value metrics of Netflix shows, including ratings, user perceptions, and trend analysis.
- A `.json` file (manifest.json) specifying the S3 bucket details and other necessary information for accessing the data.

### 2. Upload Files to S3
1. Go to the [AWS Management Console](https://aws.amazon.com/).
2. Navigate to **S3**.
3. Create a new bucket or select an existing bucket.
4. Upload the `.csv` and `manifest.json` files to the bucket.

## Creating a QuickSight Account

1. **Sign Up for QuickSight**:
   - Go to [Amazon QuickSight](https://quicksight.aws.amazon.com/).
   - Click on "Sign up for QuickSight."
   - Follow the on-screen instructions to create your account. This process typically takes around 20 minutes.

2. **Enable S3 Access**:
   - During setup, enable QuickSight's access to the S3 bucket where your data is stored.

## Connecting S3 with QuickSight

1. **Create a Data Set**:
   - In QuickSight, go to **Manage data** and choose **New data set**.
   - Select **S3** as the data source and provide the path to your `manifest.json` file.

2. **Configure the Data Source**:
   - QuickSight uses the `manifest.json` file to understand the data structure and where to find the CSV data in S3.

## Creating Visualizations

1. **Select Data Fields**:
   - After connecting the data, you can choose the attributes you want to visualize.

2. **Drag and Drop to Canvas**:
   - Drag the selected fields onto the visualization canvas.
   - Choose from various chart types (e.g., bar, line, pie charts) to represent your data.

3. **Customize Visualizations**:
   - Use the tools in QuickSight to customize the look and feel of your visualizations.

## Using Filters

1. **Adding Filters**:
   - You can add filters to your visualizations to refine the data shown.
   - Drag fields into the filter pane and set conditions (e.g., date ranges, specific values).

2. **Interacting with Filters**:
   - Filters help in comparing different metrics and understanding their relationships.

## Final Dashboard

1. **Setting Up the Dashboard**:
   - Combine multiple visualizations into a single dashboard.
   - Arrange and resize the visualizations as needed.

2. **Dashboard Overview**:
   - The final dashboard provides a comprehensive view of the data, including various metrics and insights.

## Key Learnings

- Using S3 to store data and manifest files allows for easy integration with QuickSight.
- QuickSight's intuitive tools make it simple to create and customize visualizations.
- Filters enhance data analysis by allowing for detailed exploration of relationships between metrics.

## Author

**Sreeram**  
[LinkedIn](https://www.linkedin.com/in/sreeramjvp/)  


---

For more detailed documentation, visit the [official AWS QuickSight documentation](https://docs.aws.amazon.com/quicksight/latest/user/welcome.html).
