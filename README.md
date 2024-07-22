# Teste Técnico para Desenvolvedor Sênior em IA

## Objetivo
Desenvolver uma aplicação que analisa sentimentos em reviews de produtos utilizando técnicas de IA. A aplicação deve ser construída seguindo os princípios de SOLID e Clean Code, com integração e deploy contínuos (CI/CD), e testes unitários e end-to-end (E2E). Além disso, deve utilizar Swagger para documentação da API. A principal linguagem será Python, com armazenamento de dados em MongoDB e MySQL.

## Parte 1: Configuração Inicial

### 1. Repositório e CI/CD
- Crie um repositório no GitHub ou GitLab.
- Configure um pipeline CI/CD utilizando GitHub Actions ou GitLab CI para automatizar build, testes e deploy.

## Parte 2: Desenvolvimento da Aplicação

### 2.1. Configuração do Ambiente
- Configure um ambiente virtual para o projeto utilizando `venv` ou `virtualenv`.
- Instale as dependências necessárias, incluindo bibliotecas para IA (como `scikit-learn` ou `nltk`), Flask, PyMongo para MongoDB, e MySQL connector para MySQL.
- Crie uma estrutura de diretórios organizada seguindo boas práticas de projetos Python.

### 2.2. Estrutura de Dados
- Utilize MongoDB para armazenar as reviews dos produtos.
- Utilize MySQL para armazenar informações de usuários e produtos.

### 2.3. Modelos e Serviços
- Crie modelos de dados seguindo os princípios de SOLID.
- Implemente serviços para CRUD de reviews, usuários e produtos.

### 2.4. Análise de Sentimentos
- Implemente uma função que analisa o sentimento de uma review utilizando técnicas de IA.
- Treine um modelo básico de análise de sentimentos utilizando um dataset público (como o IMDb reviews).

### 2.5. API RESTful
- Crie uma API RESTful utilizando Flask.
- Implemente endpoints para:
  - CRUD de reviews, produtos e usuários.
  - Análise de sentimentos de uma nova review.
- Documente a API utilizando Swagger.

## Parte 3: Testes

### 3.1. Testes Unitários
- Escreva testes unitários para as principais funções da aplicação utilizando `unittest` ou `pytest`.
- Garanta que todos os testes sejam executados no pipeline CI/CD.

### 3.2. Testes End-to-End (E2E)
- Escreva testes E2E para verificar o funcionamento completo da aplicação utilizando uma ferramenta como `Selenium` ou `Cypress`.
- Teste fluxos completos, como o envio de uma review e a análise de sentimento.

## Parte 4: Documentação

### 4.1. Documentação da API
- Documente todos os endpoints da API utilizando Swagger.
- Garanta que a documentação esteja disponível através de um endpoint `/swagger`.

## Entregáveis

1. **Repositório do Código**: Link para o repositório contendo todo o código fonte da aplicação.
2. **Pipeline CI/CD**: Configuração do pipeline CI/CD no repositório.
3. **Instruções de Configuração**: Instruções detalhadas sobre como configurar e executar a aplicação localmente.
4. **Documentação da API**: Documentação Swagger acessível no endpoint `/swagger`.
5. **Testes**: Testes unitários e E2E inclusos no repositório e executados no pipeline CI/CD.

## Critérios de Avaliação

1. **Qualidade do Código**: Adesão aos princípios de SOLID e Clean Code.
2. **Funcionalidade**: Implementação completa dos requisitos funcionais (CRUD, análise de sentimentos).
3. **CI/CD**: Pipeline configurado corretamente e executando testes.
4. **Testes**: Cobertura de testes unitários e E2E.
5. **Documentação**: Qualidade e completude da documentação da API.

---

## Exemplo de Estrutura de Projeto

```
my_app/
│
├── app/
│   ├── models/
│   │   ├── user.py
│   │   ├── product.py
│   │   └── review.py
│   ├── services/
│   │   ├── user_service.py
│   │   ├── product_service.py
│   │   └── review_service.py
│   ├── controllers/
│   │   ├── user_controller.py
│   │   ├── product_controller.py
│   │   └── review_controller.py
│   ├── utils/
│   │   └── sentiment_analysis.py
│   ├── __init__.py
│   └── app.py
│
├── tests/
│   ├── unit/
│   │   ├── test_user_service.py
│   │   ├── test_product_service.py
│   │   └── test_review_service.py
│   ├── e2e/
│   │   └── test_end_to_end.py
│   └── __init__.py
│
├── .github/
│   └── workflows/
│       └── ci_cd.yml
│
├── swagger/
│   └── swagger.yaml
│
├── requirements.txt
├── README.md
└── setup.py
```

## Instruções Adicionais

1. **Configuração do MongoDB e MySQL**
   - Forneça instruções claras sobre a configuração dos bancos de dados, incluindo exemplos de configuração no arquivo `app.py`.

2. **Swagger**
   - Inclua um arquivo `swagger.yaml` para a documentação da API.

3. **Pipeline CI/CD**
   - No arquivo `.github/workflows/ci_cd.yml`, configure o pipeline para instalar dependências, executar testes e realizar o deploy (se aplicável).
  
# Observação

Esse modelo não é necessariamente obrigatório. Caso queira fazer de outro jeito fique a vontade, mas explicando as alterações.
