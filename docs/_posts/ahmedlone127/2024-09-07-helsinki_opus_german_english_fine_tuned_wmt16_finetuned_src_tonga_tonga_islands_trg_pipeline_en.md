---
layout: model
title: English helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline pipeline MarianTransformer from musralina
author: John Snow Labs
name: helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline
date: 2024-09-07
tags: [en, open_source, pipeline, onnx]
task: Translation
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

Pretrained MarianTransformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline` is a English model originally trained by musralina.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline_en_5.5.0_3.0_1725748129907.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline_en_5.5.0_3.0_1725748129907.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|helsinki_opus_german_english_fine_tuned_wmt16_finetuned_src_tonga_tonga_islands_trg_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|499.6 MB|

## References

https://huggingface.co/musralina/helsinki-opus-de-en-fine-tuned-wmt16-finetuned-src-to-trg

## Included Models

- DocumentAssembler
- SentenceDetectorDLModel
- MarianTransformer