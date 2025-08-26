# HelpDesk-IA (Web, Desktop, Mobile)

Plataforma de HelpDesk com assistente de IA, disponível para Web, Desktop (Electron) e Mobile (FlutterFlow). Backend em C# (.NET 8) com MySQL, com o intuito de suprir a demando dos chamados do cliente.

## Objetivo
- Centralizar chamados (tickets)
- Chat de atendimento com IA integrada (respostas sugeridas)
- Base de conhecimento pesquisável

## Tecnologias
- Backend: .NET 8 + MySQL
- Web: HTML/CSS/JS
- Desktop: Electron
- Mobile: FlutterFlow


### Backend
1. Configure variáveis em appsettings.json (MySQL + Provider de IA opcional)
2. dotnet restore
3. dotnet ef database update (ou rode scripts/schema.mysql.sql)
4. dotnet run (porta padrão: 5819)

### Web
1. Edite scripts/main.js e defina API_BASE_URL
2. Sirva via Live Server/python -m http.server

### Desktop (Electron)
1. npm install
2. npm start

### Mobile (FlutterFlow)
- Importe o api-spec-openapi.yaml ou configure endpoints conforme mobile/flutterflow/api-config.md

## IA
- Camada Services/AiService.cs com interface IAiProvider para plugar provedores (dummy por padrão).

## Contribuição
- Conventional Commits simplificado
- GitHub Flow (main estável, feature/*, PR + review)

## Licença
MIT
