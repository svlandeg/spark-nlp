---
layout: model
title: English fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline pipeline BertForQuestionAnswering from muhammadravi251001
author: John Snow Labs
name: fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline
date: 2024-11-11
tags: [en, open_source, pipeline, onnx]
task: Question Answering
language: en
edition: Spark NLP 5.5.1
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertForQuestionAnswering, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline` is a English model originally trained by muhammadravi251001.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline_en_5.5.1_3.0_1731288888810.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline_en_5.5.1_3.0_1731288888810.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|fine_tuned_datasetqas_idk_mrc_with_indobert_large_p2_with_ittl_with_freeze_lr_1e_05_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.1+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|1.3 GB|

## References

https://huggingface.co/muhammadravi251001/fine-tuned-DatasetQAS-IDK-MRC-with-indobert-large-p2-with-ITTL-with-freeze-LR-1e-05

## Included Models

- MultiDocumentAssembler
- BertForQuestionAnswering