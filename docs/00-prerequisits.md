# 00 - Pré-requisitos para o KMD

## Amazon Web Services
Este tutorial utiliza a plataforma de núvem da [Amazon Web Services](https://aws.amazon.com/) para provisionar a infraestrutura de computação necessária para inicializar um cluster Kubernetes desde o início (from scratch).

> O provisionamento de recursos no ambiente AWS pode incorrer em custos, portanto utilize a calculadora antes de iniciar o provisionamento de qualquer componente.

## AWS CLI

### 00.01 - Instalando o AWS CLI (Command Line Interface) no seu desktop/laptop.

Siga a documentação do [AWS CLI](https://aws.amazon.com/cli) para instalar e configurar o utilitário de linha de comando da `aws`.

Verificar se o AWS CLI está instalado corretamente:

```
aws --version
```
OBS: No momento da elaboração deste documento eu utilizo a versão 1.16.130.

> saída
```
aws-cli/1.16.130 Python/2.7.16 Darwin/19.3.0 botocore/1.12.120
```

### 00.02 - Definir uma Região padrão
Definir a região padrão através dos dois comandos abaixo. Neste exemplo considero a utilização da região sa-east-1, ou seja South America - São Paulo.
```
AWS_REGION=sa-east-1
```
```
aws configure set default.region $AWS_REGION
```

Próximo: [Instalando os Client Tools](01-client-tools.md)
