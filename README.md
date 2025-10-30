# complaint-triage-bi-pipeline
VBA-based ETL process flow developed for the ingestion of unstructured corporate feedback (email complaints) data and its automated categorization via text analysis. The project aims to derive quantitative metrics, such as Risk Score and Supplier ID, which are critical for Dimensional Analysis and Data Modeling.
# 📊 Complaint Triage & Business Intelligence (BI) Data Pipeline: A VBA-based ETL Solution

### 🎯 Project Goal: Establishing a Governance-Compliant, Analytics-Ready Data Source

This project presents a robust **VBA-based Data Ingestion and ETL solution** developed for the acquisition and refinement of high-volume **unstructured corporate feedback data (email complaints)**. The system serves as a strategic infrastructure aimed at constructing an optimized analytical dataset, facilitating the **derivation of quantitative metrics** and subsequent **Dimensional Data Modeling**.

---

### 📌 The Challenge (Data Architecture and Latency)

The reliance on manual processing for email complaints introduced significant operational and analytical friction:

* **Operational Latency:** Suboptimal response times for critical quality control issues.
* **Data Governance Deficit:** Absence of a standardized structure prevented consistent **quantitative analysis** and introduced bias in risk assessment.

---

### ✅ The Automated Solution: ETL for Dimensional Modeling (VBA/Excel)

This system implements a full **Extract, Transform, Load (ETL)** cycle to prepare data for **Dimensional Analysis** and advanced **Data Modeling**:

#### 1. Extract & Structuring
* **Data Ingestion:** Automatically ingests emails from a designated Microsoft Outlook source, extracting all critical metadata.
* **Audit Trail Generation:** Preserves the original email file (`.msg`) and creates a **direct archival hyperlink** within the structured Excel output, ensuring **data traceability**.

#### 2. Transformation (Metric Derivation & Dimensional Assignment)
* **Intelligent Categorization:** The script utilizes text parsing and keyword matching to assign a precise **Complaint Category**.
* **Dimensional Assignment:** **(Core BI Step)** The system assigns two essential dimensions for relational modeling: **Supplier ID** and **Product ID**.
* **Quantitative Metric Derivation:** Converts the qualitative risk level (e.g., High) into a continuous, measurable metric: **Risk Score (1-10)**.
* **Visual Prioritization:** Implements automated conditional formatting to enable immediate operational triage.

#### 3. Load & Business Impact

The final structured output is a clean, normalized fact table containing all essential dimensions and derived metrics.

* **Strategic Value:** Enables the calculation of **Key Performance Indicators (KPIs)** such as "Supplier-Specific Defect Rate" and "Average Risk Score by Product Category."
* **Operational Efficiency:** Eliminates manual data entry, shifting the Quality Assurance function from administrative work to **proactive issue resolution**.

---

### 🛠️ Technologies & Methodology

* **Methodology:** **Process Optimization** and **Data Governance** Principles.
* **Tools:** **VBA (Visual Basic for Applications) & Microsoft Excel** (Front-end and ETL engine), **Microsoft Outlook Object Model** (Data source integration).
* **Readiness:** Output is optimized for ingestion into a relational database (e.g., **SQL Server**) or direct connection via BI platforms (**Power BI/Tableau**).

### 🔗 Code Repository

* **Macro Files:** The VBA source code is available in the respective modules.
* **Setup Instructions:** [VBA kodunu çalıştırmadan önce `saveFolderPath` değişkenini yerel sisteme uygun olarak güncelleyin.]
