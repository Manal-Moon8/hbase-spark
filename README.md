# Projet TP 4 HBase et Spark

## Description du projet

Dans ce TP, j’ai réalisé une intégration entre HBase et Apache Spark dans un environnement Hadoop exécuté avec Docker. L’objectif était de manipuler des données dans HBase (création de table, insertion et lecture) puis d’utiliser Spark pour traiter ces données.

## Technologies utilisées

Java, Apache HBase, Apache Spark, Apache Hadoop, Maven, Docker

## Structure du projet

hello-hbase : contient les opérations de base sur HBase (création de table, insertion des données, lecture)

hbase-spark : contient l’intégration avec Spark pour lire les données depuis HBase et effectuer un traitement distribué

## Commandes d'exécution

### Exécution HBase

java -cp "target/hello-hbase-1.0-SNAPSHOT.jar:lib/*" tn.insat.tp4.HelloHBase

### Exécution Spark

spark-submit --class tn.insat.tp4.HbaseSparkProcess --master yarn --deploy-mode client target/hbase-spark-1.jar

## Résultats

* Insertion de données (user1, user2)
* Lecture correcte des données depuis HBase
* Nombre total d’enregistrements : 4

## Environnement

Le projet a été exécuté dans un conteneur Docker (hadoop-master) contenant Hadoop, HBase et Spark.

## Conclusion

Ce TP m’a permis de comprendre comment intégrer HBase avec Spark et comment traiter des données de manière distribuée dans un environnement Big Data.
