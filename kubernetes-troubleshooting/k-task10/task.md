You are a junior engineer and have been asked to create a pod called pod-multi with two containers as given below:
i. --name=container1 , image name= nginx
ii. --name=container2 , image name= busybox, command:sleep 4800

dry run to generate nginx image file
k run container1 --image=nginx --dry-run=client -o yaml >pod-multi.yaml