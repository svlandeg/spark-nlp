---
layout: model
title: Persian imvladikon_charbert_roberta_wiki RoBertaForTokenClassification from PerSpaCor
author: John Snow Labs
name: imvladikon_charbert_roberta_wiki
date: 2024-09-19
tags: [fa, open_source, onnx, token_classification, roberta, ner]
task: Named Entity Recognition
language: fa
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
engine: onnx
annotator: RoBertaForTokenClassification
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaForTokenClassification model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`imvladikon_charbert_roberta_wiki` is a Persian model originally trained by PerSpaCor.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/imvladikon_charbert_roberta_wiki_fa_5.5.0_3.0_1726731170092.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/imvladikon_charbert_roberta_wiki_fa_5.5.0_3.0_1726731170092.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

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

tokenClassifier  = RoBertaForTokenClassification.pretrained("imvladikon_charbert_roberta_wiki","fa") \
     .setInputCols(["documents","token"]) \
     .setOutputCol("ner")

pipeline = Pipeline().setStages([documentAssembler, tokenizer, tokenClassifier])
data = spark.createDataFrame([["I love spark-nlp"]]).toDF("text")
pipelineModel = pipeline.fit(data)
pipelineDF = pipelineModel.transform(data)

```
```scala

val documentAssembler = new DocumentAssembler()
    .setInputCols("text")
    .setOutputCols("document")
    
val tokenizer = new Tokenizer()
    .setInputCols("document")
    .setOutputCol("token")

val tokenClassifier = RoBertaForTokenClassification.pretrained("imvladikon_charbert_roberta_wiki", "fa")
    .setInputCols(Array("documents","token")) 
    .setOutputCol("ner") 
    
val pipeline = new Pipeline().setStages(Array(documentAssembler, tokenizer, tokenClassifier))
val data = Seq("I love spark-nlp").toDS.toDF("text")
val pipelineModel = pipeline.fit(data)
val pipelineDF = pipelineModel.transform(data)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|imvladikon_charbert_roberta_wiki|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document, token]|
|Output Labels:|[ner]|
|Language:|fa|
|Size:|466.2 MB|

## References

https://huggingface.co/PerSpaCor/imvladikon-charbert-roberta-wiki