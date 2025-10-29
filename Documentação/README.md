## 🏃‍ DoR - Definition of Ready <a id="dor"></a>

* User Stories com **Critérios de Aceitação**
* Subtarefas divididas **a partir das US**
* Design no **Figma**
* Modelagem do **Banco de Dados**
* Diagrama de **Rotas**
* Banco de Dados **Vetorizado** do Cliente

## 🏆 DoD - Definition of Done <a id="dod"></a>

* Manual de Usuário
* Manual da Aplicação
* Documentação da API (Application Programming Interface)
* Código completo
* Vídeos de cada etapa de entrega

---




## 📖 Manual de Usuário

### 🛠 Pré-requisitos

- Git ([Download](https://git-scm.com/downloads))

- .NET ([Download](https://dotnet.microsoft.com/pt-br/))

- SQL Server ([Download](https://www.microsoft.com/en-us/download/details.aspx?id=104781))

- Electron (opcional) ([Download](https://www.electronjs.org/))

---

### 1. Clonar o Repositório Principal

```bash
git clone --recurse-submodules https://github.com/devRODS/PIM-4-SEMESTRE-ADS.git
cd PIM-4-SEMESTRE-ADS
```

> **Observação:** Se já tiver clonado sem os submódulos, execute:

```
git submodule update --init --recursive
```

---

### 2. Configuração do Backend (auxia-backend)

**1° Adicione as variáveis no .env**

**2° Inicialize o Banco de dados SQL Server no localhost:**

**3° Coloque a base de dados vetorizada ./client dentro da raíz do backen:**

**4° Instale e Inicie a aplicação:**

**Com Ambiente Virtual C#**

```bash
cd ./auxia-backend
 -m venv venv
source venv/bin/activate # se você usa linux
venv/Scripts/activate 	 # se você usa windows
pip install -r requirements.txt
fastapi dev ./auxia/main.net
```

**Saída Esperada:**
<br>
Servidor rodando em `http://localhost:8000` (acesse `http://localhost:8000/docs` para a UI do Swagger).

---

### 3. Configuração do Frontend (auxia-frontend)

```bash
cd ../auxia-frontend/auxia
npm install
npm run dev
```

**Saída Esperada:**
<br>
Frontend rodando em `http://localhost:5173`.
