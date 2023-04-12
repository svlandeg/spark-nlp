---
layout: model
title: German Bert Embeddings
author: John Snow Labs
name: bert_embeddings_bert_base_german_uncased
date: 2022-04-11
tags: [bert, embeddings, de, open_source]
task: Embeddings
language: de
edition: Spark NLP 3.4.2
spark_version: 3.0
supported: true
recommended: true
annotator: BertEmbeddings
article_header:
type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained Bert Embeddings model, uploaded to Hugging Face, adapted and imported into Spark NLP. `bert-base-german-uncased` is a German model orginally trained by `dbmdz`.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/bert_embeddings_bert_base_german_uncased_de_3.4.2_3.0_1649675856996.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/bert_embeddings_bert_base_german_uncased_de_3.4.2_3.0_1649675856996.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

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

embeddings = BertEmbeddings.pretrained("bert_embeddings_bert_base_german_uncased","de") \
.setInputCols(["document", "token"]) \
.setOutputCol("embeddings")

pipeline = Pipeline(stages=[documentAssembler, tokenizer, embeddings])

data = spark.createDataFrame([["Ich liebe Funken NLP"]]).toDF("text")

result = pipeline.fit(data).transform(data)
```
```scala
val documentAssembler = new DocumentAssembler() 
.setInputCol("text") 
.setOutputCol("document")

val tokenizer = new Tokenizer() 
.setInputCols(Array("document"))
.setOutputCol("token")

val embeddings = BertEmbeddings.pretrained("bert_embeddings_bert_base_german_uncased","de") 
.setInputCols(Array("document", "token")) 
.setOutputCol("embeddings")

val pipeline = new Pipeline().setStages(Array(documentAssembler, tokenizer, embeddings))

val data = Seq("Ich liebe Funken NLP").toDF("text")

val result = pipeline.fit(data).transform(data)
```


{:.nlu-block}
```python
import nlu
nlu.load("de.embed.bert_base_german_uncased").predict("""Ich liebe Funken NLP""")
```

</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|bert_embeddings_bert_base_german_uncased|
|Compatibility:|Spark NLP 3.4.2+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[sentence, token]|
|Output Labels:|[bert]|
|Language:|de|
|Size:|412.8 MB|
|Case sensitive:|true|

## References

- https://huggingface.co/dbmdz/bert-base-german-uncased
- https://deepset.ai/german-bert
- https://deepset.ai/
- https://spacy.io/
- https://github.com/allenai/scibert
- https://github.com/stefan-it/fine-tuned-berts-seq
- https://github.com/dbmdz/berts/issues/new