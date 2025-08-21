# Grocery Inventory Analysis

**Project Overview**  
تحليل بيانات المخزون في متجر بقالة لفهم العلاقة بين كمية المخزون ومعدل التدوير، احتساب "أيام التخزين"، وتصنيف المنتجات إلى فئات مثل "low stock" و"high overstock".

## Table of Contents
- [Overview](#project-overview)
- [Setup & Dependencies](#setup--dependencies)
- [Data Description](#data-description)
- [Analysis Steps](#analysis-steps)
- [Key Findings](#key-findings)
- [Future Work](#future-work)
- [Project Structure](#project-structure)
- [License & Contact](#license--contact)

---

## Overview
- تنظيف البيانات من خلال استخدام `.head()`, `.info()`, `.describe()`.
- تحويل `Unit_Price` من نص إلي قيمة رقمية بعد إزالة رموز العملة.
- رسم العلاقة بين `Stock_Quantity` و `Inventory_Turnover_Rate` باستخدام مخطط scatter.
- <img width="552" height="422" alt="image" src="https://github.com/user-attachments/assets/40d8cf31-722a-4344-92c3-cbbe63221eee" />

- حساب "Days on Hand" (عدد الأيام التي يكفي فيها المخزون) ورسم توزيعه.
- ![Uploading image.png…]()

- استخراج وتصنيف المنتجات إلى:
  - **low_stock**: الكمية أقل من مستوى إعادة الطلب ومعدل التدوير أقل من المتوسط.
  - **high_overstock**: الكمية أكبر من ضعف مستوى إعادة الطلب.

---

## Setup & Dependencies
**Python Version:** 3.x

**Dependencies:**
```bash
pip install pandas seaborn matplotlib
