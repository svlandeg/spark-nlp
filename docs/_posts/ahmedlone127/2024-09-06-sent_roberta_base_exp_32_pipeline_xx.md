---
layout: model
title: Multilingual sent_roberta_base_exp_32_pipeline pipeline XlmRoBertaSentenceEmbeddings from pere
author: John Snow Labs
name: sent_roberta_base_exp_32_pipeline
date: 2024-09-06
tags: [xx, open_source, pipeline, onnx]
task: Embeddings
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

Pretrained XlmRoBertaSentenceEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`sent_roberta_base_exp_32_pipeline` is a Multilingual model originally trained by pere.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/sent_roberta_base_exp_32_pipeline_xx_5.5.0_3.0_1725623916581.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/sent_roberta_base_exp_32_pipeline_xx_5.5.0_3.0_1725623916581.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("sent_roberta_base_exp_32_pipeline", lang = "xx")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("sent_roberta_base_exp_32_pipeline", lang = "xx")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|sent_roberta_base_exp_32_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|xx|
|Size:|1.0 GB|

## References

https://huggingface.co/pere/roberta-base-exp-32

## Included Models

- DocumentAssembler
- TokenizerModel
- SentenceDetectorDLModel
- XlmRoBertaSentenceEmbeddings