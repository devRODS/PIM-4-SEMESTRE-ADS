# Estrutura do Projeto HelpDesk

```
HelpDesk/
├── 📁  Codigo/
│   ├── 📂  .env.example
│   ├── 📂 .gitignore
│   ├── 📂 TicketSystem.API/
│   │   ├── 📂 TicketSystem.API.sln
│   │   ├── 📂 TicketSystem.API.Tests/
│   │   │   ├── Controllers/ (Testes para AuthController, TicketsController, etc.)
│   │   │   ├──  CustomWebApplicationFactory.cs
│   │   │   ├──  DomainTicketTests.cs
│   │   │   ├──  HealthEndpointTests.cs
│   │   │   └──  TicketSystem.API.Tests.csproj
│   │   └── 📂 TicketSystem.API/
│   │       ├── 📂 Configuration/
│   │       │   └── AutoMapperProfile.cs
│   │       ├── 📂 Controllers/
│   │       │   ├── AiController.cs
│   │       │   ├── AuthController.cs
│   │       │   ├── DepartmentsController.cs
│   │       │   ├── HealthController.cs
│   │       │   ├── TicketsController.cs
│   │       │   └── UsersController.cs
│   │       ├── 📂 Data/
│   │       │   ├── ApplicationDbContext.cs
│   │       │   └── TicketSystemContext.cs
│   │       ├── 📂 Models/
│   │       │   ├── DTOs/ (AuthDTOS.cs, TicketDtos.cs, UserDtos.cs, etc.)
│   │       │   ├── Entities/ (Ticket.cs, User.cs, Department.cs, etc.)
│   │       │   └── Enums/ (TicketStatus.cs, UserType.cs, etc.)
│   │       ├── 📂 Properties/
│   │       │   └── launchSettings.json
│   │       ├── 📂 Services/
│   │       │   ├── Interfaces/ (IAiService.cs, IAuthService.cs)
│   │       │   ├── AiService.cs
│   │       │   └── AuthService.cs
│   │       ├── 📂 frontend/ (HTML/JS simples, talvez para testes)
│   │       │   ├── index.html
│   │       │   └── README.md
│   │       ├── 📂 Program.cs
│   │       ├── TicketSystem.API.csproj
│   │       ├── TicketSystem.API.http
│   │       ├── appsettings.Development.json
│   │       ├── appsettings.example.json
│   │       ├── appsettings.json
│   │       ├── banco.sql
│   │       └── seed-data.sql
│   ├── 📂 android/
│   │   ├── app/
│   │   │   ├── build.gradle
│   │   │   └── src/
│   │   │       ├── main/
│   │   │       │   ├── AndroidManifest.xml
│   │   │       │   ├── java/com/suaempresa/helpdesk/MainActivity.java
│   │   │       │   └── res/ (Contém ícones, layouts, estilos e configurações XML)
│   │   │       └── ... (outros diretórios de build e teste)
│   │   ├── build.gradle
│   │   ├── gradlew
│   │   ├── gradlew.bat
│   │   └── settings.gradle
│   ├── 📂 electron/
│   │   ├── main.js
│   │   └── preload.js
│   ├── 📂 public/
│   │   ├── favicon.ico
│   │   ├── manifest.webmanifest
│   │   ├── placeholder.svg
│   │   └── robots.txt
│   ├── 📂 src/
│   │   ├── 📂 assets/
│   │   │   └── helpdesk-hero.jpg
│   │   ├── 📂 components/
│   │   │   ├── layout/ (AppSidebar.tsx, Header.tsx, Layout.tsx)
│   │   │   └── ui/ (Muitos componentes UI: button.tsx, card.tsx, input.tsx, etc.)
│   │   ├── 📂 hooks/
│   │   │   ├── use-auth-hook.ts
│   │   │   ├── use-auth.tsx
│   │   │   ├── use-local-storage.ts
│   │   │   └── use-tickets.ts
│   │   ├── 📂 lib/
│   │   │   ├── ai.ts
│   │   │   ├── api.ts
│   │   │   ├── departments.ts
│   │   │   ├── tickets.ts
│   │   │   ├── users.ts
│   │   │   └── utils.ts
│   │   ├── 📂 pages/
│   │   │   ├── Dashboard.tsx
│   │   │   ├── EditarTicket.tsx
│   │   │   ├── Login.tsx
│   │   │   ├── NovoTicket.tsx
│   │   │   ├── Perfil.tsx
│   │   │   ├── Relatorios.tsx
│   │   │   ├── TodosChamados.tsx
│   │   │   ├── Usuarios.tsx
│   │   │   ├── VisualizarTicket.tsx
│   │   │   └── ... (outras páginas como FAQ.tsx, NotFound.tsx, etc.)
│   │   ├── 📂 test/
│   │   │   └── setup.ts
│   │   ├── App.css
│   │   ├── App.tsx
│   │   ├── index.css
│   │   ├── main.tsx
│   │   ├── sw.ts
│   │   └── vite-env.d.ts
│   ├── 📂 tests/
│   │   └── e2e/
│   │       ├── login.spec.ts
│   │       └── ticket-persistence.spec.ts
│   ├── bun.lockb
│   ├── capacitor.config.ts
│   ├── components.json
│   ├── eslint.config.js
│   ├── index.html
│   ├── package.json
│   ├── package-lock.json
│   ├── playwright.config.ts
│   ├── pnpm-lock.yaml
│   ├── postcss.config.js
│   ├── tailwind.config.ts
│   ├── tsconfig.app.json
│   ├── tsconfig.json
│   ├── tsconfig.node.json
│   └── vite.config.ts
├── 📂 Documentação/
│   ├── DoR e DoD/
│   │   ├── DoR.md
│   │   ├── Manual de Aplicação.md
│   │   └── Manual do Usuario.md
│   ├── Backlog.md
│   ├── Diagramas PIM.asta
│   ├── Equipe.md
│   ├── Execução e Testes do Projeto.md
│   ├── Sprints.md
│   └──gantt.md
└── README.md
