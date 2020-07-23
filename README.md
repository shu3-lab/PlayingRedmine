# PlayingRedmine

This is Docker Environment for playing and testing [REDMINE](https://redmine.jp/).

## Run by docker-compose

Run it by `docker-compose up --build` .

## Run by compose-on-kubernetes

1. Make local registory and push images(Confirm how to do [here](https://docs.docker.com/registry/))
2. Enable your Docker Desktop to use kubernetes cluster
3. run `docker stack deploy --orchestrator=kubernetes -c docker-compose.yml redmine`
4. And run `docker stack rm --orchestrator=kubernetes redmine` when stopping kubernetes cluster.

## Confirm kubernetes status

run `kubectl get services,pods,deployment,pvc,pv`

## Rough overview when using compose-on-kubernetes

<img width="850" alt="スクリーンショット 2020-07-23 22 25 39" src="https://user-images.githubusercontent.com/56756975/88291741-adbb9780-cd33-11ea-949c-24a684a8a94a.png">