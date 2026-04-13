# SportTrack

> Plataforma web para gerenciamento e acompanhamento de treinos esportivos pessoais.

<p align="center">
  <img src="https://img.shields.io/badge/status-em%20desenvolvimento-yellow" />
  <img src="https://img.shields.io/badge/version-1.0-blue" />
  <img src="https://img.shields.io/badge/license-MIT-green" />
</p>

---

##  Sobre o Projeto

Atletas amadores frequentemente não possuem uma forma eficiente de registrar e acompanhar sua evolução nos treinos. Muitos utilizam métodos manuais, como cadernos ou planilhas, ou simplesmente não registram suas atividades.

O **SportTrack** surge como uma solução digital, permitindo o registro, acompanhamento e análise de treinos por meio de uma interface moderna e intuitiva.

---

## 🎯 Objetivo

Facilitar o acompanhamento de desempenho esportivo, oferecendo uma plataforma centralizada para registro, análise e evolução dos treinos.

---

## ⚙️ Funcionalidades

###  Principais Recursos
- Cadastro e login de usuários
- Registro de treinos (data, tipo, duração e observações)
- Histórico completo de atividades
- Dashboard com gráficos e estatísticas
- Edição e exclusão de treinos
- Metas semanais com acompanhamento de progresso

---

##  Tecnologias Utilizadas

| Tecnologia | Função |
|---|---|
| React | Interface do usuário |
| Node.js | Backend |
| Express | API REST |
| PostgreSQL | Banco de dados |
| Prisma ORM | ORM |
| JWT | Autenticação |
| Chart.js | Gráficos |

---

##  Arquitetura do Projeto

sporttrack/
│
├── backend/
│   ├── src/
│   ├── prisma/
│   └── package.json
│
├── frontend/
│   ├── src/
│   └── package.json
│
└── README.md

---

## Modelagem de Dados

Usuario           Treino              Meta
--------          --------            --------
id                id                  id
nome              titulo              usuario_id
email             tipo_esporte        treinos_semana
senha             duracao_min         progresso
criado_em         observacoes         ativa
                  usuario_id          
                  data_treino         

---

## Como Executar o Projeto
### 🔧 Pré-requisitos
- Node.js 18+
- PostgreSQL

---

###  Backend

cd backend  
npm install  
npx prisma migrate dev  
npm run dev  

---

###  Frontend

cd frontend  
npm install  
npm run dev  

---

### Variáveis de Ambiente

DATABASE_URL="postgresql://usuario:senha@localhost:5432/sporttrack"  
JWT_SECRET="sua_chave_secreta"  
PORT=3333  

---

## Indicadores do Dashboard

- Total de treinos no mês
- Tempo total treinado
- Esporte mais praticado
- Progresso das metas (%)
- Frequência semanal

---

##  Melhorias Futuras

- Aplicativo mobile
- Integração com smartwatches
- Sistema de ranking entre usuários
- Compartilhamento de resultados

---

## Autor

Vinicius Steuernagel  
Curso: 
Instituição:CATOLICA

---

## 📄 Licença

Este projeto está sob a licença MIT.
