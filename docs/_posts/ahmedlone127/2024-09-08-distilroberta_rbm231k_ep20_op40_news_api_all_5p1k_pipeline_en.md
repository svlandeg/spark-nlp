---
layout: model
title: English distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline pipeline RoBertaForSequenceClassification from judy93536
author: John Snow Labs
name: distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline
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

Pretrained RoBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline` is a English model originally trained by judy93536.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline_en_5.5.0_3.0_1725830308084.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline_en_5.5.0_3.0_1725830308084.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|distilroberta_rbm231k_ep20_op40_news_api_all_5p1k_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|308.6 MB|

## References

https://huggingface.co/judy93536/distilroberta-rbm231k-ep20-op40-news_api_all_5p1k

## Included Models

- DocumentAssembler
- TokenizerModel
- RoBertaForSequenceClassification