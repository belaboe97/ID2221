.# Delivery for ID2221 - Data-intensive computing
## Twitter Streaming API with Kafka, Spark Streaming, Cassandra

[![N|Solid](https://www.liveinlab.kth.se/polopoly_fs/1.1065101.1618224951!/image/kth%20logo%20vit%20platta.jpg)](https://nodesource.com/products/nsolid)

## Prerequisites for running the code: 


| Plugin | README |
| ------ | ------ |
| Java | [plugins/dropbox/README.md][PlDb] |
| Anaconda | [plugins/github/README.md][PlGh] |
| Kafka | [plugins/googledrive/README.md][PlGd] |
| Cassandra | [plugins/onedrive/README.md][PlOd] |

Anaconda provides: Python, Jupyter-Notebook etc. 

## Steps to run the application: 

### Start Kafka (in kafka folder)


<ol>
  <li>bin/zookeeper-server-start.sh config/zookeeper.properties</li>
  <li>bin/kafka-server-start.sh config/server.properties</li>
  <li> bin/kafka-topics.sh --create --topic saCity --bootstrap-server localhost:9092</li>
</ol> 

#### Run TwttrStreamingAPI.ipynb  
Required libraries: time, tweepy, kafka

### Start Cassandra (in cassandra folder) with bin/cassandra -f

### Run Section 1: Cassandra Setup in CassandraSetupAndDataVisualization.ipynb
Required libraries: cassandra-driver, matplotlib, pandas

### Run SparkStreamToCassandra.ipynb
Required libaries: pyspark, textblob

### Run Section2: Data Visualization in CassandraSetupAndDataVisualization.ipynb

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
