---
layout: model
title: English sarcasm_detection_bert_base_uncased_cree_pipeline pipeline BertForSequenceClassification from jkhan447
author: John Snow Labs
name: sarcasm_detection_bert_base_uncased_cree_pipeline
date: 2024-09-25
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

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`sarcasm_detection_bert_base_uncased_cree_pipeline` is a English model originally trained by jkhan447.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/sarcasm_detection_bert_base_uncased_cree_pipeline_en_5.5.0_3.0_1727263833210.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/sarcasm_detection_bert_base_uncased_cree_pipeline_en_5.5.0_3.0_1727263833210.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("sarcasm_detection_bert_base_uncased_cree_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("sarcasm_detection_bert_base_uncased_cree_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|sarcasm_detection_bert_base_uncased_cree_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|409.4 MB|

## References

https://huggingface.co/jkhan447/sarcasm-detection-Bert-base-uncased-CR

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification