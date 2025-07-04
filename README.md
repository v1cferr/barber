# Barbearia App (Nome Provisório)

Sistema completo para **gestão de clientes, agendamentos e operação de barbearias**, inspirado em plataformas como [AppBarber](https://appbarber.com.br). O objetivo é oferecer uma experiência eficiente tanto para os **clientes**, quanto para os **barbeiros e administradores**, centralizando todas as funções essenciais em um único dashboard moderno e intuitivo.

## ✂️ Funcionalidades (MVP)

### Cliente

- Cadastro/login com autenticação via Supabase
- Agendamento de horário com barbeiro disponível
- Visualização de agendamentos futuros e passados
- Edição e cancelamento de agendamentos

### Funcionário/Admin

- Painel (dashboard) com:
  - Lista de agendamentos do dia
  - Filtros por barbeiro/data
  - Gerenciamento de disponibilidade
- Cadastro e edição de horários de atendimento
- Visualização de clientes agendados

## 🧠 Tecnologias Utilizadas

| Stack                | Tecnologias                                                    |
| -------------------- | -------------------------------------------------------------- |
| **Frontend/Backend** | [Next.js](https://nextjs.org/) (App Router + API Handlers)     |
| **Deploy**           | [Vercel](https://vercel.com)                                   |
| **Banco de Dados**   | [Supabase](https://supabase.com) (PostgreSQL + Auth + Storage) |
| **Design/UI**        | Prototipado via [Google Stitch](https://stitch.withgoogle.com) |
| **Colaboração**      | Projeto desenvolvido por Victor (@v1cferr) e Rafael            |

## 🔧 Como Rodar o Projeto Localmente

```bash
# 1. Clone o repositório
git clone https://github.com/v1cferr/barber.git
cd barber

# 2. Instale as dependências
pnpm install

# 3. Crie o arquivo de variáveis de ambiente
cp .env.example .env.local
# Insira as credenciais do Supabase (URL + Anon Key)

# 4. Rode o projeto com Turbopack (recomendado)
pnpm run dev
```

## 📂 Estrutura Base (provisória)

```bash
src/
├── app/
│   ├── page.tsx             # Home
│   ├── login/               # Login e cadastro
│   ├── dashboard/           # Painel administrativo
│   └── api/                 # API Routes (Next.js Handlers)
├── components/              # Componentes reutilizáveis (UI)
├── lib/                     # Configurações e clientes Supabase
├── styles/                  # CSS/Tailwind config
```

## 🚀 Deploy

- Deploy contínuo via **Vercel**.
- Banco de dados e autenticação gerenciados via **Supabase**.
- O projeto é fullstack sem necessidade de back-end separado.

## 📌 Roadmap

- [ ] Finalizar protótipo no Google Stitch
- [ ] Conectar autenticação com Supabase
- [ ] CRUD de agendamentos (cliente e funcionário)
- [ ] Disponibilidade por horário e barbeiro
- [ ] Otimização para mobile (responsividade)
- [ ] Histórico de atendimentos

## 📝 Licença

Projeto acadêmico/experimental. Licenciamento será definido conforme evolução.

## 🤝 Contato

- Victor (@v1cferr) - [v1cferr.dev](https://v1cferr.dev)
- Rafael
