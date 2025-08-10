  I. Create a Resource Quota called “reqQuota '' with hard limits of 1 CPU,!G memory and  pods without creating it.
Ii. Get pods on all namespaces

kubectl create quota reqQuota --hard=cpu=1,memory=1G,pods=2 --dry-run=client --validate -o yaml > 5.yaml (task i)

k get pods -A(task ii)