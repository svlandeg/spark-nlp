---
layout: model
title: Multilingual scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual XlmRoBertaForSequenceClassification from haryoaw
author: John Snow Labs
name: scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual
date: 2024-09-18
tags: [xx, open_source, onnx, sequence_classification, xlm_roberta]
task: Text Classification
language: xx
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
engine: onnx
annotator: XlmRoBertaForSequenceClassification
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained XlmRoBertaForSequenceClassification model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual` is a Multilingual model originally trained by haryoaw.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual_xx_5.5.0_3.0_1726686318835.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual_xx_5.5.0_3.0_1726686318835.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
     
documentAssembler = DocumentAssembler() \
    .setInputCol('text') \
    .setOutputCol('document')
    
tokenizer = Tokenizer() \
    .setInputCols(['document']) \
    .setOutputCol('token')

sequenceClassifier  = XlmRoBertaForSequenceClassification.pretrained("scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual","xx") \
     .setInputCols(["documents","token"]) \
     .setOutputCol("class")

pipeline = Pipeline().setStages([documentAssembler, tokenizer, sequenceClassifier])
data = spark.createDataFrame([["I love spark-nlp"]]).toDF("text")
pipelineModel = pipeline.fit(data)
pipelineDF = pipelineModel.transform(data)

```
```scala

val documentAssembler = new DocumentAssembler()
    .setInputCols("text")
    .setOutputCols("document")
    
val tokenizer = new Tokenizer()
    .setInputCols(Array("document"))
    .setOutputCol("token")

val sequenceClassifier = XlmRoBertaForSequenceClassification.pretrained("scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual", "xx")
    .setInputCols(Array("documents","token")) 
    .setOutputCol("class") 
    
val pipeline = new Pipeline().setStages(Array(documentAssembler, tokenizer, sequenceClassifier))
val data = Seq("I love spark-nlp").toDS.toDF("text")
val pipelineModel = pipeline.fit(data)
val pipelineDF = pipelineModel.transform(data)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|scenario_non_kd_scr_copy_cdf_all_d2_data_cardiffnlp_tweet_sentiment_multilingual|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document, token]|
|Output Labels:|[class]|
|Language:|xx|
|Size:|883.8 MB|

## References

https://huggingface.co/haryoaw/scenario-NON-KD-SCR-COPY-CDF-ALL-D2_data-cardiffnlp_tweet_sentiment_multilingual