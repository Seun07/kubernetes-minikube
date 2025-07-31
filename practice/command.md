# create a pod in yaml but the output should be in output.yaml, container name nginxweb1, image nginx
k run nginxweb1 --image nginx -o yaml > output.yaml
