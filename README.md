# Terraform AWS Modulo-Local

Este projeto é um módulo de Terraform que permite fazer o deploy de uma VM na AWS utilizando o módulo de rede criado pelo usuário.

## Pré-requisitos

- Conta na AWS
- Acesso à chave de acesso e chave secreta da AWS
- Terraform instalado na máquina local

## Utilização

1. Clone o repositório para a sua máquina local: git clone https://github.com/seu-usuario/terraform_aws_modulo-local.git
2. Acesse a pasta do projeto: cd terraform_aws_modulo-local
3. Crie um arquivo chamado terraform.tfvars e adicione as seguintes variáveis:

- aws_access_key: sua chave de acesso da AWS
- aws_secret_key: sua chave secreta da AWS
  a- ws_region: a região da AWS onde a VM será criada
- aws_vpc_id: o ID da VPC na qual a VM será criada
- aws_subnet_id: o ID da subrede na qual a VM será criada

4. Execute o comando `terraform init` para baixar os módulos necessários.
5. Execute o comando `terraform plan` para visualizar as alterações que serão feitas na sua conta da AWS.
6. Execute o comando `terraform apply` para aplicar as alterações e criar a VM.

## Considerações finais

Lembre-se de sempre executar o comando `terraform destroy` quando quiser excluir a VM e todos os recursos criados pelo Terraform.
