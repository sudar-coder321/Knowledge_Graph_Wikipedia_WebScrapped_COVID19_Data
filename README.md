# Web_Scraping_Knowledge_Graphs
Web Scraping and Knowledge Graphs with Machine Learning

# Concepts

## About Knowledge Graph

 - Knowledge graphs are a tool of data science that deal with interconnected entities (people, organizations, places, events, etc.). Entities are the nodes which are connected via edges. Knowledge graphs consist of these entity pairs that can be traversed to uncover meaningful connections in unstructured data.




## Constructing a Knowledge Graph

 - Knowledge graphs can be constructed automatically from text using part-of-speech and dependency parsing. The extraction of entity pairs from grammatical patterns is fast and scalable to large amounts of text using NLP library SpaCy.


## Sentence segmentation

 - The first step of building a knowledge graph is to split the text document or article into sentences. Then we limit our examples to simple sentences with one subject and one object.

## Entity extraction

 - You can extract a single word entity from a sentence with the help of parts-of-speech (POS) tags. The nouns and proper nouns will be the entities. These nodes are going to be entities that are present in the Wikipedia sentences. Edges are the relationships connecting these entities. We will extract these elements in an unsupervised manner, i.e. we’ll use the grammar of the sentences.

## Relations extraction

 - These edges are relations between pairs of nodes. The function below is capable of capturing such predicates from these sentences. I used spaCy’s rule-based matching. The pattern defined in the function tries to find the ROOT word or the main verb in the sentence. 

 - https://ailab.ijs.si/dunja/SiKDD2020/Papers/03%20-%20Knowledge_graph_aware_text_classification__SiKDD_-6.pdf
