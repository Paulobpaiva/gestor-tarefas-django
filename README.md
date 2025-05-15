# Sistema de Gestão de Tarefas com Autenticação

Este projeto é um sistema de gestão de tarefas desenvolvido em Django. Ele permite que os usuários façam o cadastro e login, criem tarefas, atualizem seus status e acompanhem sua produtividade por meio de gráficos interativos. 
## 🎯 **Funcionalidades**

* Cadastro e login de usuários.
* CRUD completo de tarefas com os seguintes status:

  * Pendente
  * Em andamento
  * Concluída
* Filtros por data e categoria.
* API REST básica utilizando Django REST Framework.
* Gráficos de produtividade usando Chart.js.
* Notificações no Telegram para novas tarefas e mudanças de status.

---

## 🚀 **Diferenciais**

* Integração com o Telegram para envio de notificações em tempo real.
* Visualização de produtividade por meio de gráficos dinâmicos utilizando Chart.js.

---

## ✅ **Instalação**

1. Clone o repositório:

   ```bash
   git clone https://github.com/Paulobpaiva/gestao-tarefas.git
   cd gestao-tarefas
   ```

2. Crie um ambiente virtual:

   ```bash
   python -m venv env
   source env/bin/activate  # Linux/Mac
   .\env\Scripts\activate  # Windows
   ```

3. Instale as dependências:

   ```bash
   pip install -r requirements.txt
   ```

4. Realize as migrações:

   ```bash
   python manage.py migrate
   ```

5. Crie um superusuário:

   ```bash
   python manage.py createsuperuser
   ```

6. Execute o servidor:

   ```bash
   python manage.py runserver
   ```

---

## 🔧 **Configuração do Telegram**

1. Crie um bot no Telegram via [BotFather](https://t.me/BotFather) e obtenha o token.

2. Adicione o token no arquivo `.env`:

   ```env
   TELEGRAM_TOKEN=SEU_TOKEN
   ```

3. Defina o ID do chat onde as notificações serão enviadas:

   ```env
   TELEGRAM_CHAT_ID=SEU_CHAT_ID
   ```

---

## 📊 **Uso dos Gráficos**

Os gráficos de produtividade são gerados automaticamente e podem ser acessados na página principal após o login. Eles exibem a quantidade de tarefas por status e a produtividade diária/semana.

---

## 🛠️ **Tecnologias Utilizadas**

* Python
* Django
* Django REST Framework
* Chart.js
* Telegram API

---

## 📦 **Contribuições**

Sinta-se à vontade para abrir issues, enviar PRs ou sugerir melhorias.

---

## 📜 **Licença**

Este projeto está licenciado sob a MIT License. Consulte o arquivo LICENSE para mais detalhes.
