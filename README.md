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
