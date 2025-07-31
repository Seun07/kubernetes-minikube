k apply -f deployment.yaml -n test

k get deployment -n test
k get pods
k get pods -n test
k create namespace test
k describe pod nginx-deployment-647677fc66-q6t4n -n test
k apply -f service.yaml -n test
k get svc -n test
k delete deployment nginx-deployment -n test
k run nginxweb1 --image nginx -o yaml > output.yaml