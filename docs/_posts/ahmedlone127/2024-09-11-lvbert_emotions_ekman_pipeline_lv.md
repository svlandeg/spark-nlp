---
layout: model
title: Latvian lvbert_emotions_ekman_pipeline pipeline BertForSequenceClassification from AiLab-IMCS-UL
author: John Snow Labs
name: lvbert_emotions_ekman_pipeline
date: 2024-09-11
tags: [lv, open_source, pipeline, onnx]
task: Text Classification
language: lv
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`lvbert_emotions_ekman_pipeline` is a Latvian model originally trained by AiLab-IMCS-UL.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/lvbert_emotions_ekman_pipeline_lv_5.5.0_3.0_1726095069203.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/lvbert_emotions_ekman_pipeline_lv_5.5.0_3.0_1726095069203.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("lvbert_emotions_ekman_pipeline", lang = "lv")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("lvbert_emotions_ekman_pipeline", lang = "lv")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|lvbert_emotions_ekman_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|lv|
|Size:|414.9 MB|

## References

https://huggingface.co/AiLab-IMCS-UL/lvbert-emotions-ekman

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification