---
layout: model
title: Moldavian, Moldovan, Romanian sent_romanian_sentence_bert_base_uncased_v1_pipeline pipeline BertSentenceEmbeddings from iliemihai
author: John Snow Labs
name: sent_romanian_sentence_bert_base_uncased_v1_pipeline
date: 2024-09-15
tags: [ro, open_source, pipeline, onnx]
task: Embeddings
language: ro
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
annotator: PipelineModel
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertSentenceEmbeddings, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`sent_romanian_sentence_bert_base_uncased_v1_pipeline` is a Moldavian, Moldovan, Romanian model originally trained by iliemihai.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/sent_romanian_sentence_bert_base_uncased_v1_pipeline_ro_5.5.0_3.0_1726377266233.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/sent_romanian_sentence_bert_base_uncased_v1_pipeline_ro_5.5.0_3.0_1726377266233.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("sent_romanian_sentence_bert_base_uncased_v1_pipeline", lang = "ro")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("sent_romanian_sentence_bert_base_uncased_v1_pipeline", lang = "ro")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|sent_romanian_sentence_bert_base_uncased_v1_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|ro|
|Size:|463.3 MB|

## References

https://huggingface.co/iliemihai/romanian-sentence-bert-base-uncased-v1

## Included Models

- DocumentAssembler
- TokenizerModel
- SentenceDetectorDLModel
- BertSentenceEmbeddings