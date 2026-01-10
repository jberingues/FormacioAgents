# Introducció a Sistemes Multi-Agent amb CrewAI
## JCM Technologies - Departament de R+D

![CrewAI](https://img.shields.io/badge/CrewAI-0.80+-blue)
![Python](https://img.shields.io/badge/Python-3.10+-green)
![Google Gemini](https://img.shields.io/badge/Gemini-2.0-orange)

Formació pràctica per crear sistemes d'agents d'IA que col·laboren per resoldre problemes complexos.

**🎯 Durada:** 4 hores  
**👥 Modalitat:** Presencial amb o sense pràctiques / Autodidacta  
**💻 Requisits:** Ordinador portàtil + ganes d'aprendre

---

## 🚀 Inici Ràpid

### ⚠️ ABANS DE LA FORMACIÓ (obligatori si es volen fer pràctiques)

**Temps necessari:** 30-45 minuts

Segueix aquests 5 passos per estar preparat:

#### 1️⃣ Instal·lar Cursor
- Descarrega: https://cursor.com
- Instal·la per al teu sistema operatiu
- Obre'l una vegada per verificar

*(Nota: També pot funcionar amb Visual Studio Code, però els exemples seran amb Cursor)*

#### 2️⃣ Descarregar el repositori

**Opció A:** Descarregar ZIP
- Ves a aquest repositori → Botó verd "Code" → "Download ZIP"
- Descomprimeix-lo al teu ordinador

**Opció B:** Clonar amb Git
```bash
git clone https://github.com/jberingues/FormacioAgents
```
*(Nota: Cal tenir Git instal·lat: https://git-scm.com/downloads)*

#### 3️⃣ Obrir el projecte
- Obre Cursor
- File → Open Folder
- Selecciona la carpeta del repositori

#### 4️⃣ Seguir el Setup
- Obre el fitxer: `00_setup_crewai.ipynb`
- Segueix **TOTES** les instruccions
- Això instal·larà Python, dependències, i API Keys

#### 5️⃣ Verificar
- Executa la cel·la de verificació al final del Setup
- Has de veure: **🎉 TOT CORRECTE!**

### ❌ Si tens problemes
- Revisa la secció "Troubleshooting" del Setup
- Contacta amb Jordi Beringues


---

## 📚 Contingut de la Formació

### Part 0: Setup (00_setup_crewai.ipynb)
**⏱️ Fer abans de la formació**

- Configuració de l'entorn de desenvolupament
- Instal·lació d'UV i dependències
- Configuració d'API Keys (Gemini i Gmail)
- Verificació de l'entorn

### Part 1: Conceptes Fonamentals (1 hora)
**📓 Notebook:** `01_conceptes_CrewAI.ipynb`

**Continguts:**
- Recordatori ràpid: Què són els LLMs?
- Costos i models: Google Gemini
- Frameworks d'agents: De baix a alt nivell
- Workflows vs Agents: La diferència clau
- Mans a l'obra: El teu primer Crew
- Cas pràctic: Crew analitzador de BOM

**🎯 Aprendràs:**
- La diferència fonamental entre workflows i agents
- L'arquitectura de CrewAI i les capes de frameworks
- Com crear el teu primer agent amb Google Gemini
- Aplicar-ho a un cas real: analitzar un BOM (Bill of Materials)

### Part 2: Tools i Function Calling (1 hora)
**📓 Notebook:** `02_tools_CrewAI.ipynb`

**Continguts:**
- Què són les Tools?
- Primera Tool: Llegir fitxers Excel
- Segona Tool: Consultar API de preus
- Traces en profunditat (debugging)
- Múltiples agents col·laborant

**🎯 Aprendràs:**
- Què són les tools i per què són essencials per als agents
- Com crear tools personalitzades amb `@tool`
- Com els agents decideixen quina tool usar (function calling)
- Com interpretar traces per debugar agents
- Com crear sistemes multi-agent col·laboratius

### Part 3: Cas Pràctic Complet (2 hores)
**📓 Notebook:** `03_cas_practic_CrewAI.ipynb`

**Continguts:**
- Visió general del sistema
- Agent 1: BOM Analyzer
- Agent 2: RFQ Generator
- Enviar emails REALS amb Gmail API
- Dinàmica amb 3 voluntaris (participació interactiva)
- Agent 3: Email Parser
- Agents 4 i 5: Comparació de preus i generació d'informes
- Integració completa del sistema

**🎯 Aprendràs:**
- Com construir un sistema complet multi-agent amb 5 agents col·laborant
- Integració real amb Gmail API per enviar i rebre emails
- Parsing intel·ligent d'emails no estructurats
- Comparativa multi-proveïdor automatitzada
- Generació d'informes executius en Markdown

---

## 🎯 Què Aconseguiràs

Al final d'aquesta formació, seràs capaç de:

✅ Crear i configurar agents d'IA amb CrewAI  
✅ Dissenyar workflows multi-agent  
✅ Desenvolupar tools personalitzades per als teus agents  
✅ Integrar APIs externes (Gmail, Google Sheets, etc.)  
✅ Debugar i optimitzar sistemes d'agents  
✅ Aplicar agents d'IA a problemes reals de JCM  

---

## 💻 Requisits Tècnics

### Sistema Operatiu
- ✅ Windows 10/11
- ✅ macOS 12+
- ✅ Linux (Ubuntu 20.04+)

### Software
- **Python:** 3.10 o superior (s'instal·la al Setup si no el tens)
- **Cursor:** Editor de codi (https://cursor.com)
- **Git:** Opcional, per clonar el repositori


### APIs
- **Google Gemini API Key** (s'obté al Setup) - Gratuïta
- **Gmail API** (opcional, per la Part 3) - Gratuïta
- **OpenAI API Key** (per executar la Part 3) - De pagament

---

## 📁 Estructura del Projecte

```
formacioagents/
├── README.md                                    # Aquest fitxer
├── pyproject.toml                               # Dependències del projecte
├── uv.lock                                      # Versions exactes
├── .env                                         # API Keys (NO pujar a Git!)
├── .gitignore                                   # Fitxers a ignorar
├── 00_setup_crewai.ipynb                        # Setup inicial ⚠️ FER PRIMER
│
├── notebooks/
│   ├── 01_conceptes_fonamentals_crewai.ipynb   # Part 1 (1h)
│   ├── 02_tools_function_calling.ipynb         # Part 2 (1h)
│   └── 03_cas_practic_crewai.ipynb             # Part 3 (2h)
│
├── data/
│   └── Bill_of_Materials-TESTBOM.xlsx          # BOM per test
│
└── .venv/                                       # Entorn virtual (creat per UV)
```

---

## 🆘 Problemes Comuns

### "No trobo l'API Key de Gemini"
**Solució:** Ves a https://aistudio.google.com/app/apikey i crea'n una (gratuïta)

### "UV no funciona"
**Solució:** El Setup l'instal·la automàticament. Si falla, segueix les instruccions manuals de la Secció 2 del Setup.

### "El kernel no es troba a Cursor"
**Solució:** 
1. Ctrl/Cmd + Shift + P
2. Escriu "Select Kernel"
3. Selecciona `.venv/bin/python` (o `.venv\Scripts\python.exe` a Windows)

### "Import error amb CrewAI"
**Solució:** 
```bash
cd formacioagents
uv sync
```

### "403 Forbidden amb Gmail API"
**Solució:** Has d'afegir el teu email com a "test user" a la consola de Google Cloud (explicat al Setup)

### Altres problemes
Contacta amb el formador: jordi@jcmtechnologies.com

---

## 🔐 Seguretat i Bones Pràctiques

### ⚠️ MOLT IMPORTANT - NO pugis mai a Git:

❌ `.env` (conté API Keys)  
❌ `credentials.json` (OAuth Gmail)  
❌ `token.json` (OAuth Gmail)  

✅ Aquests fitxers ja estan al `.gitignore`

### Si comparteixes codi:
1. Elimina sempre les API Keys abans
2. Revisa que no hi hagi informació sensible
3. Usa variables d'entorn per a secrets

---

## 📖 Material Addicional (després del curs)

### Documentació oficial:
- **CrewAI:** https://docs.crewai.com/
- **Google Gemini:** https://ai.google.dev/gemini-api/docs
- **Gmail API:** https://developers.google.com/gmail/api

### Cursos recomanats:
- **DeepLearning.AI - Multi AI Agent Systems:** https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/
- **CrewAI GitHub:** https://github.com/joaomdmoura/crewAI

### Eines útils:
- **Google AI Studio:** https://aistudio.google.com/ (per provar prompts)
- **LangSmith:** https://smith.langchain.com/ (per debugging avançat)

---

## 📅 Informació de la Sessió

**Data:** [DATA DE LA FORMACIÓ]  
**Horari:** [HORA INICI] - [HORA FI]  
**Lloc:** [SALA/EDIFICI]  
**Durada:** 4 hores (amb breaks de 10 min cada hora)

### Què portar:
✅ Ordinador portàtil (bateria carregada + carregador)  
✅ Setup completat (00_setup_crewai.ipynb)  
✅ Ganes d'aprendre! 🚀  

---

## 👥 Sobre la Formació

**Formador:** Jordi Beringues  
**Rol:** Director R+D  
**Empresa:** JCM Technologies, SAU  
**Contacte:** jordi@jcmtechnologies.com

Aquesta formació està dissenyada per introduir els conceptes fonamentals dels sistemes multi-agent d'IA mitjançant exemples pràctics i aplicacions reals de JCM Technologies.

---

## 📜 Llicència

Aquest material està creat per JCM Technologies, SAU i està destinat a introduir al món dels agents d'IA a tothom qui tingui interès en el tema.

---

## ✅ Checklist Pre-Formació

Abans de venir a la formació, assegura't que:

- [ ] Tens Cursor instal·lat
- [ ] Has descarregat el repositori
- [ ] Has obert el projecte a Cursor
- [ ] Has completat `00_setup_crewai.ipynb`
- [ ] La verificació final passa correctament (🎉 TOT CORRECTE!)
- [ ] Tens l'API Key de Gemini guardada
- [ ] Portes el portàtil + carregador

**Si tot està ✅ → Estàs preparat!**

---

*Última actualització: Gener 2026*
