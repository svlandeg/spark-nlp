---
layout: model
title: English depression_detection_model_ganda_pipeline pipeline DistilBertForSequenceClassification from thePixel42
author: John Snow Labs
name: depression_detection_model_ganda_pipeline
date: 2024-09-12
tags: [en, open_source, pipeline, onnx]
task: Text Classification
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

Pretrained DistilBertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`depression_detection_model_ganda_pipeline` is a English model originally trained by thePixel42.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/depression_detection_model_ganda_pipeline_en_5.5.0_3.0_1726125182807.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/depression_detection_model_ganda_pipeline_en_5.5.0_3.0_1726125182807.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("depression_detection_model_ganda_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("depression_detection_model_ganda_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|depression_detection_model_ganda_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|249.5 MB|

## References

https://huggingface.co/thePixel42/depression_detection_model-lg

## Included Models

- DocumentAssembler
- TokenizerModel
- DistilBertForSequenceClassification