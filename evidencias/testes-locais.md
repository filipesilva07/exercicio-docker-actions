# Evidências — Docker e GitHub Actions

## Repositório
https://github.com/filipesilva07/exercicio-docker-actions

## Pipelines executadas com sucesso

- Versão 1.0: https://github.com/filipesilva07/exercicio-docker-actions/actions/runs
- Versão 2.0: https://github.com/filipesilva07/exercicio-docker-actions/actions

## Imagens publicadas
- ghcr.io/filipesilva07/hello-actions:1.0
- ghcr.io/filipesilva07/hello-actions:2.0

## Validação das imagens baixadas do GHCR

### Versão 1.0
```text
$ docker pull ghcr.io/filipesilva07/hello-actions:1.0
1.0: Pulling from filipesilva07/hello-actions
Digest: sha256:66d06986fe4cfbf89f5b6a7963134ee45e79cab784712a6beb60d458d38c1cf5
Status: Image is up to date for ghcr.io/filipesilva07/hello-actions:1.0
ghcr.io/filipesilva07/hello-actions:1.0
$ curl http://localhost:8080/hello
"Hello World"
```

### Versão 2.0
```text
$ docker pull ghcr.io/filipesilva07/hello-actions:2.0
2.0: Pulling from filipesilva07/hello-actions
881fc932939e: Pulling fs layer
497083c8cda2: Pulling fs layer
aa121b1b1cdb: Pulling fs layer
113b91713f05: Pulling fs layer
cc36311dc778: Pulling fs layer
8a6aaa514228: Pulling fs layer
12713a10b83a: Pulling fs layer
ca551e87b631: Pulling fs layer
cc36311dc778: Already exists
44136fa355b3: Already exists
881fc932939e: Already exists
113b91713f05: Already exists
aa121b1b1cdb: Already exists
497083c8cda2: Download complete
8a6aaa514228: Download complete
12713a10b83a: Download complete
8a6aaa514228: Pull complete
12713a10b83a: Pull complete
df1c0293b815: Download complete
ca551e87b631: Download complete
497083c8cda2: Pull complete
ca551e87b631: Pull complete
Digest: sha256:e3ea723c4629cf88fb2c4a5817dd23210095e378bc538eb23a03d75c93118d39
Status: Downloaded newer image for ghcr.io/filipesilva07/hello-actions:2.0
ghcr.io/filipesilva07/hello-actions:2.0
$ curl http://localhost:8080/hello
"Hello World 2"
```
