# Jenkins Installation
## 1. Step 1: Create a Namespace for Jenkins. It is good to categorize all the DevOps tools as a separate namespace from other applications.
```
kubectl create namespace devops-tools
```

## 2. Apply 1-role-service-account.yml.
```
kubectl apply -f 1-role-service-account.yml
```

## 3. Apply 2-storage.yml 
```
kubectl create -f 2-storage.yaml
```

## 4. Apply 3-jenkins-deploy.yml
```
kubectl create -f 3-jenkins-deploy.yml
```

## 5. Expose jenkins deployment
```
kubectl apply -f 4-jenkins-lb-service.yml
```