# Hi, I'm Matthew Hall 👋
### Bioinformatics Scientist | Population Genomics ($N=342k$)

I provide **high-fidelity genomic insights** by integrating massive cohort data analysis with a foundational understanding of **molecular biology**. My work focuses on deriving high-resolution associations from population-scale datasets while maintaining a 'zero-failure' mindset for data integrity.
---

### 🧬 Current Focus
* **GLP-1R Variant Discovery:** Architecting GWAS pipelines within the NIH All of Us (v9) environment.
* **Cloud Infrastructure:** Optimizing R/Python workflows on the Terra/Researcher Workbench (WDL/Jupyter).
* **Molecular Validation:** Correlating in-silico findings with bench-top assays (Western Blot, qRT-PCR).

### 🛠 Technical Toolkit
* **Dry Lab:** R (ggplot2, UpSetR), Python (Pandas, NumPy), GWAS, WGS/WES Analysis, ANNOVAR.
* **Wet Lab:** Western Blotting, qRT-PCR, Chromatography, P1 Phage Transduction, DNA/RNA Extraction.
* **Compliance:** METRC, HIPAA, GMP/GLP Standards, 100% Audit Accuracy.

### 📊 Impact Metric
**Managed and analyzed genomic data for a cohort of N=342,874 participants to identify novel variant associations within the GLP-1R locus.**

---
📫 [LinkedIn](https://www.linkedin.com/in/matthall-genomics) | 📧 Mhhall725@gmail.com
---

# Project: Genomic Data Pipeline (v9 Analysis Framework)
This repository demonstrates a modular Python-based pipeline designed for the ingestion, quality control (QC), and processing of high-volume genomic datasets, specifically optimized for the **NIH All of Us (v9)** environment.

### 🧬 Current Phase: Phase 1 - Automated Ingestion & QC
The pipeline currently implements a hardened ingestion module (`01_data_ingestion.py`) featuring:
- **Automated Logging:** Full traceability of data loading events using the Python `logging` library.
- **QC Protocol:** Immediate generation of descriptive statistics (Mean, Std, Quartiles) to verify data distribution before analysis.
- **Data Privacy:** Local-only `data/` directory structure to ensure compliance with HIPAA and researcher workbench security protocols.

### Project Architecture
- **`data/`**: (Local Only) Directory for raw genomic source files.
- **`scripts/`**: Modular Python components for data processing and analysis.
- **`results/`**: Automated output directory for QC reports and processed summaries.

### How to Run
1. Ensure a valid CSV is present in the `data/` directory.
2. Execute the ingestion module:
   ```powershell
   python scripts/01_data_ingestion.py
