docker build -f .\src\ContainerSample\Dockerfile -t containerapi:0.1 .
docker run -it --rm -p 8888:80 containerapi:0.1
curl http://localhost:8888/WeatherForecast


kubectl delete service containerapi
kubectl delete service containerapi
kubectl apply -f .\build\k8.yml

kubectl get all
curl http://localhost:30181/WeatherForecast
