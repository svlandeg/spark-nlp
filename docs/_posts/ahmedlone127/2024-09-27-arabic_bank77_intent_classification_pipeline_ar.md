---
layout: model
title: Arabic arabic_bank77_intent_classification_pipeline pipeline BertForSequenceClassification from bassemessam
author: John Snow Labs
name: arabic_bank77_intent_classification_pipeline
date: 2024-09-27
tags: [ar, open_source, pipeline, onnx]
task: Text Classification
language: ar
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`arabic_bank77_intent_classification_pipeline` is a Arabic model originally trained by bassemessam.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/arabic_bank77_intent_classification_pipeline_ar_5.5.0_3.0_1727414093863.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/arabic_bank77_intent_classification_pipeline_ar_5.5.0_3.0_1727414093863.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("arabic_bank77_intent_classification_pipeline", lang = "ar")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("arabic_bank77_intent_classification_pipeline", lang = "ar")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|arabic_bank77_intent_classification_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|ar|
|Size:|507.5 MB|

## References

https://huggingface.co/bassemessam/Arabic-bank77-intent-classification

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification