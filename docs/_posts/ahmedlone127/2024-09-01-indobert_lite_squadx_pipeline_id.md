---
layout: model
title: Indonesian indobert_lite_squadx_pipeline pipeline BertForQuestionAnswering from Wikidepia
author: John Snow Labs
name: indobert_lite_squadx_pipeline
date: 2024-09-01
tags: [id, open_source, pipeline, onnx]
task: Question Answering
language: id
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`indobert_lite_squadx_pipeline` is a Indonesian model originally trained by Wikidepia.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/indobert_lite_squadx_pipeline_id_5.4.2_3.0_1725184736016.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/indobert_lite_squadx_pipeline_id_5.4.2_3.0_1725184736016.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("indobert_lite_squadx_pipeline", lang = "id")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("indobert_lite_squadx_pipeline", lang = "id")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|indobert_lite_squadx_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|id|
|Size:|41.9 MB|

## References

https://huggingface.co/Wikidepia/indobert-lite-squadx

## Included Models

- MultiDocumentAssembler
- BertForQuestionAnswering