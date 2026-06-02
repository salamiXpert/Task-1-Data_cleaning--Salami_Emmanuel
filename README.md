# E-Commerce Sales Dataset Cleaning Project

## Project Overview

This project focuses on cleaning and preparing an e-commerce sales dataset for data analysis.
The original dataset contained inconsistent values, missing data, formatting issues, and duplicate records that could affect analysis accuracy.

The cleaning process was performed in Microsoft Excel to improve data quality, consistency, and usability for further analytics and reporting.

---

## Dataset Information

The dataset contains the following columns:

* OrderID
* Date
* CustomerID
* Product
* Quantity
* UnitPrice
* ShippingAddress
* PaymentMethod
* OrderStatus
* TrackingNumber
* ItemsInCart
* CouponCode
* ReferralSource
* TotalPrice

---

# Data Cleaning Tasks Performed

## 1. Removed Duplicate Records

* Checked for duplicate rows using Excel's **Remove Duplicates** feature.
* Ensured that each order record is unique.

---

## 2. Handled Missing Values

### CouponCode Column

* Missing/null values in the `CouponCode` column were replaced with:

```markdown
NO_COUPON
```

* This was done to maintain consistency and avoid blank entries during analysis.

---

## 3. Standardized Date Format

* Converted all date values into a consistent format:

```markdown
YYYY-MM-DD
```

Example:

```markdown
2023/01/04 → 2023-01-04
```

---

## 4. Corrected Data Types

The following data types were verified and standardized:

| Column     | Data Type   |
| ---------- | ----------- |
| Quantity   | Integer     |
| UnitPrice  | Decimal     |
| TotalPrice | Decimal     |
| Date       | Date Format |

---

## 5. Cleaned Text Data

* Removed extra spaces from text columns.
* Standardized text formatting for consistency.

Example:

```markdown
" Debit Card " → "Debit Card"
```

---

## 6. Validated Numeric Columns

* Checked for invalid or negative values in:

  * Quantity
  * UnitPrice
  * TotalPrice

* Ensured calculations were accurate.

---

## 7. Created Cleaned Dataset

* Saved the cleaned version of the dataset in a separate worksheet named:

```markdown
Cleaned_Dataset
```

This preserves the original raw data for reference.

---

# Tools Used

* Microsoft Excel
* Excel Functions
* Data Cleaning Techniques

---

# Outcome

After cleaning:

* Missing values were handled
* Data consistency improved
* Dataset became analysis-ready
* Errors and duplicates were minimized

The cleaned dataset can now be used for:

* Sales analysis
* Customer behavior analysis
* Dashboard creation
* Business intelligence reporting

---

# File Structure

```markdown
Dataset           -> Raw original dataset
Cleaned_Dataset   -> Cleaned dataset ready for analysis
```

---

# Author

**Salami Emmanuel Hammed**

---

# Future Improvements

* Automate cleaning using Python or SQL
* Create interactive dashboards in Power BI or Tableau
* Perform Exploratory Data Analysis (EDA)
* Build predictive analytics models
