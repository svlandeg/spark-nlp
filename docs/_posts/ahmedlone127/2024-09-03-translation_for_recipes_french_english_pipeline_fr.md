---
layout: model
title: French translation_for_recipes_french_english_pipeline pipeline MarianTransformer from PaulineSanchez
author: John Snow Labs
name: translation_for_recipes_french_english_pipeline
date: 2024-09-03
tags: [fr, open_source, pipeline, onnx]
task: Translation
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

Pretrained MarianTransformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`translation_for_recipes_french_english_pipeline` is a French model originally trained by PaulineSanchez.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/translation_for_recipes_french_english_pipeline_fr_5.5.0_3.0_1725404994160.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/translation_for_recipes_french_english_pipeline_fr_5.5.0_3.0_1725404994160.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("translation_for_recipes_french_english_pipeline", lang = "fr")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("translation_for_recipes_french_english_pipeline", lang = "fr")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|translation_for_recipes_french_english_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|fr|
|Size:|508.1 MB|

## References

https://huggingface.co/PaulineSanchez/translation_for_recipes_fr_en

## Included Models

- DocumentAssembler
- SentenceDetectorDLModel
- MarianTransformer