[https://github.com/ajeetraina/kubernetes101/blob/master/concept/day-1/getting-started.adoc](https://github.com/ajeetraina/kubernetes101/blob/master/concept/day-1/getting-started.adoc)

POD
create pod
     `kubectl create -f templates/pod.yaml`
    
 Get list of pod
   `  kubectl get pods`
  
  check pod came up fine 
     ` kubectl -n default port-forward $(kubectl -n default get pod -l name=nginx-pod -o jsonpath='{.items[0].metadata.name}') 8080:80`
     
 Delete pod
 
     `kubectl delete -f templates/pod.yaml`
     
     
 Deployement
        ` kubectl create -f templates/deployment.yaml --record`
     
     
     