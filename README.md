<div style="max-width: 900px; text-align: justify;">

#### **About this notebook**

A general notebook developed for reading, analyzing, pre-processing rain-gauge / river-stage data and flash-flood modeling with detailed analysis of performance and predictions of machine-leaning algorithms.<br> 

The notebook loads all station-separated files, aligns them on a unified 10-minute time grid, and inserts NaNs where measurements are missing. It then performs a set of analyses to extract and summarize key characteristics of the time series from each station. A curated collection of data frames is produced, including only stations that are active and meet predefined data-quality criteria.<br>

River-stage records undergo a two-step pre-processing pipeline: first, outliers are identified and removed using the Hampel filter; second, a zero-phase low-pass filter is applied to obtain smooth, noise-reduced time series. Rainfall data are treated with a different procedure, appropriate for their discrete and event-driven nature.<br>

The resulting processed rain-gauge and river-stage data are exported as well-structured CSV files, and dedicated training datasets are generated for use within the ML4FF framework. This notebook also provides a step-by-step guide for producing stage forecasting models with this framework and also for analyzing their performance and predictions.

Code author:

<pre>
- Rafael Marques Paes Teixeira 
- Orcid: 0000-0001-7290-3573
</pre>

Important contributions to this notebook were made by:

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

Contact emails: 
rafael.mpt@gmail.com, santoslbl@gmail.com

</div>
