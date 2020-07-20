# PlayingRedmine

This is Docker Environment for playing and testing [REDMINE](https://redmine.jp/).

## Run by docker-compose

Run it by `docker-compose up --build` .

## Run by compose-on-kubernetes

1. Make local registory and push images(Confirm how to do [here](https://docs.docker.com/registry/))
2. Enable your Docker Desktop to use kubernetes cluster
3. run `docker stack deploy --orchestrator=kubernetes -c docker-compose.yml redmine`

## Confirm kubernetes status

run `kubectl get services,pods,deployment,pvc,pv`
