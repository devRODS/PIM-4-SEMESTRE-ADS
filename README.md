# Help Desk-IA (Sistema de Help Desk em Web, Desktop, Mobile)

Plataforma de HelpDesk com assistente de IA, disponível para Web, Desktop (Electron) e Mobile (FlutterFlow). Backend em C# (.NET 8) com MySQL, com o intuito de suprir a demando dos chamados do cliente.

> Status do Projeto: Em progresso

 
## Desafio <a id="desafio"></a>

O desafio consiste em desenvolver uma aplicação de helpdesk com inteligência artificial integrada, disponível para plataformas mobile, web e desktop. A aplicação deve permitir que os usuários abram chamados ou solicitações de suporte, e que a IA responda automaticamente a esses chamados com base em um banco de dados de conhecimento e aprendizado contínuo. Paralelamente, a aplicação deve possibilitar que atendentes humanos possam intervir e complementar as respostas da IA, garantindo a melhor qualidade no atendimento

## Solução <a id="solucao"></a>

Help Desk, será uma solução que permitirá aos usuários abrir chamados de suporte em múltiplas plataformas (mobile, web e desktop) e receber respostas automáticas de modelos de IA integrados. Os usuários poderão avaliar cada resposta recebida segundo critérios objetivos, além de contar com a opção de intervenção humana para complementar o atendimento. Ao final, o sistema possibilitará a comparação entre a resposta da IA e a intervenção humana, permitindo que o usuário escolha qual foi a melhor solução e justifique sua decisão.

Esse processo garantirá um aprendizado contínuo por reforço, alimentando os modelos de IA com dados reais de avaliação e interação, promovendo assim o aprimoramento constante da qualidade do suporte prestado pela plataforma. Todos os dados de chamados, avaliações e justificativas serão armazenados para análise e futuros treinamentos dos modelos de inteligência artificial.




## Tecnologias
- Backend: .NET 8 + MySQL
- Web: HTML/CSS/JS
- Desktop: Electron
- Mobile: FlutterFlow


### Backend
1. Configure variáveis em appsettings.json (MySQL + Provider de IA opcional)
2. dotnet restore


### Web
1. Edit index.html
2. Edit /styles.css

### Desktop (Electron)
1. npm install
2. npm start

### Mobile (FlutterFlow)
- Importe o api-spec-openapi.yaml ou configure endpoints conforme mobile/flutterflow/api-config.md

## IA
- Camada Services/AiService.cs com interface IAiProvider para plugar provedores (dummy por padrão).


## 📅 Cronograma de Sprints <a id="sprint"></a>

| Sprint          |    Período    | Documentação                                     |
| --------------- | :-----------: | ------------------------------------------------ |
| 🔖 **SPRINT 1** | 20/08 - 24/08 | Inicio do Front End Web| ✅
| 🔖 **SPRINT 2** | 25/08 - 27/08 | Inicio do Mobile em FlutterFlow | ✅
| 🔖 **SPRINT 3** | 03/09 - 08/09 | ....


## 📖 Manual de Instalação <a id="manual"></a>

### 🛠 Pré-requisitos

- Git ([Download](https://git-scm.com/downloads)
- VsCode ([Download](https://code.visualstudio.com/download))
- FlutterFlow ([Download](https://www.flutterflow.io/downloads))



