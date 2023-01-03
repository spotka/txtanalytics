1. Sparsify graph using network-backbone. See 4.7 in the First Course in Network Science. See https://github.com/aekpalakorn/python-backbone-network/blob/master/backbone.py.

2. Use pages rather than whole file as unit of analysis. Or paragraphs, as suggested in the Blueprints book. 

3. Do topic extraction for each community as in the Blueprints book. Generate wordmaps using topic names.

4. Do word association analysis as in InfraNodus-Paranyushkin-WWW19-Conference. 

5. Do sliding window of several years as in the Longitudinal DH (LDH) paper. 

6. Do network measurements (e.g. diameter, closeness, clustering coefficient) + gini index of keywords extracted (https://www.kaggle.com/code/akhatova/extract-keywords)

7. Try different similarity measures (beyond TFIDF cosine). Evaluate them as in https://aclanthology.org/2021.nlp4dh-1.19. They use human assigned tags. We can do the same eval based on HSS collection, just to show which similarity method works best for humanities docs. See also https://towardsdatascience.com/the-best-document-similarity-algorithm-in-2020-a-beginners-guide-a01b9ef8cf05. 
