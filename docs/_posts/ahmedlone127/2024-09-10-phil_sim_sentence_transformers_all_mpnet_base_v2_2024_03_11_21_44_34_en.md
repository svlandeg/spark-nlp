---
layout: model
title: English phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34 MPNetEmbeddings from dbourget
author: John Snow Labs
name: phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34
date: 2024-09-10
tags: [en, open_source, onnx, embeddings, mpnet]
task: Embeddings
language: en
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
engine: onnx
annotator: MPNetEmbeddings
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained MPNetEmbeddings model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34` is a English model originally trained by dbourget.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34_en_5.5.0_3.0_1725963825998.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34_en_5.5.0_3.0_1725963825998.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
 
documentAssembler = DocumentAssembler() \
      .setInputCol("text") \
      .setOutputCol("document")
    
embeddings = MPNetEmbeddings.pretrained("phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34","en") \
      .setInputCols(["document"]) \
      .setOutputCol("embeddings")       
        
pipeline = Pipeline().setStages([documentAssembler, embeddings])
data = spark.createDataFrame([["I love spark-nlp"]]).toDF("text")
pipelineModel = pipeline.fit(data)
pipelineDF = pipelineModel.transform(data)

```
```scala

val documentAssembler = new DocumentAssembler() 
    .setInputCol("text") 
    .setOutputCol("document")
    
val embeddings = MPNetEmbeddings.pretrained("phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34","en") 
    .setInputCols(Array("document")) 
    .setOutputCol("embeddings")

val pipeline = new Pipeline().setStages(Array(documentAssembler, embeddings))
val data = Seq("I love spark-nlp").toDF("text")
val pipelineModel = pipeline.fit(data)
val pipelineDF = pipelineModel.transform(data)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|phil_sim_sentence_transformers_all_mpnet_base_v2_2024_03_11_21_44_34|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document]|
|Output Labels:|[mpnet]|
|Language:|en|
|Size:|407.1 MB|

## References

https://huggingface.co/dbourget/phil-sim-sentence-transformers-all-mpnet-base-v2-2024-03-11_21-44-34