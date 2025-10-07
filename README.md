Claro, Miguel! Aqui está uma versão mais bonita e organizada do seu README, com emojis, seções bem destacadas e uma linguagem mais envolvente para facilitar a leitura e causar uma ótima impressão:

---

# 🎓 API de Gerenciamento Escolar

Sistema desenvolvido para facilitar o controle de dados escolares, incluindo professores, turmas e alunos. A API segue boas práticas de desenvolvimento e conta com validações específicas para cada entidade.

---

## 👥 Integrantes

| Nome                          | RA      |
|-------------------------------|---------|
| Paulo Henrique Pires Cordeiro | 2402602 |
| Gustavo Meirelles Festa       | 2403079 |
| Miguel Condello Liando        | 2403877 |

---

## 📌 Descrição

Esta API foi criada com o objetivo de simplificar o gerenciamento escolar. Ela permite:

- Cadastro e controle de professores
- Organização de turmas
- Associação de alunos às turmas
- Cálculo de médias e acompanhamento de desempenho

Tudo isso com uma interface documentada e fácil de usar!

---

## 🛠️ Tecnologias Utilizadas

- 🐍 Python 3  
- 🔥 Flask  
- 🧮 Flask-SQLAlchemy  
- 📘 Flasgger (Swagger)  
- 🗃️ SQLite  
- 🐳 Docker  

---

## 🚀 Como Executar

### 🐳 Utilizando Docker

1. Certifique-se de ter o Docker instalado.
2. No diretório do projeto, construa a imagem:
   ```bash
   docker build -t flask-api .
   ```
3. Rode o container:
   ```bash
   docker run -p 5002:5002 flask-api
   ```
4. Acesse a documentação interativa:  
   👉 [http://localhost:5002/apidocs](http://localhost:5002/apidocs)

---

### 🐍 Utilizando Python diretamente

1. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
2. Execute o servidor:
   ```bash
   python app.py
   ```
3. Acesse a documentação interativa:  
   👉 [http://localhost:5002/apidocs](http://localhost:5002/apidocs)

---

## 🧩 Estrutura das Entidades

| Entidade   | Atributos |
|------------|-----------|
| **Professor** | id, nome, idade, matéria, observações |
| **Turma**     | id, descrição, ativo, professor_id |
| **Aluno**     | id, nome, idade, turma_id, data_nascimento, nota_primeiro_semestre, nota_segundo_semestre, media_final |

---

## 🔗 Endpoints Principais

- `GET /professores/` – Listar professores  
- `POST /professores/` – Criar novo professor  
- `GET /turmas/` – Listar turmas  
- `POST /turmas/` – Criar nova turma  
- `GET /alunos/` – Listar alunos  
- `POST /alunos/` – Criar novo aluno  

---

## 📚 Documentação Swagger

A API conta com documentação automática via Swagger, detalhando todos os endpoints, parâmetros e exemplos de uso.  
📍 Basta acessar: `/apidocs` após iniciar o servidor.

---
