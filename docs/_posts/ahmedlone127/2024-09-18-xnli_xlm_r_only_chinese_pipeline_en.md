---
layout: model
title: English xnli_xlm_r_only_chinese_pipeline pipeline XlmRoBertaForSequenceClassification from semindan
author: John Snow Labs
name: xnli_xlm_r_only_chinese_pipeline
date: 2024-09-18
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

Pretrained XlmRoBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`xnli_xlm_r_only_chinese_pipeline` is a English model originally trained by semindan.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/xnli_xlm_r_only_chinese_pipeline_en_5.5.0_3.0_1726633084035.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/xnli_xlm_r_only_chinese_pipeline_en_5.5.0_3.0_1726633084035.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("xnli_xlm_r_only_chinese_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("xnli_xlm_r_only_chinese_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|xnli_xlm_r_only_chinese_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|807.1 MB|

## References

https://huggingface.co/semindan/xnli_xlm_r_only_zh

## Included Models

- DocumentAssembler
- TokenizerModel
- XlmRoBertaForSequenceClassification