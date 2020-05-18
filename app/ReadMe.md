## K8S部署Go App

### 编写Go App
### Docker化
```shell
# 构建镜像
docker build -f Dockerfile -t docker-registry.dhc:5000/k8s-go-app:1.0.0 .

# 推送到镜像中心
docker push docker-registry.dhc:5000/k8s-go-app:1.0.0

```
#### K8S deployment
```shell
kubectl apply -f k8s-deployment.yml

# 
kubectl get services
kubectl get pods
```


### 参考资料
+ [《Deploying a containerized Go app on Kubernetes》](https://www.callicoder.com/deploy-containerized-go-app-kubernetes/)