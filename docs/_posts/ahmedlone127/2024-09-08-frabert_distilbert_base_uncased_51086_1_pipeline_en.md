---
layout: model
title: English frabert_distilbert_base_uncased_51086_1_pipeline pipeline DistilBertForSequenceClassification from Francesco0101
author: John Snow Labs
name: frabert_distilbert_base_uncased_51086_1_pipeline
date: 2024-09-08
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

Pretrained DistilBertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`frabert_distilbert_base_uncased_51086_1_pipeline` is a English model originally trained by Francesco0101.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/frabert_distilbert_base_uncased_51086_1_pipeline_en_5.5.0_3.0_1725808458803.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/frabert_distilbert_base_uncased_51086_1_pipeline_en_5.5.0_3.0_1725808458803.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("frabert_distilbert_base_uncased_51086_1_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("frabert_distilbert_base_uncased_51086_1_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|frabert_distilbert_base_uncased_51086_1_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|249.5 MB|

## References

https://huggingface.co/Francesco0101/FRABERT-distilbert-base-uncased-51086-1

## Included Models

- DocumentAssembler
- TokenizerModel
- DistilBertForSequenceClassification