---
layout: model
title: Russian ruscibert_pipeline pipeline RoBertaEmbeddings from ai-forever
author: John Snow Labs
name: ruscibert_pipeline
date: 2024-09-01
tags: [ru, open_source, pipeline, onnx]
task: Embeddings
language: ru
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`ruscibert_pipeline` is a Russian model originally trained by ai-forever.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/ruscibert_pipeline_ru_5.4.2_3.0_1725186068091.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/ruscibert_pipeline_ru_5.4.2_3.0_1725186068091.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("ruscibert_pipeline", lang = "ru")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("ruscibert_pipeline", lang = "ru")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|ruscibert_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|ru|
|Size:|463.7 MB|

## References

https://huggingface.co/ai-forever/ruSciBERT

## Included Models

- DocumentAssembler
- TokenizerModel
- RoBertaEmbeddings