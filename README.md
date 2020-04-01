<h1>APACHE KAFKA POC ON KUBERNETES With Java producer consumer</h1>

<p>
These project is to do a POC on how to install and configure apache kafka / zookeeper / kafka connect on kubernetes (I have used Docker desktop single node kubernetes cluster) all configuration file are in the kube-config folder , once the setup is done , then test using the default kafka producer / consumer or use conduktor.io desktop kafka client to test the settings. These is bare project and doesn't have any security channels for communication.These is a single node broker , but once can create multi node broker.

Then one can use the java project to run the kafka producer / consumer .
<p>

<h2>Kubernetes scripts<h2>
```bash
kubectl create -f kube-config/zookeeper.yml
kubectl create -f kube-config/kafka-service.yml
kubectl create -f kube-config/kafka-broker.yml

kubectl port-forward <kafka-broker-pod-name> 9092

<h2>Kafka Producer Consumer</h2>
<h3>kafkacat: Linux based producer consumer</h3>
<p>
</p>
<h3>conduktor.io : Desktop client</h3>
<p>
</P>
