# CardioIA Portal

Portal de diagnóstico cardiovascular desenvolvido em React + Vite para simulação de gerenciamento de pacientes e consultas cardiológicas.

## 🚀 Tecnologias

- React 18
- Vite
- React Router DOM
- Context API
- CSS Modules
- JSONPlaceholder (API mock)

## 📋 Funcionalidades

- ✅ Autenticação simulada com JWT fake
- ✅ Dashboard com métricas
- ✅ Listagem de pacientes
- ✅ Agendamento de consultas
- ✅ Proteção de rotas
- ✅ Filtros de busca
- ✅ Design responsivo

## 👨‍🎓 Integrantes do Grupo

- Amanda Vieira Pires (RM566330)
- Ana Gabriela Soares Santos (RM565235)
- Bianca Nascimento de Santa Cruz Oliveira (RM561390)
- Milena Pereira dos Santos Silva (RM565464)
- Nayana Mehta Miazaki (RM565045)

## 🔧 Instalação

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/nome-do-grupo-cardioia-portal.git
cd nome-do-grupo-cardioia-portal
Instale as dependências:

bash
npm install
npm install react-router-dom
Execute o projeto:

bash
npm run dev
Acesse http://localhost:5173

```

# 🔐 Credenciais de Teste

- **Email:** medico@cardioia.com
- **Senha:** 123456

---

# 📁 Estrutura do Projeto

```text
cardioia-portal/
├── src/
│   ├── contexts/
│   │   └── AuthContext.jsx
│   ├── components/
│   │   ├── Layout/
│   │   │   ├── Header.jsx
│   │   │   ├── Sidebar.jsx
│   │   │   └── ProtectedRoute.jsx
│   │   ├── Dashboard/
│   │   │   ├── StatsCard.jsx
│   │   │   └── RecentAppointments.jsx
│   │   └── Patients/
│   │       └── PatientCard.jsx
│   ├── services/
│   │   ├── api.js
│   │   └── mockData.js
│   ├── pages/
│   │   ├── Login.jsx
│   │   ├── Dashboard.jsx
│   │   ├── Patients.jsx
│   │   ├── Appointments.jsx
│   │   └── NewAppointment.jsx
│   ├── hooks/
│   │   └── useAppointments.js
│   ├── styles/
│   │   └── global.css
│   ├── App.jsx
│   └── main.jsx
├── index.html
├── package.json
├── vite.config.js
└── README.md

```

# 🎯 Requisitos Atendidos

## Autenticação simulada via Context API

- Implementada no arquivo `src/contexts/AuthContext.jsx`
- Utiliza JWT fake armazenado no `localStorage`
- Proteção de rotas com componente `ProtectedRoute`

## Listagem de pacientes com API fake

- Dados mockados em `src/services/mockData.js`
- Simulação de API em `src/services/api.js`
- Integração com JSONPlaceholder para dados complementares

## Formulário de agendamento com useState e useReducer

- Página `NewAppointment.jsx` com `useState` para controle do formulário
- Hook customizado `useAppointments` com `useReducer` para gerenciamento de estado global das consultas

## Dashboard com métricas

- Cards de estatísticas em `Dashboard.jsx`
- Contagem de pacientes e consultas agendadas
- Filtros por nível de risco

## Estilização com CSS Modules

- Todos os componentes utilizam CSS Modules
- Design responsivo para mobile e desktop
- Temas consistentes em toda a aplicação

---

# 🏥 Diagnósticos Suportados

O sistema trabalha com os seguintes diagnósticos cardiológicos e relacionados:

| ID  | Diagnóstico                |
| --- | -------------------------- |
| 1   | Infarto Agudo do Miocárdio |
| 2   | Pneumonia                  |
| 3   | Enxaqueca                  |
| 4   | Gastrite                   |
| 5   | Transtorno de Ansiedade    |
| 6   | Insuficiência Cardíaca     |

---

# 🎥 Vídeo de Demonstração

[Link para o vídeo no YouTube - Não Listado]

---

# 📝 Observações

- Este projeto foi desenvolvido como atividade acadêmica para a disciplina de Front-End
- Todos os dados são simulados e não há integração com back-end real
- O foco principal é a aplicação dos conceitos de React, Hooks e Context API

---

# 🔄 Hooks Utilizados

| Hook                            | Local                             | Finalidade                               |
| ------------------------------- | --------------------------------- | ---------------------------------------- |
| `useState`                      | Login, NewAppointment, Patients   | Gerenciar estado local dos formulários   |
| `useEffect`                     | Dashboard, Patients, Appointments | Carregar dados na montagem do componente |
| `useContext`                    | Header, ProtectedRoute, Sidebar   | Acessar estado de autenticação global    |
| `useReducer`                    | useAppointments                   | Gerenciar estado complexo das consultas  |
| `useNavigate`                   | Login, NewAppointment             | Navegação programática entre páginas     |
| `Custom Hook (useAppointments)` | -                                 | Lógica reutilizável para consultas       |

---

# 🎨 Paleta de Cores

| Cor            | Código    | Uso                        |
| -------------- | --------- | -------------------------- |
| Roxo Principal | `#667eea` | Header, botões, gradientes |
| Roxo Escuro    | `#764ba2` | Gradientes, hover states   |
| Azul Escuro    | `#2c3e50` | Sidebar, textos principais |
| Azul Claro     | `#3498db` | Links ativos, detalhes     |
| Vermelho       | `#e74c3c` | Casos críticos, alertas    |
| Laranja        | `#f39c12` | Alto risco, avisos         |
| Verde          | `#2ecc71` | Baixo risco, sucesso       |
| Cinza Claro    | `#ecf0f1` | Bordas, backgrounds        |

---

# 📱 Responsividade

O layout se adapta aos seguintes breakpoints:

| Dispositivo | Largura        | Comportamento                   |
| ----------- | -------------- | ------------------------------- |
| Mobile      | < 768px        | Menu colapsado, cards em coluna |
| Tablet      | 768px - 1024px | Menu lateral reduzido           |
| Desktop     | > 1024px       | Layout completo                 |

---

# 🚦 Status do Projeto

✅ **Concluído**

---

# 📄 Licença

Este projeto é parte de uma atividade acadêmica e não possui licença comercial.

```

```
