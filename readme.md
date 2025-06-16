# Projeto BRNX

![Node.js](https://img.shields.io/badge/NodeJS-20232A?style=for-the-badge&logo=node.js&logoColor=339933)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

Sistema de gerenciamento de demandas de provedores da BRNX

## 📚 Visão Geral

Esse sistema é uma plataforma completa que integra:

- ✨ **Criação inteligente** de relatorios  
- 📊 **Gerenciamento** de demandas  


## 🏗️ Estrutura do Projeto

| Componente       | Tecnologias-Chave                  | Repositório                                                |
|------------------|------------------------------------|------------------------------------------------------------|
| **Backend**      | Node.js, Express, PostgreSQL       | [brnx-back](https://github.com/LazimR/brnx-back)     |
| **Frontend**     | React, Redux                       | [brnx-front](https://github.com/LazimR/brnx-front) |
| **Infra**        | Docker, Docker Compose             |                                                            |

## 🛠️ Tecnologias Principais

### Backend
- **Express**
- **PostgreSQL** (Prisma ORM)
- **Geração de PDFs**: Pdfkit
- **Autenticação**: Bcrypt

### Frontend (Em Desenvolvimento)
- **React 19** + TypeScript
- **Gerenciamento de Estado**: Redux Toolkit

## 🚀 Funcionalidades
- Geração automática de relatorios
- Armazenamento de Provedores
- Gerenciamento de Demandas


## 🐳 Executando com Docker

1. Clone o repositório principal:
```bash
git clone https://github.com/LazimR/brnx.git
cd brnx
git clone https://github.com/LazimR/brnx-back
git clone https://github.com/LazimR/brnx-front
```

2. Inicie os containers:
- Crie um docker-compose a partir do docker-compose.example

```bash
docker-compose up -d --build

```

3. Crie um usuario para acessar o sistema:
```bash
curl -X POST http://localhost:3000/users \
-H "Content-Type: application/json" \
-d '{"name":"admin","password":"admin123"}'
```

4. Acesse:
BD: http://localhost:5432/

Backend: http://localhost:3000/

Frontend: http://localhost:80
