---
layout: model
title: Castilian, Spanish t5_base_translation_spanish_english_pipeline pipeline T5Transformer from vgaraujov
author: John Snow Labs
name: t5_base_translation_spanish_english_pipeline
date: 2024-08-12
tags: [es, open_source, pipeline, onnx]
task: [Question Answering, Summarization, Translation, Text Generation]
language: es
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained T5Transformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`t5_base_translation_spanish_english_pipeline` is a Castilian, Spanish model originally trained by vgaraujov.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/t5_base_translation_spanish_english_pipeline_es_5.4.2_3.0_1723458511908.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/t5_base_translation_spanish_english_pipeline_es_5.4.2_3.0_1723458511908.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("t5_base_translation_spanish_english_pipeline", lang = "es")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("t5_base_translation_spanish_english_pipeline", lang = "es")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|t5_base_translation_spanish_english_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|es|
|Size:|1.0 GB|

## References

https://huggingface.co/vgaraujov/t5-base-translation-es-en

## Included Models

- DocumentAssembler
- T5Transformer