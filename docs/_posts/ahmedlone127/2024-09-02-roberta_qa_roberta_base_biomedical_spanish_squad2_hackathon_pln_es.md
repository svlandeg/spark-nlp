---
layout: model
title: Castilian, Spanish roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln RoBertaForQuestionAnswering from hackathon-pln-es
author: John Snow Labs
name: roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln
date: 2024-09-02
tags: [es, open_source, onnx, question_answering, roberta]
task: Question Answering
language: es
edition: Spark NLP 5.5.0
spark_version: 3.0
supported: true
engine: onnx
annotator: RoBertaForQuestionAnswering
article_header:
  type: cover
use_language_switcher: "Python-Scala-Java"
---

## Description

Pretrained RoBertaForQuestionAnswering model, adapted from Hugging Face and curated to provide scalability and production-readiness using Spark NLP.`roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln` is a Castilian, Spanish model originally trained by hackathon-pln-es.

{:.btn-box}
<button class="button button-orange" disabled>Live Demo</button>
<button class="button button-orange" disabled>Open in Colab</button>
[Download](https://s3.amazonaws.com/auxdata.johnsnowlabs.com/public/models/roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln_es_5.5.0_3.0_1725252437530.zip){:.button.button-orange.button-orange-trans.arr.button-icon}
[Copy S3 URI](s3://auxdata.johnsnowlabs.com/public/models/roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln_es_5.5.0_3.0_1725252437530.zip){:.button.button-orange.button-orange-trans.button-icon.button-copy-s3}

## How to use



<div class="tabs-box" markdown="1">
{% include programmingLanguageSelectScalaPythonNLU.html %}
```python
             
documentAssembler = MultiDocumentAssembler() \
     .setInputCol(["question", "context"]) \
     .setOutputCol(["document_question", "document_context"])
    
spanClassifier = RoBertaForQuestionAnswering.pretrained("roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln","es") \
     .setInputCols(["document_question","document_context"]) \
     .setOutputCol("answer")

pipeline = Pipeline().setStages([documentAssembler, spanClassifier])
data = spark.createDataFrame([["What framework do I use?","I use spark-nlp."]]).toDF("document_question", "document_context")
pipelineModel = pipeline.fit(data)
pipelineDF = pipelineModel.transform(data)

```
```scala

val documentAssembler = new MultiDocumentAssembler()
    .setInputCol(Array("question", "context")) 
    .setOutputCol(Array("document_question", "document_context"))
    
val spanClassifier = RoBertaForQuestionAnswering.pretrained("roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln", "es")
    .setInputCols(Array("document_question","document_context")) 
    .setOutputCol("answer") 
    
val pipeline = new Pipeline().setStages(Array(documentAssembler, spanClassifier))
val data = Seq("What framework do I use?","I use spark-nlp.").toDS.toDF("document_question", "document_context")
val pipelineModel = pipeline.fit(data)
val pipelineDF = pipelineModel.transform(data)

```
</div>

{:.model-param}
## Model Information

{:.table-model}
|---|---|
|Model Name:|roberta_qa_roberta_base_biomedical_spanish_squad2_hackathon_pln|
|Compatibility:|Spark NLP 5.5.0+|
|License:|Open Source|
|Edition:|Official|
|Input Labels:|[document_question, document_context]|
|Output Labels:|[answer]|
|Language:|es|
|Size:|464.7 MB|

## References

https://huggingface.co/hackathon-pln-es/roberta-base-biomedical-es-squad2-es