---
layout: model
title: English antismetisimlargedata_finetuned_mlm_nepal_bhasa BertEmbeddings from Dhanush66
author: John Snow Labs
name: antismetisimlargedata_finetuned_mlm_nepal_bhasa
date: 2024-09-13
tags: [en, open_source, onnx, embeddings, bert]
task: Embeddings
language: en
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
engine: onnx
annotator: BertEmbeddings
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained BertEmbeddings model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`antismetisimlargedata_finetuned_mlm_nepal_bhasa` is a English model originally trained by Dhanush66.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/antismetisimlargedata_finetuned_mlm_nepal_bhasa_en_5.5.0_3.0_1726189255244.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/antismetisimlargedata_finetuned_mlm_nepal_bhasa_en_5.5.0_3.0_1726189255244.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
 
documentAssembler = DocumentAssembler() \
      .setInputCol("text") \
      .setOutputCol("document")
    
tokenizer = Tokenizer() \ 
      .setInputCols("document") \ 
      .setOutputCol("token")

embeddings = BertEmbeddings.pretrained("antismetisimlargedata_finetuned_mlm_nepal_bhasa","en") \
      .setInputCols(["document", "token"]) \
      .setOutputCol("embeddings")       
        
pipeline = Pipeline().setStages([documentAssembler, tokenizer, embeddings])
data = spark.createDataFrame([["I love spark-nlp"]]).toDF("text")
pipelineModel = pipeline.fit(data)
pipelineDF = pipelineModel.transform(data)

```
```scala

val documentAssembler = new DocumentAssembler() 
    .setInputCol("text") 
    .setOutputCol("document")
    
val tokenizer = new Tokenizer() 
    .setInputCols(Array("document"))
    .setOutputCol("token")

val embeddings = BertEmbeddings.pretrained("antismetisimlargedata_finetuned_mlm_nepal_bhasa","en") 
    .setInputCols(Array("document", "token")) 
    .setOutputCol("embeddings")

val pipeline = new Pipeline().setStages(Array(documentAssembler, tokenizer, embeddings))
val data = Seq("I love spark-nlp").toDF("text")
val pipelineModel = pipeline.fit(data)
val pipelineDF = pipelineModel.transform(data)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|antismetisimlargedata_finetuned_mlm_nepal_bhasa|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document, token]|
|Output Labels:|[bert]|
|Language:|en|
|Size:|407.1 MB|

## References

https://huggingface.co/Dhanush66/AntismetisimLargedata-finetuned-MLM-NEW