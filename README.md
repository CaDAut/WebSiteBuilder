# 🚀 WebSite Builder

Construtor open source de websites com interface drag-and-drop. Crie sites profissionais sem código!

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![React](https://img.shields.io/badge/React-18.2-61dafb.svg)
![Node.js](https://img.shields.io/badge/Node.js-18+-green.svg)
![TypeScript](https://img.shields.io/badge/TypeScript-5.1-blue.svg)

## ✨ Funcionalidades

- 🎨 **Interface Drag & Drop** intuitiva
- 📱 **Design Responsivo** automático  
- 🧱 **Blocos Modulares** (Header, Hero, Forms, etc.)
- 💾 **Salvamento Automático** de projetos
- 🌐 **Versão Web** e **Desktop** (Electron)
- 📤 **Export HTML/CSS** limpo
- 🎭 **Sistema de Temas** personalizáveis
- 👥 **Colaboração** em tempo real

## 🛠️ Stack Tecnológico

- **Frontend**: React 18 + TypeScript + Tailwind CSS
- **Desktop**: Electron
- **Backend**: Node.js + Express  
- **Banco**: MySQL/MariaDB
- **Build**: Vite
- **Drag & Drop**: React DnD

## 🚀 Instalação Rápida

### Pré-requisitos
- Node.js 18+
- MySQL/MariaDB 8.0+
- Git

### Setup do Projeto

```bash
# Clone o repositório
git clone https://github.com/CaDAut/WebSiteBuilder.git
cd WebSiteBuilder

# Instale dependências
npm install

# Configure o banco de dados
cp .env.example .env
# Edite o .env com suas configurações de BD

# Execute migrações
npm run db:migrate

# Popule dados iniciais
npm run db:seed

# Inicie o desenvolvimento
npm run dev
```

### 🌐 Versão Web
```bash
npm run dev:web
# Acesse: http://localhost:5173
```

### 🖥️ Versão Desktop
```bash
npm run dev:electron
```

## 📁 Estrutura do Projeto

```
src/
├── web/              # Aplicação React web
│   ├── components/   # Componentes reutilizáveis
│   ├── blocks/       # Blocos drag-and-drop
│   ├── pages/        # Páginas da aplicação
│   ├── hooks/        # Custom hooks
│   ├── store/        # Estado global (Zustand)
│   └── utils/        # Utilitários
├── desktop/          # Configuração Electron
├── server/           # Backend API
│   ├── routes/       # Rotas da API
│   ├── models/       # Modelos do banco
│   └── middleware/   # Middlewares
├── shared/           # Código compartilhado
└── database/         # Scripts SQL
```

## 🎯 Blocos Disponíveis

| Bloco | Descrição | Status |
|-------|-----------|---------|
| 🏠 Header | Cabeçalhos e navegação | ✅ |
| 🦸 Hero | Seções de destaque | ✅ |
| 📝 Content | Texto, imagens, vídeos | ✅ |
| 📋 Forms | Formulários de contato | ✅ |
| 🖼️ Gallery | Galerias de imagens | ✅ |
| 🃏 Cards | Cards informativos | ✅ |
| 💬 Testimonials | Depoimentos | ✅ |
| 🦶 Footer | Rodapés | ✅ |

## 📱 Comandos Úteis

```bash
# Desenvolvimento
npm run dev                # Web + Backend
npm run dev:web           # Apenas web
npm run dev:server        # Apenas backend
npm run dev:electron      # Aplicação desktop

# Build e Deploy
npm run build             # Build completo
npm run build:web         # Build web
npm run build:electron    # Build desktop

# Qualidade de Código
npm run lint              # Verificar código
npm run lint:fix          # Corrigir automaticamente
npm run format            # Formatar código
npm test                  # Executar testes

# Banco de Dados
npm run db:migrate        # Rodar migrações
npm run db:seed          # Inserir dados iniciais
```

## 🌍 Variáveis de Ambiente

Crie um arquivo `.env` na raiz:

```env
# Banco de Dados
DB_HOST=localhost
DB_PORT=3306
DB_NAME=websitebuilder
DB_USER=root
DB_PASS=senha

# JWT
JWT_SECRET=seu_jwt_secret_super_seguro
JWT_EXPIRES_IN=7d

# Server
PORT=3001
NODE_ENV=development

# Upload
MAX_FILE_SIZE=10485760
UPLOAD_PATH=uploads/
```

## 🤝 Contribuindo

1. Faça um fork do projeto
2. Crie uma branch: `git checkout -b feature/nova-funcionalidade`
3. Commit suas mudanças: `git commit -m 'Adicionar nova funcionalidade'`
4. Push para a branch: `git push origin feature/nova-funcionalidade`
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja [LICENSE](LICENSE) para mais detalhes.

## 🆘 Suporte

- 📧 Email: [seu-email@exemplo.com]
- 💬 Issues: [GitHub Issues](https://github.com/CaDAut/WebSiteBuilder/issues)
- 📖 Docs: [Documentação](https://github.com/CaDAut/WebSiteBuilder/wiki)

---

⭐ Se este projeto te ajudou, considere dar uma estrela!
