---
layout: model
title: French nermembert_large_3entities_pipeline pipeline CamemBertForTokenClassification from CATIE-AQ
author: John Snow Labs
name: nermembert_large_3entities_pipeline
date: 2024-08-31
tags: [fr, open_source, pipeline, onnx]
task: Named Entity Recognition
language: fr
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained CamemBertForTokenClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`nermembert_large_3entities_pipeline` is a French model originally trained by CATIE-AQ.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/nermembert_large_3entities_pipeline_fr_5.4.2_3.0_1725140474975.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/nermembert_large_3entities_pipeline_fr_5.4.2_3.0_1725140474975.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("nermembert_large_3entities_pipeline", lang = "fr")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("nermembert_large_3entities_pipeline", lang = "fr")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|nermembert_large_3entities_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|fr|
|Size:|1.3 GB|

## References

https://huggingface.co/CATIE-AQ/NERmembert-large-3entities

## Included Models

- DocumentAssembler
- TokenizerModel
- CamemBertForTokenClassification