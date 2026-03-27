# Projet TP 4 HBase et Spark


## Description du projet

Ce projet illustre l'intégration entre HBase et Apache Spark dans un environnement Hadoop exécuté avec Docker. L'objectif est de manipuler des données dans HBase et d'utiliser Spark pour effectuer des traitements distribués sur ces données.

## Technologies utilisées

Java, Apache HBase, Apache Spark, Apache Hadoop, Maven, Docker

## Structure du projet

hello-hbase : opérations de base sur HBase (création, insertion, lecture)
hbase-spark : intégration avec Spark et traitement distribué

## Commandes d'exécution

### Exécution HBase

java -cp "target/hello-hbase-1.0-SNAPSHOT.jar:lib/*" tn.insat.tp4.HelloHBase

### Exécution Spark

spark-submit --class tn.insat.tp4.HbaseSparkProcess --master yarn --deploy-mode client target/hbase-spark-1.jar

## Résultats

* Insertion : user1, user2
* Lecture des données réussie
* Nombre d'enregistrements : 4

## Environnement

Exécution dans Docker (conteneur hadoop-master avec Hadoop, HBase et Spark)

## Conclusion

Ce projet montre l'utilisation de HBase avec Spark pour traiter des données distribuées dans un environnement Big Data.
