# Exercício Docker e GitHub Actions

Aplicação FastAPI com endpoint GET /hello.

Versões:
- 1.0: Hello World
- 2.0: Hello World 2

Imagens publicadas automaticamente no GHCR via GitHub Actions.

## Evidências de execução

### GitHub Actions
As duas pipelines foram executadas com sucesso:
- Versão 1.0: commit `117063e`
- Versão 2.0: commit `f3c6ecc`

Pipeline: https://github.com/filipesilva07/exercicio-docker-actions/actions

### Imagens publicadas no GHCR
- `ghcr.io/filipesilva07/hello-actions:1.0`
- `ghcr.io/filipesilva07/hello-actions:2.0`

### Validação local
As imagens foram baixadas do GHCR usando `docker pull` e executadas com `docker run`.

| Versão | Endpoint | Resposta |
|---|---|---|
| 1.0 | GET /hello | Hello World |
| 2.0 | GET /hello | Hello World 2 |
