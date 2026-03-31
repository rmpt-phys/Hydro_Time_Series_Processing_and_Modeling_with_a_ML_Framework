### **Hydrometeorological Time-Series Processing and Flash-Flood Modeling Using a Cross-Validated ML Framework**

**About this repository:**

This repository implements an end-to-end pipeline for reading, analyzing, and preprocessing rain-gauge and river-stage data, together with flash-flood modeling and performance evaluation of machine learning algorithms.

The core component of the repository is the notebook *Project_Summary.ipynb*. It summarizes the main contributions of the author during a four-month research project carried out at the National Center for Natural Disaster Monitoring and Alerts (*Centro Nacional de Monitoramento e Alertas de Desastres Naturais* - CEMADEN), in collaboration with other researchers. The notebook serves as a structured and self-contained guide covering the problem statement, motivation, a brief literature overview, and the adopted methodology. The workflow is organized into two main parts:

- **Part 1**: Conversion of raw gauge measurements into unified hydrometeorological datasets, including data cleaning, filtering, temporal alignment, and preparation for modeling;

- **Part 2**: Flash-flood modeling using the ML4FF framework, including a step-by-step guide to configuring the auxiliary Python script *Run_ML4FF_Code.py* (input data definition, cross-validation setup, training/test splits, and output management), followed by a structured analysis of model performance and predictions.

The notebook loads station-separated datasets, aligns them onto a unified 10-minute time grid, and explicitly handles missing data through NaN insertion. It then performs exploratory and statistical analyses to extract key time-series characteristics for each station, producing a curated collection of data frames restricted to stations that satisfy predefined activity and data-quality criteria.

River-stage records are processed through a two-step pipeline: outlier detection and removal using the Hampel filter, followed by zero-phase low-pass filtering to obtain smooth, noise-reduced signals. Rainfall data are treated using a separate procedure tailored to their discrete and event-driven nature.

The processed rain-gauge and river-stage datasets are exported as structured CSV files, and dedicated training datasets are generated for integration with the ML4FF framework. The repository also includes example results (*ML4FF_Results*) and provides a reproducible workflow for building forecasting models and rigorously evaluating their predictive performance.

**Code author:**

<pre>
- Rafael Marques Paes Teixeira 
- Orcid: 0000-0001-7290-3573
</pre>

Important contributions to the notebook were made by:

<pre>
- Leonardo Bacelar Lima Santos (project manager)
- Orcid: 0000-0002-3129-772X
</pre>

Collaborators that contributed with important codes, data and discussions:

<pre>
- Andrea S. Viteri López     (0000-0002-9929-391X)
- Lidiane S. Lima            (0000-0001-5490-3975)
- Elton V. Escobar Silva     (0000-0002-9437-9351)
- Jaqueline A. J. P. Soares  (0000-0002-2569-7620)
- Kleber L. Rocha-Filho      (0009-0001-7558-1108)
- Glauston R. T. Lima        (0000-0002-6854-7921)
- Cristiano W. Eichholz      (0000-0001-7123-5438)
</pre>

Contact emails: rafael.mpt@gmail.com, santoslbl@gmail.com

#### **Preparations for the complete execution of the notebook:**

The ML4FF framework and the needed data to reproduce the results presented and analyzed in this notebook can be obtained from the links below:

https://zenodo.org/records/17654660

https://github.com/jaqueline-soares/ML4FF-framework
