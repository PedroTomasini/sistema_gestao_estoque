Com base na estrutura de pastas que você forneceu, aqui está uma versão aprimorada do README, detalhando melhor os módulos do projeto:

---

# Sistema de Gestão de Estoque (SGE)

Este é um projeto de Sistema de Gestão de Estoque (SGE), desenvolvido para facilitar o controle e monitoramento de produtos, fornecedores, marcas, categorias, entradas e saídas de estoque, com visualizações e gráficos para análise de vendas e lucro. O sistema inclui autenticação e permissões de usuários para garantir a segurança e controle de acesso.

## Funcionalidades

- **Dashboard**: Visão geral das principais métricas de estoque, incluindo:
  - Quantidade de produtos
  - Custo e valor do estoque
  - Lucro estimado do estoque
  - Quantidade e valor das vendas
  - Lucro das vendas
- **Autenticação e Controle de Acesso**: Autenticação de usuário e permissões para garantir acesso seguro.
- **Gestão de Fornecedores**: Cadastro e gerenciamento de fornecedores para o estoque.
- **Marcas e Categorias**: Organização dos produtos por marcas e categorias.
- **Produtos**: Cadastro, edição e exclusão de produtos no estoque.
- **Entradas e Saídas**: Controle de movimentações de estoque, registrando entradas e saídas de produtos.
- **Gráficos e Relatórios**:
  - Gráfico de valor de vendas dos últimos 7 dias
  - Quantidade de vendas diárias
  - Distribuição de produtos por categoria e marca

## Estrutura do Projeto

- **authentication**: Módulo responsável pela autenticação e controle de permissões dos usuários.
- **brands**: Gerenciamento das marcas dos produtos.
- **categories**: Gerenciamento das categorias dos produtos.
- **core**: Contém configurações e funcionalidades centrais do projeto.
- **inflows**: Gerenciamento de entradas de produtos no estoque.
- **outflows**: Gerenciamento de saídas de produtos do estoque.
- **products**: Módulo principal para o cadastro e gerenciamento dos produtos.
- **suppliers**: Gerenciamento de fornecedores.

## Tecnologias Utilizadas

- **Backend**: Django
- **Frontend**: Django Templates, Bootstrap 5 e JavaScript
- **Banco de Dados**: SQLite (pode ser adaptado para outro banco, como PostgreSQL ou MySQL)
- **Bibliotecas e Ferramentas**:
  - Controle de autenticação e permissões de usuários
  - Gráficos e visualizações para relatórios

## Pré-requisitos

- Python 3.x
- Pip (gerenciador de pacotes do Python)

## Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/PedroTomasini/sistema_gestao_estoque.git
   ```

2. Acesse a pasta do projeto:
   ```bash
   cd sistema_gestao_estoque
   ```

3. Crie um ambiente virtual e ative-o:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows: venv\Scripts\activate
   ```

4. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

5. Configure as variáveis de ambiente e o banco de dados.

6. Execute as migrações para configurar o banco de dados:
   ```bash
   python manage.py migrate
   ```

7. Crie um superusuário para acesso administrativo:
   ```bash
   python manage.py createsuperuser
   ```

8. Inicie o servidor:
   ```bash
   python manage.py runserver
   ```

## Uso

1. Acesse o sistema no navegador em `http://127.0.0.1:8000`.
2. Faça login com as credenciais de administrador para acessar todas as funcionalidades.
3. Navegue pelo menu lateral para gerenciar produtos, fornecedores, categorias, marcas e visualizar relatórios.

## Desenvolvimento

Durante o desenvolvimento, você pode usar o arquivo `requirements_dev.txt` para instalar pacotes adicionais de desenvolvimento:

```bash
pip install -r requirements_dev.txt
```

## Contribuição

1. Faça um fork do projeto.
2. Crie uma nova branch para a sua feature: `git checkout -b feature/nova-feature`.
3. Commit suas mudanças: `git commit -m 'Adiciona nova feature'`.
4. Envie para a branch principal: `git push origin feature/nova-feature`.
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a [Nome da Licença]. Veja o arquivo `LICENSE` para mais detalhes.

---

Esse README fornece uma visão geral do projeto e instruções detalhadas para instalação e uso. Se precisar de ajustes adicionais, estou à disposição!
