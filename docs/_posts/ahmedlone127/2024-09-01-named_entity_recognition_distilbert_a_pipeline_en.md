---
layout: model
title: English named_entity_recognition_distilbert_a_pipeline pipeline DistilBertForTokenClassification from imrazaa
author: John Snow Labs
name: named_entity_recognition_distilbert_a_pipeline
date: 2024-09-01
tags: [en, open_source, pipeline, onnx]
task: Named Entity Recognition
language: en
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DistilBertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`named_entity_recognition_distilbert_a_pipeline` is a English model originally trained by imrazaa.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/named_entity_recognition_distilbert_a_pipeline_en_5.4.2_3.0_1725170632486.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/named_entity_recognition_distilbert_a_pipeline_en_5.4.2_3.0_1725170632486.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("named_entity_recognition_distilbert_a_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("named_entity_recognition_distilbert_a_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|named_entity_recognition_distilbert_a_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|247.4 MB|

## References

https://huggingface.co/imrazaa/named-entity-recognition-distilbert-A

## Included Models

- DocumentAssembler
- TokenizerModel
- DistilBertForTokenClassification