# 📋 To-Do List API

Uma **API RESTful** simples para gerenciamento de tarefas (To-Do List) construída com **Python + Django + Django REST Framework**.

---

## 🚀 **Funcionalidades**

- ✅ **Criar tarefas**
- ✅ **Listar tarefas**
- ✅ **Atualizar tarefas**
- ✅ **Marcar como concluídas**
- ✅ **Excluir tarefas**

---

## ⚙️ **Tecnologias**

- [Python](https://www.python.org/)
- [Django](https://www.djangoproject.com/)
- [Django REST Framework](https://www.django-rest-framework.org/)

---

## 📂 **Como rodar o projeto**

1. **Clone o repositório**
   ```bash
   git clone https://github.com/GustavoRizerioDev/lista-de-tarefas.git
   cd lista-de-tarefas
   ```

2. **Crie e ative um ambiente virtual**
   ```bash
    python -m venv venv
    source venv/bin/activate  
    venv\Scripts\activate    
   ```

3. **Instale as dependências**
   ```bash
    pip install -r requirements.txt   
   ```

4. **Aplique as migrações**
   ```bash
    python manage.py migrate   
   ```

5. **Rode o servidor**
   ```bash
    python manage.py runserver 
   ```

6. **Acesse**
- **API**: http://127.0.0.1:8000/api/tasks/
- **Admin**: http://127.0.0.1:8000/admin/



## 🔑 **Exemplos de requisições**

**Criar tarefa**
   ```bash
    POST /api/tasks/
    Body: 
    {
     "title": "Nova tarefa",
     "completed": false
    }
   ```
---
**Atualizar tarefa**
   ```bash
    PATCH /api/tasks/<id>/
    Body: 
    {
     "completed": true
    }
   ```