# ClinTrialsAPItoExcel
A Connection to Clin Trials API using Excel VBA. 
# Clinical Trial Data Fetcher Add-In

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Prerequisites](#prerequisites)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Available Search Variables](#available-search-variables)
7. [Examples](#examples)
8. [Troubleshooting](#troubleshooting)
9. [Version History](#version-history)
10. [License](#license)
11. [Contact](#contact)

---

## Introduction

**Clinical Trial Data Fetcher Add-In** is an Excel add-in designed to streamline the retrieval of clinical trial information directly within your Excel worksheets. By leveraging the ClinicalTrials.gov API, this add-in allows users to fetch detailed data about clinical studies using the unique NCT Identifier (NCT ID) and specific search variables.

---

## Features

- **Easy Data Retrieval:** Fetch clinical trial details by simply entering the NCT ID and desired data points.
- **Comprehensive Data Mapping:** Access a wide range of data fields, including study titles, sponsors, status, eligibility criteria, outcomes, and more.
- **User-Friendly:** Seamlessly integrates with Excel, allowing data retrieval through simple functions.
- **Automatic Updates:** Refresh data to get the latest information from ClinicalTrials.gov.

---

## Prerequisites

- **Microsoft Excel:** Version 2013 or later is recommended.
- **Internet Connection:** Required to fetch data from the ClinicalTrials.gov API.
- **Enabled Macros:** Ensure that macros are enabled in Excel to allow the add-in to function correctly.

---

## Installation

Follow these steps to install the **Clinical Trial Data Fetcher Add-In**:

1. **Download the Add-In:**
   - Obtain the `.xlam` file from the distribution source (e.g., [GitHub Repository](#), [Dropbox Link](#), etc.).

2. **Open Excel:**
   - Launch Microsoft Excel on your computer.

3. **Access Add-In Settings:**
   - Navigate to the **File** tab.
   - Click on **Options**.
   - In the **Excel Options** window, select **Add-Ins** from the left sidebar.

4. **Manage Excel Add-Ins:**
   - At the bottom of the window, ensure **Excel Add-ins** is selected in the **Manage** dropdown.
   - Click on the **Go...** button.

5. **Browse and Select the Add-In:**
   - In the **Add-Ins** dialog box, click on **Browse...**.
   - Navigate to the location where you saved the `.xlam` file.
   - Select the file and click **OK**.

6. **Enable the Add-In:**
   - Ensure that the checkbox next to the add-in is checked.
   - Click **OK** to finalize the installation.

7. **Verify Installation:**
   - You should now see a new tab or menu related to the add-in in the Excel ribbon (if designed to add one).
   - Alternatively, the functions provided by the add-in will be available for use in your worksheets.

---

## Usage

The add-in provides a custom function named `GetClinicalTrialValue` that can be used directly within your Excel worksheets to fetch specific data points from ClinicalTrials.gov.

### Function Syntax

```excel
=GetClinicalTrialValue(NCT_ID, Search_Variable)
