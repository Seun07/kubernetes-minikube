# create a pod in yaml but the output should be in output.yaml, container name nginxweb1, image nginx
# imperative command
k run nginxweb1 --image nginx -o yaml > output.yaml
# dry run
 kubectl run nginxweb2 --image=nginx --dry-run=client -o yaml >output3.yaml
 # exec to container
 k exec -it nginxweb2 -- sh #and type# ls
 k exec -it nginx1 -n myspace -- sh
 # create busybox pod
 k run busybox --image=busybox --command --restart=Never -it -- ls