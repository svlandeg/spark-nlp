---
layout: model
title: Italian mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline pipeline T5Transformer from gsarti
author: John Snow Labs
name: mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline
date: 2024-08-26
tags: [it, open_source, pipeline, onnx]
task: [Question Answering, Summarization, Translation, Text Generation]
language: it
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained T5Transformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline` is a Italian model originally trained by gsarti.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline_it_5.4.2_3.0_1724681822519.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline_it_5.4.2_3.0_1724681822519.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline", lang = "it")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline", lang = "it")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|mt5_base_repubblica_tonga_tonga_islands_ilgiornale_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|it|
|Size:|2.4 GB|

## References

https://huggingface.co/gsarti/mt5-base-repubblica-to-ilgiornale

## Included Models

- DocumentAssembler
- T5Transformer