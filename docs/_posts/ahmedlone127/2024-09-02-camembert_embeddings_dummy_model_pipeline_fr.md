---
layout: model
title: French camembert_embeddings_dummy_model_pipeline pipeline CamemBertEmbeddings from winterdawn
author: John Snow Labs
name: camembert_embeddings_dummy_model_pipeline
date: 2024-09-02
tags: [fr, open_source, pipeline, onnx]
task: Embeddings
language: fr
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained CamemBertEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`camembert_embeddings_dummy_model_pipeline` is a French model originally trained by winterdawn.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/camembert_embeddings_dummy_model_pipeline_fr_5.5.0_3.0_1725296780101.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/camembert_embeddings_dummy_model_pipeline_fr_5.5.0_3.0_1725296780101.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("camembert_embeddings_dummy_model_pipeline", lang = "fr")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("camembert_embeddings_dummy_model_pipeline", lang = "fr")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|camembert_embeddings_dummy_model_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|fr|
|Size:|264.0 MB|

## References

https://huggingface.co/winterdawn/dummy-model

## Included Models

- DocumentAssembler
- TokenizerModel
- CamemBertEmbeddings