---
layout: model
title: Portuguese ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline pipeline T5Transformer from llmf
author: John Snow Labs
name: ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline
date: 2024-08-05
tags: [pt, open_source, pipeline, onnx]
task: [Question Answering, Summarization, Translation, Text Generation]
language: pt
edition: Spark NLP 5.4.2
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained T5Transformer, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline` is a Portuguese model originally trained by llmf.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline_pt_5.4.2_3.0_1722837637011.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline_pt_5.4.2_3.0_1722837637011.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline", lang = "pt")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline", lang = "pt")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|ptt5_base_portuguese_finetuned_summ_rulingbr_v2_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.4.2+|
|License:|Open Source|
|Edition:|Official|
|Language:|pt|
|Size:|952.2 MB|

## References

https://huggingface.co/llmf/ptt5-base-portuguese-finetuned-Summ-RulingBR-V2

## Included Models

- DocumentAssembler
- T5Transformer