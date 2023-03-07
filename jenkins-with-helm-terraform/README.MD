## 1. 
```
helm repo add jenkins https://charts.jenkins.io
```

## 2. 
```
helm search repo jenkins
```

## 3. 
```
kubectl create ns jenkins
```

## 4. 
```
helm pull jenkins/jenkins --untar=true
```

## 5. Customize your local values and install 
```
helm install jenkins ./jenkins  --values=myvalues.yml --namespace=jenkins
```