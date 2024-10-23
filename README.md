# 📊 Development of Advanced Analytics Tools supporting Business Development


## Overview
This project involves the creation of a graph database (**Neo4j**) that aggregates and organizes scientific studies focused on the most prominent sequencing techniques, including **RNA-seq**, **scRNA-seq**, **Spatial Transcriptomics**, **Whole Genome (WGS)**, and **Whole Exome (WES) sequencing**, **ATAC-seq**, **ChIP-seq**, and **TCR-seq**. The structure is designed for adaptability and can easily be transferred to SQL-based relational databases.



### Core Database Structure
<img src="https://github.com/antiparticle25/genomic_data_solutions/blob/main/files/core_database.png?raw=true" width="1100" alt="Core Database Structure">

### Visualization of Data Query Capabilities
Flexibility in querying detailed information about studies and researchers in the database:

<div>
  <img src="https://github.com/antiparticle25/genomic_data_solutions/blob/main/files/general_to_study.gif?raw=true" alt="Studies from Journals" style="width: 70%; float: left;">
  <img src="https://github.com/antiparticle25/genomic_data_solutions/blob/main/files/country_to_study.gif?raw=true" alt="Researchers by Location" style="width: 70%; float: right;">
</div>

<p style="font-size: 18px;">Check <a href="https://drive.google.com/file/d/14Qx4DzydU5uWo9ttAsMsMSX_Tsiq3b6x/view?usp=drive_link"><strong>here</strong></a> and <a href="https://drive.google.com/file/d/1OgZKWGWOV03JPGYA-DNNbyjW1ZKa6eBg/view?usp=drive_link"><strong>here</strong></a> for videos.</p>

## Trend Analysis
This approach enables:
- **Identification** of researchers working on specific sequencing techniques.
- **Pinpointing** the institutions and countries where these researchers are located.
- **Finding** studies based on MeSH terms or Keywords.
- **Analyzing** trends across different journals and subjects over time.

## Integration with LLM Tools
By utilizing an appropriate embedding model, each study can be represented in a high-dimensional space, eventually allowing for similarity assessments based on their content.

### Visualization
Dimensionality reduction (UMAP) of all scRNA-seq studies in Europe provides a visual representation of the data clustering, in this case COVID-19 and remaining studies

<img src="https://github.com/antiparticle25/genomic_data_solutions/blob/main/files/scRNA_covid.png?raw=true" width="600" alt="UMAP Visualization of scRNA-seq Studies">

## Automated Business Messaging
Through prompt engineering, it is possible to generate automated business messages tailored to specific research topics. Here's a zero-shot example using an outdated LLM:


> **Subject: Enhancing Your Research on Intestinal Treg Functions**
>
> Dear Dr. Researcher,
>
> I hope this message finds you well. I recently had the opportunity to delve into your compelling research on immune microniches shaping intestinal Treg function. The insights your team provides on the cellular dynamics and spatial compartmentalization in the gut are not only fascinating but also pivotal to advancing our understanding of immune tolerance.
>
> Your innovative approach using in vivo live imaging alongside photo-activation-guided single-cell RNA sequencing and spatial transcriptomics offers a remarkable view into the interaction dynamics within the intestinal lamina propria. I am particularly impressed by your findings on how eTreg cells stabilize within their microniche and how inflammation can disrupt this crucial balance, emphasizing the importance of spatial analysis in immunology.
>
> At Genomics, we specialize in enhancing research such as yours through our advanced sequencing capabilities and comprehensive bioinformatics solutions. Our expertise in spatial transcriptomics aligns seamlessly with your research needs, offering you refined tools and methodologies to further explore and visualize cellular interactions in complex tissues.
>
> We would be thrilled to discuss how our services can support and expand the capabilities of your research. Please feel free to reach out to me directly at genomics@genomics or call me at 31415926 to arrange a meeting where we can discuss this in more detail.
>
> Best regards,
> 
> John Polymerase
> 
> Genomics



## Business Development Applications
By linking this structured data and similarity analysis with large language models (LLMs), the developed system enables:
- **Automated lead generation**: Tailoring business intereactions with researchers and institutions based on their current work and interests.
- **Strategic expansion**: Understanding current client needs to identify potential new customers with similar research profiles.
- **Resource optimization**: Providing business representatives with data-driven insights prior to client visits, ensuring targeted discussions about relevant research and needs.

## Future Enhancements
Planned upgrades include:
- **Natural Language Interface**: Allowing users to query the database with natural language.
- **Equipment and Reagent Cataloging**: I am currently fine-tuning a model for name entity recognition to catalog equipment and reagents (e.g., sequencing machines and library preparation kits); this allows a better understanding of its usage in different institutes and research subjects.
- **Chatbot Development**: Providing sequencing service advice, recommending techniques tailored to specific needs.
