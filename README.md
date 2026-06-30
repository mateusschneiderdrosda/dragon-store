# 🐉 Dragon Store

Uma plataforma profissional para venda de scripts para Roblox com autenticação completa, pagamentos via PIX, painel administrativo, bot Discord e sistema de licenças.

## 🎯 Características

- ✅ **Autenticação Completa**: JWT, OAuth2 (Discord, Google), Refresh Token
- ✅ **Pagamentos**: Integração Asaas, PIX, Webhooks, Assinaturas
- ✅ **Painel Admin**: Dashboard com estatísticas, gerenciamento de usuários e produtos
- ✅ **Painel Cliente**: Perfil, compras, downloads, licenças
- ✅ **Bot Discord**: Comandos interativos e notificações
- ✅ **Sistema de Licenças**: Geração, validação e renovação automática
- ✅ **Cupons**: Desconto percentual, valor fixo, expiração
- ✅ **Afiliados**: Código único, comissão, dashboard
- ✅ **Suporte**: Sistema de tickets com status
- ✅ **Segurança**: bcrypt, JWT, HTTPS, Rate Limit, CSRF, XSS Protection
- ✅ **Documentação**: README, API docs, Deploy guide

## 🛠️ Tecnologias

### Backend
- Python 3.13
- FastAPI
- SQLAlchemy
- Alembic
- PostgreSQL
- Redis
- Pydantic
- Uvicorn

### Frontend
- React 18
- Vite
- TypeScript
- TailwindCSS
- React Router
- Axios
- Zustand

### Bot
- discord.py

### Infraestrutura
- Docker
- Docker Compose
- Nginx

## 📁 Estrutura do Projeto

Ver [CONTRIBUTING.md](CONTRIBUTING.md) para estrutura detalhada.

## 🚀 Quick Start

### Com Docker Compose (Recomendado)

```bash
# Clone o repositório
git clone https://github.com/mateusschneiderdrosda/dragon-store.git
cd dragon-store

# Configure as variáveis de ambiente
cp backend/.env.example backend/.env
cp frontend/.env.example frontend/.env
cp discord-bot/.env.example discord-bot/.env

# Inicie os serviços
docker-compose up -d

# Crie o banco de dados
docker-compose exec backend alembic upgrade head

# Acesse
# Backend: http://localhost:8000
# Frontend: http://localhost:5173
# API Docs: http://localhost:8000/docs
```

## 📖 Documentação

- **[API.md](docs/API.md)** - Documentação completa da API REST
- **[INSTALL.md](docs/INSTALL.md)** - Guia de instalação local
- **[DEPLOY.md](docs/DEPLOY.md)** - Guia de deployment
- **[SECURITY.md](docs/SECURITY.md)** - Boas práticas de segurança
- **[DATABASE.md](docs/DATABASE.md)** - Schema do banco de dados

## 🔐 Segurança

- Senhas hasheadas com bcrypt
- JWT com refresh token
- HTTPS obrigatório em produção
- Rate limiting em todos os endpoints
- CSRF protection
- XSS protection
- SQL injection prevention
- Logs de auditoria
- Backup automático diário

## 🧪 Testes

```bash
# Backend
cd backend
pytest

# Frontend
cd frontend
npm test

# Com coverage
pytest --cov=app tests/
```

## 📦 Variáveis de Ambiente

Veja os arquivos `.env.example` em cada diretório para configurações necessárias.

## 🤝 Contribuição

Leia [CONTRIBUTING.md](CONTRIBUTING.md) para diretrizes de contribuição.

## 📄 Licença

Este projeto está licenciado sob a MIT License - veja [LICENSE](LICENSE).

## 👨‍💻 Autor

Mateus Schneider Drosda

---

**Desenvolvido com ❤️ para a comunidade Roblox**