---
layout: model
title: None malasar_luke_dict_pipeline pipeline WhisperForCTC from leenag
author: John Snow Labs
name: malasar_luke_dict_pipeline
date: 2024-09-17
tags: [nan, open_source, pipeline, onnx]
task: Automatic Speech Recognition
language: nan
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained WhisperForCTC, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`malasar_luke_dict_pipeline` is a None model originally trained by leenag.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/malasar_luke_dict_pipeline_nan_5.5.0_3.0_1726550818088.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/malasar_luke_dict_pipeline_nan_5.5.0_3.0_1726550818088.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("malasar_luke_dict_pipeline", lang = "nan")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("malasar_luke_dict_pipeline", lang = "nan")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|malasar_luke_dict_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|nan|
|Size:|1.7 GB|

## References

https://huggingface.co/leenag/Malasar_Luke_Dict

## Included Models

- AudioAssembler
- WhisperForCTC