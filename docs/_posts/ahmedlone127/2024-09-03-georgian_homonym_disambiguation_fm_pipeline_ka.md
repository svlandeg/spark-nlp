---
layout: model
title: Georgian georgian_homonym_disambiguation_fm_pipeline pipeline DistilBertEmbeddings from davmel
author: John Snow Labs
name: georgian_homonym_disambiguation_fm_pipeline
date: 2024-09-03
tags: [ka, open_source, pipeline, onnx]
task: Embeddings
language: ka
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DistilBertEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`georgian_homonym_disambiguation_fm_pipeline` is a Georgian model originally trained by davmel.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/georgian_homonym_disambiguation_fm_pipeline_ka_5.5.0_3.0_1725389256185.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/georgian_homonym_disambiguation_fm_pipeline_ka_5.5.0_3.0_1725389256185.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("georgian_homonym_disambiguation_fm_pipeline", lang = "ka")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("georgian_homonym_disambiguation_fm_pipeline", lang = "ka")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|georgian_homonym_disambiguation_fm_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|ka|
|Size:|247.2 MB|

## References

https://huggingface.co/davmel/ka_homonym_disambiguation_FM

## Included Models

- DocumentAssembler
- TokenizerModel
- DistilBertEmbeddings