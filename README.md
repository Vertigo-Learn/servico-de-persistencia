# servico-de-persistencia

## Gerando a imagem da aplicacao

```shell script
./mvnw package

 docker build -f src/main/docker/Dockerfile.jvm -t <docker-hub-user>/servico-de-persistencia .
 docker push <docker-hub-user>/servico-de-persistencia

```

## Instalando no Kubernetes

```shell script
kubectl apply -f ./kubernetes/deployment.yaml
kubectl apply -f ./kubernetes/service.yaml

```