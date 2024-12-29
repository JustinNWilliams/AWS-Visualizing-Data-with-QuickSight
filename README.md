# Visualizing Netflix Data with Amazon QuickSight

## Introduction

In this project, I used **Amazon QuickSight** to visualize Netflix data. In this project I created interactive dashboards, visualized data, and generated business insights in real-time.

---
## What is Amazon QuickSight?

![image](https://github.com/user-attachments/assets/ce220e15-ba64-451e-8a14-cd02982a3f3e)

**Amazon QuickSight** is a fully managed, scalable and cost-effective cloud-based Business Intelligence (BI) service that enables users to:
- Build interactive dashboards.
- Gain actionable insights from data.
- Scale seamlessly with enterprise-level capabilities.

---

## Project Overview

This project demonstrates:
1. Uploading a dataset to **Amazon S3**.
2. Connecting the dataset to **Amazon QuickSight**.
3. Creating visualizations and applying filters.
4. Designing a dashboard to present the final insights.

---

## Prerequisites

To complete this project, I needed:
- An **AWS account** with access to Amazon S3 and QuickSight.
- A dataset (`netflix_titles.csv`) for analysis.
- Basic familiarity with cloud services and data visualization.

---

## Steps to Complete the Project

### 1. Upload Dataset Files to Amazon S3
I started by uploading the following files into an **S3 bucket**:
- `netflix_titles.csv`
- `manifest.json`

Next, I edited the `manifest.json` file to include the **S3 URI** for the `netflix_titles.csv` file. This step is essential because QuickSight uses the `manifest.json` file to locate and read the dataset.

![Screenshot 2024-12-29 033731](https://github.com/user-attachments/assets/f6aba519-8ec5-4358-a7f4-2d4876051f0b)

---

### 2. Create a QuickSight Account
I created a **QuickSight account** using the **30-day free trial**. The account creation process was straightforward and took about **3-5 minutes**.

![Screenshot 2024-12-29 034259](https://github.com/user-attachments/assets/b16c6b74-0b89-41c0-810b-26f880141dfe)


---

### 3. Connect the Dataset to QuickSight
1. I navigated to the **Datasets** panel on the QuickSight home page and clicked **New Dataset**.
2. I selected **S3** as the data source and connected it using the **S3 URI** from the `manifest.json` file.

💡 The `manifest.json` file was critical because it provided QuickSight with the location and structure of my dataset.

![Screenshot 2024-12-29 034950](https://github.com/user-attachments/assets/5b7b3246-43a7-44a8-9df8-f7ecc3fecf55)

---

### 4. Create Visualizations
After uploading the dataset, I created my first visualizations. Here’s what I did:
- **Top 20 Records by Release Year and Type**:
  - Dragged `release_year` into the **Y-axis** of a **Donut Chart**.
  - Dragged `release_year` into the **Y-axis** and `type` into the **group/color field** of a **Vertical Bar Graph**.

![Screenshot 2024-12-29 035938](https://github.com/user-attachments/assets/c445d10e-264d-4bba-b7c1-c78a4b17f6ed)

---

### 5. Apply Filters
I used filters to refine the data and focus on specific insights. For instance:
- I created a filter for `release_year` to display records from **2015 and later**.
- I visualized genres like **Action & Adventure**, **TV Comedies**, and **Thrillers**.

![Screenshot 2024-12-29 092115](https://github.com/user-attachments/assets/a33aad91-212b-43fb-bb93-afe314ac455c)


---

### 6. Designing a Dashboard
To present the insights, I designed a dashboard with the following steps:
1. Labeled each graph clearly.
2. Aligned all visualizations for a clean and professional look.
3. Exported the dashboard as a **PDF** by clicking **Export** in the top-right corner and selecting **Generate PDF**.

![Screenshot 2024-12-29 093524](https://github.com/user-attachments/assets/e8f0af05-5137-4717-ab5c-6414aebd656a)

---

## Key Takeaways

- I learned that **Amazon QuickSight** is an intuitive BI tool that simplifies data visualization and analysis.
- This project helped me understand how to integrate S3 datasets with QuickSight and create meaningful insights.
- Filters and dashboards are powerful features for refining and presenting data.

---

## Time Taken

This project took me approximately **90 minutes** to complete.

---

## Resources

- [Amazon QuickSight Documentation](https://aws.amazon.com/quicksight/)
- [AWS S3 Documentation](https://aws.amazon.com/s3/)
- [Netflix Dataset (Kaggle)](https://www.kaggle.com/datasets/shivamb/netflix-shows)
