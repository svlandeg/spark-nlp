---
layout: model
title: English rinna_arabert_qa_ar4_pipeline pipeline BertForQuestionAnswering from Echiguerkh
author: John Snow Labs
name: rinna_arabert_qa_ar4_pipeline
date: 2024-09-17
tags: [en, open_source, pipeline, onnx]
task: Question Answering
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

Pretrained BertForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`rinna_arabert_qa_ar4_pipeline` is a English model originally trained by Echiguerkh.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/rinna_arabert_qa_ar4_pipeline_en_5.5.0_3.0_1726567613877.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/rinna_arabert_qa_ar4_pipeline_en_5.5.0_3.0_1726567613877.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("rinna_arabert_qa_ar4_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("rinna_arabert_qa_ar4_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|rinna_arabert_qa_ar4_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|504.8 MB|

## References

https://huggingface.co/Echiguerkh/rinna-AraBert-qa-ar4

## Included Models

- MultiDocumentAssembler
- BertForQuestionAnswering