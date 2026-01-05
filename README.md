# Sistema de Gestão de Estoque (SGE)

O **Sistema de Gestão de Estoque (SGE)** é uma aplicação web desenvolvida em **Django**, projetada para o controle de produtos, fornecedores e movimentações de entrada e saída, com foco em organização operacional, escalabilidade e integração com APIs e BI.

O projeto foi estruturado de forma modular, seguindo boas práticas de arquitetura backend, e serve como base para sistemas corporativos de pequeno e médio porte.

---

## 🧩 Principais Funcionalidades

- Gestão de Produtos, Marcas e Categorias
- Controle de Fornecedores
- Registro de Entradas e Saídas de Estoque
- Controle de preços (custo e venda)
- Autenticação e permissões via Django Auth
- API REST com JWT para integrações externas
- Estrutura preparada para expansão financeira e BI

---

## 🏗️ Arquitetura do Projeto

O sistema é organizado por domínios independentes:

- `authentication` – autenticação e controle de acesso
- `products` – cadastro e gestão de produtos
- `brands` – marcas
- `categories` – categorias de produtos
- `suppliers` – fornecedores
- `inflows` – entradas de estoque
- `outflows` – saídas de estoque
- `ai` – módulo experimental para futuras automações

Essa separação facilita manutenção, testes e evolução do sistema.

---

## 🔐 Segurança e Autenticação

- Autenticação baseada no Django Auth
- Controle de permissões por modelo
- API protegida com JWT (`SimpleJWT`)
- Configurações sensíveis isoladas em variáveis de ambiente

---

## ⚙️ Tecnologias Utilizadas

- Python 3.8+
- Django 5
- Django Rest Framework
- Simple JWT
- SQLite (desenvolvimento)
- PostgreSQL (produção)
- Bootstrap 5
- Docker (opcional)

---

## 🚀 Execução Local

### 1. Criar e ativar o ambiente virtual
```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
