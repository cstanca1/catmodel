# catmodel
CAT Modeling Leveraging Open Source, e.g. QGIS, GeoServer, GeoMesa and Hortonworks Data Platforms

Project structure:

/data includes country/state/county boundaries and hurricane track data for 154 years.

/zeppelin includes an example of zeppelin notebook leveraging zeppelin-leaflet to display a filtered on-hurricane track on US map

/nifi includes flows to load, index and post with GeoMesa geospatial NiFi processors (to HBase, HDFS, Kafka).

/qgis includes a multi-layer project displaying hurricanes for 154 years on US map. This project needs to point to the actual location of the data and it can be run as standalone QGIS and as QGIS connected to GeoServer which is connected to HBase leveraging GeoMesa framework.

/R includes an example of an analytical visualization of disasters impact on people and property. This could be executed locally, but it can also leverage data stored in HBase and accessed via GeoServer/GeoMese/SparkSQL querying HBase-stored data

Environment setup followed the instruction presented at: www.geomesa.org, e.g.:

https://www.geomesa.org/documentation/user/hbase/install.html

https://www.geomesa.org/documentation/user/kafka/install.html

https://www.geomesa.org/documentation/user/nifi.html

https://www.geomesa.org/documentation/user/spark/sparksql.html

Quick start examples:

https://www.geomesa.org/documentation/tutorials/geomesa-quickstart-hbase.html

https://www.geomesa.org/documentation/tutorials/geomesa-quickstart-kafka.html

