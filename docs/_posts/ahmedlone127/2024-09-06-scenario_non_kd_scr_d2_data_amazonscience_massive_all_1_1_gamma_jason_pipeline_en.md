---
layout: model
title: English scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline pipeline XlmRoBertaForSequenceClassification from haryoaw
author: John Snow Labs
name: scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline
date: 2024-09-06
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

Pretrained XlmRoBertaForSequenceClassification, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline` is a English model originally trained by haryoaw.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline_en_5.5.0_3.0_1725620259720.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline_en_5.5.0_3.0_1725620259720.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python

pipeline = PretrainedPipeline("scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline", lang = "en")
annotations =  pipeline.transform(df)   

```
```scala

val pipeline = new PretrainedPipeline("scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline", lang = "en")
val annotations = pipeline.transform(df)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|scenario_non_kd_scr_d2_data_amazonscience_massive_all_1_1_gamma_jason_pipeline|
|Type:|pipeline|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Language:|en|
|Size:|884.3 MB|

## References

https://huggingface.co/haryoaw/scenario-NON-KD-SCR-D2_data-AmazonScience_massive_all_1_1_gamma-jason

## Included Models

- DocumentAssembler
- TokenizerModel
- XlmRoBertaForSequenceClassification