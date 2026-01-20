# 📝 Tasks API – CRUD com Flask  
### API simples para gerenciamento de tarefas (To-Do List)

Este projeto é uma API em Python usando **Flask**, desenvolvida para fins de estudo: CRUD, boas práticas, testes automatizados com PyTest e documentação via Swagger/OpenAPI.

---

## 🚀 Funcionalidades Principais

- 🆕 Criar tarefas  
- 📄 Listar tarefas  
- 🔍 Buscar tarefa por ID  
- ✏️ Atualizar tarefa  
- 🗑️ Deletar tarefa  
- 🧪 Testes automatizados (PyTest)  
- 📘 Documentação com OpenAPI/Swagger  

---

## 🛠️ Tecnologias Utilizadas

- **Python 3**
- **Flask**
- **OpenAPI / Swagger**
- **PyTest**
- **Requests**

---

# ⚙️ Como Rodar o Projeto Localmente

## 📦 1. Clone o repositório

```bash
git clone https://github.com/seuusuario/tasks-flask-crud
cd tasks-flask-crud
```

## 📦 2. Crie e ative o ambiente virtual
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

## 📜 3. Instale as dependências
```bash
pip install flask pytest requests
```
## 🚀 4. Inicialize a API
```bash
python app.py
```

A API rodará em:
http://127.0.0.1:5000

## 📑 Documentação da API (Swagger)

A documentação pode ser aberta no Swagger Editor usando o arquivo:

## 📄 openapi.yaml

Ou acesse (caso esteja configurado no projeto):

## 📘 Swagger UI
```bash
http://127.0.0.1:5000/swagger
```
---

### 🛠️ Endpoints da API
## 📍 1. Criar tarefa

POST /tasks
```bash
Corpo da requisição:
{
  "title": "Minha tarefa",
  "description": "Descrição da tarefa"
}
```
Resposta:
```bash
{
  "message": "Nova tarefa criada com sucesso!",
  "id": 1
}
```
## 📍 2. Listar todas as tarefas
 
GET /tasks
```bash
Resposta:
{
  "tasks": [...],
  "total_tasks": 3
}
```
## 📍 3. Buscar tarefa por ID

GET /tasks/<id>

## 📍 4. Atualizar tarefa

PUT /tasks/<id>

Corpo da requisição:
```bash
{
  "title": "Título atualizado",
  "description": "Nova descrição",
  "completed": true
}
```
## 📍 5. Deletar tarefa

DELETE /tasks/<id>

Resposta:
```bash
{
  "message": "Tarefa removida com sucesso!"
}
```
### 🧪 Testes Automatizados (PyTest)

O arquivo tests.py valida:

✔️ Criação de tarefas
✔️ Listagem
✔️ Busca por ID
✔️ Atualização
✔️ Remoção

## ▶️ Executar testes:
pytest -v

## 🧱 Estrutura do Projeto
```plaintext
/
├── app.py                # API principal Flask
├── models/               # Modelos (ex.: Task)
├── openapi.yaml          # Documentação Swagger
├── tests.py              # Testes automatizados PyTest
├── requirements.txt      # Dependências
└── README.md             # Documentação do projeto
```
## 📜 Documentação OpenAPI

Toda a documentação da API está no arquivo:

## 📄 openapi.yaml

## Pode ser aberto no editor oficial:
🔗 https://editor.swagger.io/
---
## 👩‍💻 Autor

Desenvolvido por Gabriele Marciano
🎓 Projeto de estudo – 2025
💙 GitHub: https://github.com/gabrieleMarciano
