# Provisionamento de Servidor com Ansible

Este projeto demonstra como utilizar o Ansible para realizar o provisionamento básico de um servidor Linux. As tarefas incluem:

- Instalação de um servidor web (Apache)
- Criação de usuários
- Definição de permissões em diretórios

## 📦 Estrutura do Projeto

```
provisionamento-servidor/
├── inventory.ini
├── playbook.yml
└── roles/
    ├── webserver/
    │   └── tasks/main.yml
    ├── usuarios/
    │   └── tasks/main.yml
    └── permissao/
        └── tasks/main.yml
```

## 🚀 Como Executar

1. Configure o arquivo `inventory.ini` com o IP do servidor e credenciais de acesso.
2. Execute o playbook com o comando:

```bash
ansible-playbook -i inventory.ini playbook.yml
```

## 📚 Conceitos Envolvidos

- **Infraestrutura como Código (IaC)**: Automatiza a configuração de servidores.
- **Sintaxe declarativa**: Define o estado desejado da infraestrutura.
- **Idempotência**: Garante que múltiplas execuções não causem efeitos colaterais.

## 🧰 Requisitos

- Ansible instalado na máquina local
- Acesso SSH ao servidor remoto

## 📄 Licença

Este projeto está licenciado sob os termos da licença MIT.