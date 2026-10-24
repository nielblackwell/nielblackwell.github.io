---
layout: landing
title: Ashley Blackwell
---

![head-shot]({{ '/assets/images/head-shot.png' | relative_url }})

Applied data scientist with an MS in Data Analytics and BA in History (Minor in Art). With machine learning, model evaluation, data visualization, and 13+ years of operational leadership behind me, I am also experienced in the development and deployment of systems across NLP, computer vision, predictive modeling, and network analysis, with strengths in evaluation, explainability, human-in-the-loop methods, and translating complex requirements into usable tools. My interest lies in interdisciplinary research software and computational approaches to historical, cultural, and human-centered research.

## Selected Work

### The Absent Archive: Mapping What Remains When History Is Unraveled 

The Metropolitan Museum of Art holds 484,956 objects, including 2,108 from Andean cultures. Andean cultures like the Inka Empire kept their records and accounting using khipukuna (also known as the khipu, which is a Quechua term for "knots”). The Met holds none.

Developed and accepted over centuries as a complex administrative tool, the khipu was the primary system of record-keeping, computing, and accounting for many of these cultures. Presently, and globally, only around 900 khipu remain, scattered across three continents and 88 collections. 

Initially, my goal was simply to map the interconnectedness of khipu across Andean civilizations using network analysis. The Met’s open-access dataset was a random choice for a starting point. But as I cleaned the data and ran my confirmation sweeps, I discovered a profound, literal void: a total count of zero. 

I decided to treat this absence as the subject itself. By building a network graph linking the Met's 2,108 Andean objects to their respective cultures and mediums, I used betweenness centrality to find the hidden tissue holding the picture together. 

**The data revealed something beautiful:**

>**Materials over Politics:** The top connectors in the network aren't specific empires—they are materials like ceramic, camelid hair, and silver. Materiality is what stitches distinct, separate peoples together across history.

>**The Moche Bridge:** The Moche culture emerged as the single greatest architectural bridge in the network, sharing deep attributes across nearly the entire Andean collection. When the written or knotted record is silenced, the physical medium speaks for it. This network visualizes what keeps the story intact when so much of the archive is missing. 

![The Absent Archive betweenness centrality visualization]({{ '/assets/images/absent-archive.png' | relative_url }})

[Explore the Interactive HTML Here!](https://ashleybrookeblackwell.github.io/andean-heritage-network/Andean_Network_Betweenness_Centrality.html)

**Methods / Tools**

- **Data Source:** The Metropolitan Museum of Art Open Access ( MetObjects.csv ), CC0 1.0 Universal.
- **Full collection:** 484,956 objects
- **Andean subset:** 2,108 objects
- **Tools:** pandas, NetworkX, PyVis, Jupyter 

**The Network**

>**Nodes:** 2,258 (objects + their culture and material attributes)

>**Edges:** 5,509

>**Distinct materials after cleaning:** 109

>**Metric:** Betweenness Centrality — *which attribute nodes sit on the most paths between everything else*.

[Explore the Project Here](https://github.com/ashleybrookeblackwell/andean-heritage-network/tree/main)


### Lung CT Cancer Classification and Model Deployment

This project classifies chest CT-scan images into lung cancer subtypes (adenocarcinoma, large-cell carcinoma, squamous-cell carcinoma) versus normal tissue. Rather than building a single model, I benchmarked three distinct approaches to determine the most accurate and generalizable strategy on a small, class-imbalanced medical imaging dataset — then deployed the strongest model with Grad-CAM explainability so its predictions can be visually interrogated, not just trusted blindly.

**Three modeling strategies were evaluated for lung cancer subtype classification from CT scans:**

>Baseline CNN

>AutoKeras AutoML

>EfficientNetB0 *Transfer Learning* 

The Baseline CNN collapsed under class imbalance, while AutoML improved performance modestly but remained unstable. The selected EfficientNetB0 model, fine-tuned via transfer learning, achieved **85.71% test accuracy**, **0.8551 macro-F1**, and **0.969 AUC**, with Grad-CAM overlays enabling visual inspection of model attention within lung regions. Deployed live via Gradio on Hugging Face.

![Grad-CAM visualization]({{ '/assets/images/grad-cam.png' | relative_url }})

[Hugging Face Deployment](https://huggingface.co/spaces/ablackwellb/chest-ct-cancerscan)

**Methods / Tools** 

- **Data Source:** A public, four-class chest CT-scan dataset from Kaggle (three cancer subtypes + normal), with meaningful class imbalance — a realistic constraint that shaped every modeling decision below.

- **Tools:** Python, TensorFlow, Keras, EfficientNetB0 (transfer learning), AutoKeras, Grad-CAM, Gradio, Hugging Face Spaces, scikit-learn, NumPy, Matplotlib

[Explore the Project Here](https://github.com/ashleybrookeblackwell/cancer-site-detection-cnn)

## Current Research

### Misreading The Archive: What Is Missing When Machines Read An Archive? 

**Research in progress**

This research is beginning with English-language Allied records concerning Germany during and immediately after World War II. Candidate sources include administrative reports, displaced-person records, reconstruction documentation, cultural-property inventories, unit records, and damage assessments. The initial corpus is currently being selected.

**The research is guided by four questions:**

> What does one administrative system call something that another describes differently?
> Who appears in one archive but not the other?
> Can entities be reconciled across the English and German records?
> What gets lost when the same place/person/event travels across languages, handwriting, OCR and cataloging systems?

**Status:** Research in progress.

[Explore the Project Here](https://github.com/ashleybrookeblackwell/misreading-the-archive)

## Background

I build predictive analytics, machine learning, and decision-support systems that make complex information understandable, actionable, and ethically useful. I am interested in how data systems function inside real organizations: how patterns are identified, how inefficiencies are diagnosed, how risk is interpreted, how decisions are made, and how complex information can be translated into something people can actually use.

My work sits at the intersection of data science, operations, ethics, and human-centered decision support. I bring a technical foundation in machine learning, predictive modeling, data analytics, business analytics, and deep learning, supported by an MS in Data Analytics, a Graduate Certificate in Business Analytics, a Deep Learning Specialization, a Certification in IT Automation with Python, and a BA in History (Minor in Art).

## Connect

- [GitHub](https://github.com/ashleybrookeblackwell)
- [LinkedIn](https://www.linkedin.com/in/ashleybrookeblackwell)
- [CV]({{ '/assets/files/CV.pdf' | relative_url }})
- [Email](mailto:ashleybrookeblackwell@gmail.com)
