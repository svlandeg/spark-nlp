---
layout: model
title: Hindi muril_large_chaii_pipeline pipeline BertForQuestionAnswering from abhishek
author: John Snow Labs
name: muril_large_chaii_pipeline
date: 2024-09-23
tags: [hi, open_source, pipeline, onnx]
task: Question Answering
language: hi
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`muril_large_chaii_pipeline` is a Hindi model originally trained by abhishek.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/muril_large_chaii_pipeline_hi_5.5.0_3.0_1727070855702.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/muril_large_chaii_pipeline_hi_5.5.0_3.0_1727070855702.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("muril_large_chaii_pipeline", lang = "hi")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("muril_large_chaii_pipeline", lang = "hi")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|muril_large_chaii_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|hi|
|Size:|1.9 GB|

## References

https://huggingface.co/abhishek/muril-large-chaii

## Included Models

- MultiDocumentAssembler
- BertForQuestionAnswering