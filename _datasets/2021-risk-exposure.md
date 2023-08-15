---
title: "Risk Exposure Measures"
collection: datasets
type: "A Dataset"
permalink: /datasets/2021-risk-exposure
date: 2021-01-01
---

Firm-level risk exposures are derived by first parsing all public 10-K filings available in the EDGAR database reported between 1/1/2018 and 3/1/20206. Specifically, all readable text under "Item 1" is processed by a Python program to ensure the extracted raw terms are following the standard procedure in the text-analysis literature; i.e., the text is cleaned from abbreviations, headings, plurals, stop words, and numbers, leaving only relevant lower-cased terms. Firm $i$'s level of risk exposure to category $j$ is defined each calender year as:
<br/> 
$$Risk\, Exposure_{i,j} = \frac{\sum_{y,j}^{Y,j}term_{y,j}}{\sum_{j=1}^{J=44}\sum_{y,j}^{Y,j}term_{y,j}}$$
<br/> 
In essence, this formula estimates each firm's risk exposure to category $j$ as the total number of terms extracted from
the document falling under risk factor $j$ divided by the total number of terms captured for all 44
risk factors for firm $i$. Risk categories, and their associated terms, are created by [Davis, S. J., Hansen, S., & Seminario-Amez, C. (2021). *Firm-level Risk Exposures and Stock Returns in The Wake of COVID-19*](https://doi.org/10.3386/w27867). All 44 risk factors, and their terms, are obtained from the authors’ article. Categories (or factors) include Commercial Property, Display Technology, Traditional Retail, E-commerce, and Franchising. For further detail, please read [the recent draft of my paper.](https://dx.doi.org/10.2139/ssrn.3906487)