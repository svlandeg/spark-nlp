---
layout: model
title: English malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline pipeline BertForSequenceClassification from liangyuant
author: John Snow Labs
name: malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline
date: 2024-09-26
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

Pretrained BertForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline` is a English model originally trained by liangyuant.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline_en_5.5.0_3.0_1727376458845.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline_en_5.5.0_3.0_1727376458845.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|malay_marco_minilm_l_12_v2_finetuned_10epoch_num200_450_405cls_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|124.8 MB|

## References

https://huggingface.co/liangyuant/ms-marco-MiniLM-L-12-v2-finetuned-10epoch-num200-450-405cls

## Included Models

- DocumentAssembler
- TokenizerModel
- BertForSequenceClassification