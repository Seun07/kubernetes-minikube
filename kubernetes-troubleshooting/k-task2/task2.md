I. Create a single pod of image httpd:alpine3.20 in namespace application (check if namespace exist or not)
Pls the pod should be name web1 and the container should be name web-container

Ii. Write  a shell script to output the status of the pod

k -n application get pod1 web1  -o yaml

K -n application get pod web1  -o json

k -n application get pod web1  -o jsonpath={.status}
K -n application get pod1 web1  -o jsonpath={.status.phase}
vi web1-status.sh and dump the command in line11 with #!/bin/bash