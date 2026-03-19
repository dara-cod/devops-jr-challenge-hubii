# Segurança do Projeto

## Gerenciamento de Segredos
- Utilizar ferramentas como AWS Secrets Manager ou Kubernetes Secrets
- Nunca versionar credenciais no Git

## Proteção de Credenciais
- Uso de variáveis de ambiente
- Integração com IAM Roles

## Segurança da Imagem Docker
- Uso de imagem base slim
- Execução como usuário não-root
- Scan de vulnerabilidades com Trivy

## Boas práticas em Cloud
- Princípio do menor privilégio (IAM)
- Uso de VPC privada
- Logs e monitoramento habilitados