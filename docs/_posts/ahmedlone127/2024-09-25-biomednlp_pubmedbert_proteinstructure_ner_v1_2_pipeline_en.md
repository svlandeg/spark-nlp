---
layout: model
title: English biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline pipeline BertForTokenClassification from PDBEurope
author: John Snow Labs
name: biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline
date: 2024-09-25
tags: [en, open_source, pipeline, onnx]
task: Named Entity Recognition
language: en
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline` is a English model originally trained by PDBEurope.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline_en_5.5.0_3.0_1727275559505.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline_en_5.5.0_3.0_1727275559505.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|biomednlp_pubmedbert_proteinstructure_ner_v1_2_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|408.3 MB|

## References

https://huggingface.co/PDBEurope/BiomedNLP-PubMedBERT-ProteinStructure-NER-v1.2

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForTokenClassification