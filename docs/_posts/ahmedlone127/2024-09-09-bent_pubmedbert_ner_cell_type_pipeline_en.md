---
layout: model
title: English bent_pubmedbert_ner_cell_type_pipeline pipeline BertForTokenClassification from pruas
author: John Snow Labs
name: bent_pubmedbert_ner_cell_type_pipeline
date: 2024-09-09
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

Pretrained BertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`bent_pubmedbert_ner_cell_type_pipeline` is a English model originally trained by pruas.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bent_pubmedbert_ner_cell_type_pipeline_en_5.5.0_3.0_1725886966776.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bent_pubmedbert_ner_cell_type_pipeline_en_5.5.0_3.0_1725886966776.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("bent_pubmedbert_ner_cell_type_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("bent_pubmedbert_ner_cell_type_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bent_pubmedbert_ner_cell_type_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|408.1 MB|

## References

https://huggingface.co/pruas/BENT-PubMedBERT-NER-Cell-Type

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForTokenClassification