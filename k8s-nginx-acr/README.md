# 
https://github.com/MicrosoftDocs/azure-docs/blob/main/articles/container-registry/container-registry-auth-kubernetes.md

kubectl create namespace <namespace>
kubectl create secret docker-registry <secret-name> \
    --namespace <namespace> \
    --docker-server=<container-registry-name>.azurecr.io \
    --docker-username=<service-principal-ID> \
    --docker-password=<service-principal-password>


kubectl create namespace k8s-nginx-acr

kubectl create secret docker-registry acr-secret \
    --namespace k8s-nginx-acr \
    --docker-server=ecvtwsa.azurecr.io \
    --docker-username=ecvtwsa \
    --docker-password=ePsD0lrwpMiPafVyRbTR2zSLUV83myzjVxkN3bu/yT+ACRCnabxM