# Fake Shop


## Variável de Ambiente
DB_HOST	=> Host do banco de dados PostgreSQL.

DB_USER => Nome do usuário do banco de dados PostgreSQL.

DB_PASSWORD	=> Senha do usuário do banco de dados PostgreSQL.

DB_NAME	=>	Nome do banco de dados PostgreSQL.

DB_PORT	=>	Porta de conexão com o banco de dados PostgreSQL.

## Desafio 2 - Kubernetes

Exercício prático feito durante Imersão DevOps && Cloud.

[Link do desafio](https://imersao.devopspro.com.br/desafio/desafio-devops-e-cloud/desafio-2-kubernetes/)

## Comandos

 ```
k3d cluster create -s 3 -a 3

kubectl api-resources

kubectl apply -f k8s/deployment.yaml

kubectl get pod

kubectl port-forward pod/postgre-7d876f754c-njjfx 5432:5432

 ```

## Desafio 3 - Pipeline CI/CD

[Link do desafio](https://imersao.devopspro.com.br/desafio/desafio-devops-e-cloud/desafio-3-pipeline-cicd/)

### Modo de usar
 A pipeline executa automaticamente no *push* da *branch* main.
 É necessário configurar os seguintes *secrets* do github no seu *fork*:
 - DOCKERHUB_USERNAME: O nome de usuário do DockerHub
 - DOCKERHUB_PASSWORD: O password de usuário do DockerHub
 - KS8_KUBECONFIG: Arquivo .kube/config do ambiente de deploy