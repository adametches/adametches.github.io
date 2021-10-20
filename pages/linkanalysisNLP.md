## Knowledge Graph Building from NLP using Spacy
---

A simple example of producing a knowledge graph using NLP the example uses the following tooling:
  - Jupyter Labs and Python
  - Spacy NLP
  - Networkx

In this example I take a low effort approach by using off-the-shelf models and tooling. I wanted to evaluate the default models in Spacy to process a document with the following processing pipeline:

1. Named Entity Extraction NER
2. Co-reference resolution 
3. Semantic type enhancement using wikidata
4. Relationship extraction
5. Create NetworkX graph

From a limited set of control data and a small amount of code the output is reasonable. It's a simple model so could be extended <a href="../jupyter/simple-pipeline.html"> View Source in Html </a> 

### Document Input
<iframe src="../html/simplepipelineinput.html" title="Simple Pipline Input" style="border:none;" width="100%" height="100px"></iframe>


### Knowledge Graph Output
<iframe src="../html/simplepipelineoutput.html" title="Simple Pipline Input" style="border:none;" width="100%" height="400px"></iframe>
