kind create cluster --name kind-cassandra --config ./kind-config.yaml

kubectl -n cass-operator apply -f ./storageclass-kind.yaml

kubectl -n cass-operator apply -f ./cassandra/install-cass-operator-v1.3.yaml

kubectl -n cass-operator apply -f ./cassandra/cassandra-cluster-1nodes.yaml


kubectl -n cass-operator apply -f ./cassandra/cassandra-cluster-3nodes.yaml


https://github.com/DataStax-Academy/cassandra-workshop-series


https://kind.sigs.k8s.io/docs/user/quick-start/


https://github.com/DataStax-Academy/cassandra-workshop-series/tree/master/week5-Cass-in-k8s

https://github.com/DataStax-Academy/cassandra-workshop-series/blob/master/week5-Cass-in-k8s/README_CASSANDRA.MD

https://github.com/DataStax-Academy/cassandra-workshop-series/tree/master/week5-Cass-in-k8s

https://github.com/DataStax-Academy/cassandra-workshop-series/tree/master/week5-Cass-in-k8s

https://github.com/DataStax-Academy/cassandra-workshop-series

https://medium.com/@kayaerol84/cassandra-cluster-management-with-docker-compose-40265d9de076