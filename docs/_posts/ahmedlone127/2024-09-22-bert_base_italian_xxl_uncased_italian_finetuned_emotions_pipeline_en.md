---
layout: model
title: English bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline pipeline BertForSequenceClassification from MelmaGrigia
author: John Snow Labs
name: bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline
date: 2024-09-22
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

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline` is a English model originally trained by MelmaGrigia.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline_en_5.5.0_3.0_1727030100823.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline_en_5.5.0_3.0_1727030100823.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bert_base_italian_xxl_uncased_italian_finetuned_emotions_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|414.8 MB|

## References

https://huggingface.co/MelmaGrigia/bert-base-italian-xxl-uncased-italian-finetuned-emotions

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification