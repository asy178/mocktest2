ASHA DALILA MOCK TEST 2

CHECK 1:
1. nano 1.1-namespace.yaml
2. kubectl create -f 1.1-namespace.yaml
3. nano 1.2-deployment.yaml
4. kubectl create -n qq2 -f 1.2-deployment.yaml
5. kubectl get deployments -n qq2
6. kubectl get pods -n qq2

CHECK 2:
1. nano 2.2-deployment.yaml
2. kubectl create -n qq2 -f 2.2-deployment.yaml
3. kubectl scale -n qq2 deployments lab-deployment --replicas=4
4. kubectl get deployments -n qq2
5. kubectl get pods -n qq2

CHECK 3:
1. kubectl create -f 3.1-namespace.yaml
2. kubectl apply -n qq3 -f 3.2-deployment.yaml
3. kubectl set image deployment/nginx-deployment nginx=nginx:alpine -n qq3
4. kubectl describe deployment nginx-deployment -n qq3

CHECK 4:
1. kubectl create deployment apache-deployment --image=httpd:latest --dry-run=client -o yaml --namespace=qq3 > 4.2-deployment.yaml
2. kubectl apply -n qq3 -f 4.2-deployment.yaml
3. kubectl set image deployment/apache-deployment httpd=httpd:bookworm --namespace=qq3
4. kubectl rollout undo deployment/apache-deployment --namespace=qq3
5. kubectl rollout history deployment/apache-deployment --namespace=qq3

CHECK 6:
1. nano 6.3-daemonset.yaml
2. kubectl apply -n qq3 -f 6.3-daemonset.yaml
