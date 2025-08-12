1.Create a pod with image nginx with image called nginimage expose traffic on port 80
(k run nginimage --image=nginx --port=80)
2.change port image to nginx:1.7.1
(k set image pod nginimage nginimage=nginx:1.7.1)
3.get nginx pod Ip created in question 2 above
(k run nginx4 --image=nginx --env="myval1=myval1")
(k exec -it nginx4 -- sh)
4. Create an nginx pod and set an env value of ‘myval1=myval1’, check the env val