---
layout: model
title: Latin laberta_pipeline pipeline RoBertaEmbeddings from bowphs
author: John Snow Labs
name: laberta_pipeline
date: 2024-09-01
tags: [la, open_source, pipeline, onnx]
task: Embeddings
language: la
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`laberta_pipeline` is a Latin model originally trained by bowphs.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/laberta_pipeline_la_5.4.2_3.0_1725165435540.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/laberta_pipeline_la_5.4.2_3.0_1725165435540.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("laberta_pipeline", lang = "la")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("laberta_pipeline", lang = "la")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|laberta_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|la|
|Size:|469.8 MB|

## References

https://huggingface.co/bowphs/LaBerta

## Included Models

- DocumentAssembler
- TokenizerModel
- RoBertaEmbeddings