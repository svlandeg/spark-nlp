---
layout: model
title: Multilingual distil_multilingual_cased_fire_classification_silvanus_pipeline pipeline DistilBertForSequenceClassification from rollerhafeezh-amikom
author: John Snow Labs
name: distil_multilingual_cased_fire_classification_silvanus_pipeline
date: 2024-09-22
tags: [xx, open_source, pipeline, onnx]
task: Text Classification
language: xx
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained DistilBertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`distil_multilingual_cased_fire_classification_silvanus_pipeline` is a Multilingual model originally trained by rollerhafeezh-amikom.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/distil_multilingual_cased_fire_classification_silvanus_pipeline_xx_5.5.0_3.0_1727020800633.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/distil_multilingual_cased_fire_classification_silvanus_pipeline_xx_5.5.0_3.0_1727020800633.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("distil_multilingual_cased_fire_classification_silvanus_pipeline", lang = "xx")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("distil_multilingual_cased_fire_classification_silvanus_pipeline", lang = "xx")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|distil_multilingual_cased_fire_classification_silvanus_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|xx|
|Size:|507.6 MB|

## References

https://huggingface.co/rollerhafeezh-amikom/distil-multilingual-cased-fire-classification-silvanus

## Included Models

- DocumentAssembler
- TokenizerModel
- DistilBertForSequenceClassification