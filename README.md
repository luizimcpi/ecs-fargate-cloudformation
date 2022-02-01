# Cloudformation ECS Fargate Stack

## Requisitos
```
-Conta aws criada
-ecsTaskExecutionRole no IAM (https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_execution_IAM_role.html)

IMPORTANTE
*Este projeto está utilizando uma imagem publica do ECR que utiliza spring boot,
caso queira utilizar uma imagem própria fazer o upload para o ECR e substituir no arquivo my-template.yml a linha 'Image' pelo endereço da sua imagem docker.
*As subnets e VpcID também deverão ser substituídas pelas informações da conta da aws no arquivo my-template.yml
```

## Como executar
```
Criar uma nova stack no cloud formation, escolhendo a opção 'Template is ready' e na área 'Specify template' selecione 'Upload a template file', escolha o arquivo my-template.yml
```

## Teste
```
Obter o ip publico ou dns do alb criado e chamar no navegador ou via Postman GET /hello
```