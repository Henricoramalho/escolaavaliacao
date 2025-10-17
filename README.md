# 🧑‍🏫 Avaliação Prática — Sistema de Gerenciamento de Turmas e Atividades

### 🎯 Objetivo
O propósito deste projeto é desenvolver um **sistema web completo (full-stack)** voltado ao gerenciamento de turmas e atividades de professores.  
A aplicação deve permitir que docentes **cadastrem, visualizem e removam** suas turmas e atividades de forma simples e eficiente.  

---

## 📚 Contexto
A desorganização no controle das atividades pedagógicas pode gerar diversos problemas na gestão escolar e no acompanhamento do aprendizado.  
Em regiões remotas do Brasil, a ausência de ferramentas digitais adequadas ainda representa um obstáculo para o bom andamento do processo educacional.  
Diante disso, o sistema proposto busca **otimizar o trabalho dos professores** e **melhorar a organização das informações acadêmicas**.

---

## 💻 Desafio
O sistema deve oferecer aos professores as seguintes funcionalidades:

- Realizar login (autenticação segura);  
- Consultar, cadastrar e remover suas turmas;  
- Registrar atividades vinculadas a uma turma específica;  
- Efetuar logout de forma segura.

---

## ⚙️ Requisitos de Ambiente

Para executar o sistema corretamente, é necessário preparar o ambiente conforme as especificações abaixo:

### 🗄️ Banco de Dados
- **SGBD:** MySQL  
- **Versão mínima recomendada:** 8.0  
- **Observação:** Crie um banco de dados próprio para o projeto e configure as credenciais no arquivo `.env`.

### 💾 Servidor / Sistema Operacional
- **Sistema Operacional:** Windows 10 ou 11  
- **Servidor de Aplicação:** Node.js  
- **Versão recomendada:** 18 ou superior  

### 🧠 Tecnologias Utilizadas
- **Back-end:** Node.js, Express, Prisma ORM  
- **Front-end:** HTML e CSS  
- **Banco de Dados:** MySQL  

---

## 🚀 Passo a Passo para Instalação e Execução

### 1️⃣ Clonar o Repositório

```bash
git clone https://github.com/Henricoramalho/escolaavaliacao.git
cd escolaavaliacao

 2. Instalar Dependências

```bash
npm install
ou
npm i
```

### 3. Configurar Banco de Dados
- Crie um banco de dados MySQL específico para o projeto.  
- Configure usuário e senha no arquivo `.env`:

```env
DATABASE_URL="mysql://root@localhost:3306/nome_do_banco"
```

### 4. Rodar Migrations do Prisma

```bash
npx prisma migrate dev --name init
```

### 5. Iniciar o Servidor

```bash
npm run dev
```

O servidor estará disponível em `http://localhost:3001`.

### 6. Testar o Sistema
- Acesse pelo navegador ou utilize o **Insomnia/Postman** para testar a API.  
- Funcionalidades para testar:
  - Cadastro, listagem, edição e exclusão de turmas;
  - Cadastro, listagem, edição e exclusão de atividades;
  - Login e logout do professor.


