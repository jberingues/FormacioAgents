# Introducció a Sistemes Multi-Agent amb CrewAI
## JCM Technologies - Departament de R+D

![CrewAI](https://img.shields.io/badge/CrewAI-0.80+-blue)
![Python](https://img.shields.io/badge/Python-3.10+-green)
![Google Gemini](https://img.shields.io/badge/Gemini-2.0-orange)

Aquest és un repositori per a la formació interna d'agents d'IA utilitzant CrewAI.

---

## 📚 Contingut de la Formació

### **Part 0: Setup (00_setup_crewai.ipynb)** -- Executar abans de la formació
- Configuració de l'entorn de desenvolupament
- Instal·lació d'UV i dependències
- Configuració d'API Keys (Gemini i Gmail)
- Verificació de l'entorn

### **Part 1: Conceptes Fonamentals (01_conceptes_fonamentals_crewai.ipynb)**
- Diferència entre Workflows i Agents
- Arquitectura de CrewAI
- Creació del primer agent
- Anàlisi de BOM amb agents

### **Part 2: Tools i Function Calling (02_tools_function_calling.ipynb)**
- Què són les tools i per què són necessàries
- Creació de tools personalitzades
- Lectura de fitxers Excel
- APIs mock per a preus
- Debugging de traces d'execució
- Col·laboració multi-agent

### **Part 3: Cas Pràctic Complet (03_cas_practic.ipynb)**
- Sistema de cotitzacions per email **REAL**
- 5 agents col·laborant
- Integració Gmail API
- Parsing intel·ligent d'emails no estructurats
- Comparativa multi-proveïdor
- Generació d'informes executius

**Durada total:** ~4 hores (pràctica intensiva)

---

## 📋 PREPARACIÓ (30-45 minuts aprox.)

### ✅ PAS 1: Instal·lar Cursor (editor de codi)

- Aneu a: **https://cursor.com**
- Descarregueu la versió per al vostre sistema operatiu
- Instal·leu-lo
- Obriu-lo una vegada per verificar que funciona

**⏰ Temps:** 5 minuts

---

### ✅ PAS 2: Descarregar el repositori de la formació

Teniu **2 opcions** (escolliu la que us sigui més fàcil):

#### 📦 OPCIÓ A: Descarregar ZIP (recomanat, més fàcil)

- Aneu a: **[URL_DEL_REPOSITORI_GITHUB]**
- Cliqueu el botó verd **"Code"** → **"Download ZIP"**
- Descomprimiu-lo al vostre ordinador
- Recordeu on l'heu desat!

**⏰ Temps:** 2 minuts

#### 🔧 OPCIÓ B: Clonar amb Git (si sou usuaris avançats)

- Instal·leu Git: **https://git-scm.com/downloads**
- Obriu un terminal/command prompt
- Executeu: `git clone [URL_DEL_REPOSITORI]`

**⏰ Temps:** 5-10 minuts (si cal instal·lar Git)

---

### ✅ PAS 3: Obrir el projecte amb Cursor

- Obriu Cursor
- **File** → **Open Folder**
- Seleccioneu la carpeta del repositori (on heu descomprimit el ZIP)

---

### ✅ PAS 4: Seguir les instruccions del fitxer Setup

- A Cursor, obriu el fitxer: **`00_setup.ipynb`**
- Seguiu **TOTES** les instruccions pas a pas

Aquest fitxer us guiarà per:

- Instal·lar Python i les dependències necessàries
- Crear la vostra API Key de Google Gemini (gratuïta)
- Configurar les variables d'entorn
- (Opcional) Configurar Gmail API

**⏰ Temps:** 20-30 minuts

---

### ✅ PAS 5: Verificar que tot funciona

Al final del fitxer `00_setup.ipynb` hi ha una secció de verificació.

Executeu-la i assegureu-vos que veieu: **🎉 TOT CORRECTE!**

---

## ⚠️ IMPORTANT

- Feu **TOTS** els passos **ABANS** de la formació
- No tindrem temps per fer la instal·lació el dia de la sessió
- Si teniu problemes:
  - Reviseu la secció **"Troubleshooting"** del `00_setup.ipynb`
  - Escriviu-me: **[EL_TEU_EMAIL]**
  - Arribeu **15 minuts abans** i us ajudo presencialment


---


## 📁 Estructura del Projecte
```
formacioagents/
├── README.md                                    # Aquest fitxer
├── pyproject.toml                               # Dependències del projecte
├── uv.lock                                      # Versions exactes (generat per UV)
├── .env                                         # API Keys (NO pujar a Git!)
├── .gitignore                                   # Fitxers a ignorar
│
├── notebooks/
│   ├── 00_setup_crewai.ipynb                   # Setup inicial
│   ├── 01_conceptes_fonamentals_crewai.ipynb   # Part 1
│   ├── 02_tools_function_calling.ipynb         # Part 2
│   └── 03_cas_practic.ipynb                    # Part 3
│
├── data/
│   └── Bill_of_Materials-TESTBOM.xlsx          # BOM real de JCM
│
├── formacioagents/                              # Paquet Python del projecte
│   └── __init__.py
│
└── .venv/                                       # Entorn virtual (creat per UV)
```

---

## 🎯 Objectius d'Aprenentatge

Al final d'aquesta formació, seràs capaç de:

✅ Crear i configurar agents d'IA amb CrewAI  
✅ Dissenyar workflows multi-agent  
✅ Desenvolupar tools personalitzades per als teus agents  
✅ Integrar APIs externes (Gmail, Google Sheets, etc.)  
✅ Debugar i optimitzar sistemes d'agents  
✅ Aplicar agents d'IA a problemes reals de JCM  

---

## 📖 Material Addicional

### **Documentació oficial:**
- **CrewAI:** https://docs.crewai.com/
- **Google Gemini:** https://ai.google.dev/gemini-api/docs
- **Gmail API:** https://developers.google.com/gmail/api

### **Recursos recomanats:**
- **DeepLearning.AI - Multi AI Agent Systems:** https://www.deeplearning.ai/short-courses/multi-ai-agent-systems-with-crewai/
- **CrewAI GitHub:** https://github.com/joaomdmoura/crewAI
- **Google AI Studio:** https://aistudio.google.com/

---

## 🆘 Suport i Ajuda

### **Durant la formació:**
- Pregunta al formador (Jordi)
- Consulta els notebooks (tenen explicacions detallades)

### **Abans de la formació:**
- Si tens problemes amb el Setup, contacta amb el Jordi
- Revisa aquest README i el notebook `00_setup_crewai.ipynb`

### **Problemes comuns:**

**"No trobo l'API Key de Gemini"**
→ Ves a https://aistudio.google.com/app/apikey i crea'n una

**"UV no funciona"**
→ El Setup l'instal·la automàticament. Si falla, executa manualment les instruccions de la Secció 2

**"El kernel no es troba"**
→ Selecciona `.venv/bin/python` com a kernel a Cursor

**"Import error amb CrewAI"**
→ Executa `uv sync` de nou a la carpeta del projecte

---

## 🔒 Seguretat

**⚠️ MOLT IMPORTANT:**

❌ **MAI pugis a Git:**
- `.env` (conté API Keys)
- `credentials.json` (OAuth Gmail)
- `token.json` (OAuth Gmail)

✅ Aquests fitxers ja estan al `.gitignore`

✅ Si comparteixes codi, **elimina sempre les API Keys** abans

---

## 📝 Llicència

Aquest material està creat per Jordi Beringues de **JCM Technologies, SAU** i està destinat a introduir al món dels agents a tothom qui tingui interès en el tema.

---

## 👥 Contacte

**Formador:** Jordi Beringues  
**Departament:** R+D  
**Empresa:** JCM Technologies, SAU

---

## 🎉 Preparat per començar?

1. ✅ Verifica que tens Python 3.10+ i Git instal·lats
2. ✅ Clona el repositori
3. ✅ Obre `00_setup_crewai.ipynb` a Cursor
4. ✅ Segueix les instruccions del Setup
5. 🚀 **Gaudeix de la formació!**

---

*Última actualització: Gener 2026*