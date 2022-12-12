PS C:\Users\louis\cour devops\TP - WIK-DPS-TP04> kubectl port-forward echo 8888:8080
Forwarding from 127.0.0.1:8888 -> 8080
Forwarding from [::1]:8888 -> 8080
Handling connection for 8888
Handling connection for 8888
Handling connection for 8888

PS C:\Users\louis\cour devops\TP - WIK-DPS-TP04> kubectl apply -f .\podReplica.yaml
replicaset.apps/frontend created
PS C:\Users\louis\cour devops\TP - WIK-DPS-TP04> kubectl get pod
NAME READY STATUS RESTARTS AGE
frontend-4hhjf 1/1 Running 0 26s
frontend-fl48h 1/1 Running 0 26s
frontend-sxj67 1/1 Running 0 26s
frontend-w48rn 1/1 Running 0 26s
