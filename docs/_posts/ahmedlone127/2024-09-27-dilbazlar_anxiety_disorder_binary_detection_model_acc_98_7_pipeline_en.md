---
layout: model
title: English dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline pipeline BertForSequenceClassification from halilibr
author: John Snow Labs
name: dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline
date: 2024-09-27
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

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline` is a English model originally trained by halilibr.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline_en_5.5.0_3.0_1727412666757.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline_en_5.5.0_3.0_1727412666757.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|dilbazlar_anxiety_disorder_binary_detection_model_acc_98_7_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|691.6 MB|

## References

https://huggingface.co/halilibr/dilbazlar-anxiety-disorder-binary-detection-model-acc-98.7

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification