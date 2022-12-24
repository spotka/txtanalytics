##Text analytics code

[tfidf_createvecs.ipynb](https://github.com/thomouvic/txtanalytics/blob/main/tfidf_createvecs.ipynb): Given a document collection (e.g. [txts.zip](https://github.com/thomouvic/txtanalytics/blob/main/txts.zip)), it creates normalized TFIDF vectors. There will be a vector for each document in the collection. The vectors will be stored all together in a pandas dataframe, then to a csv file (e.g. [docvecs.csv](https://github.com/thomouvic/txtanalytics/blob/main/docvecs.csv)). The structure of the dataframe (and csv file) is as follows: 

<pre>
docid,termid,score,term
0,41217,0.7963703814049661,pratt
0,29708,0.26072073508329247,james
0,44505,0.18392130794771977,religion
0,44509,0.1782887684728951,religious
</pre>

The above notebook, also creates a dataframe and csv file of docnames: [docnames.csv](https://github.com/thomouvic/txtanalytics/blob/main/docnames.csv)

[tfidf_cos_sim.ipynb](https://github.com/thomouvic/txtanalytics/blob/main/tfidf_cos_sim.ipynb): Given a document name, it finds the top similar documents to the given one. It uses cosine similarity, which for normalized vectors amounts to dot-product. It outputs the top similar documents in terms of their similarity score, docid, and docname. E.g. if we input docname 'txts/Arbuckle-Christie-Siemens_IntroductionSRC7.2_11-15-16.txt', it outputs

<pre>
scoremult	docid	docname
0.351171	7	txts/Arbuckle-Mauro-Siemens_Intro-Sydney-Whist...
0.270747	6	txts/Arbuckle-Crompton-Mauro_SRC-intro_Dec14.txt
0.184882	5	txts/Arbuckle-Christie_Intersections-Between_S...
0.183604	12	txts/Arbuckle-et-al-2020-Introduction-Open-Sch...
0.150295	99	txts/Siemens-2016-Faster-Alone-Further-Togethe...
</pre>
