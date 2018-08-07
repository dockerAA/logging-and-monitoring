# logging

# docker swarm manager config 
$ echo 'vm.max_map_count=262144' | sudo tee -a /etc/sysctl.conf <br>
$ sudo sysctl -p

<br>
<br>

# Docker Container List (logging)
1. docker.elastic.co/elasticsearch/elasticsearch:6.2.3 (9200:9200) <br>
2. docker.elastic.co/logstash/logstash:6.2.3 (syslog port => 51415) <br>
3. docker.elastic.co/kibana/kibana:6.2.3 (9080:5601) <br>
4. gliderlabs/logspout:v3.2.4 <br>
# Docker Container List (monitoring)
1. google/cadvisor:latest (# 8080:8080) <br>
2. basi/node-exporter:v1.13.0 <br>
3. prom/prometheus:v1.8.2 (9070:9090) <br>
4. grafana/grafana:5.1.2 (9030:3000) <br> 

