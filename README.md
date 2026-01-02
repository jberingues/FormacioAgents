# Formació d'Agents d'IA amb CrewAI
## JCM Technologies - Departament de R+D

![CrewAI](https://img.shields.io/badge/CrewAI-0.80+-blue)
![Python](https://img.shields.io/badge/Python-3.10+-green)
![Google Gemini](https://img.shields.io/badge/Gemini-2.0-orange)

Repositori oficial per a la formació interna d'agents d'IA utilitzant CrewAI i Google Gemini.

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

## ⚙️ Pre-requisits

Abans de començar, assegura't de tenir instal·lat:

### **1. Software necessari**

| Software | Versió mínima | Com instal·lar |
|----------|---------------|----------------|
| **Python** | 3.10+ | https://www.python.org/downloads/ |
| **Git** | Qualsevol | https://git-scm.com/ |
| **Cursor** | Última | https://cursor.sh/ (o VS Code) |

**Nota:** **UV** (gestor de dependències) s'instal·larà automàticament durant el Setup (Secció 2).

### **2. Comptes necessaris**

- ✅ **Compte Google/Gmail no JCM** (per API Keys i Gmail API)
- ✅ **Accés a Google AI Studio** - https://aistudio.google.com/
- ✅ **Accés a Google Cloud Console** - https://console.cloud.google.com/ (per Part 3)

### **3. Verificar instal·lació**

Abans de clonar el repositori, verifica que tens:
```bash
python --version    # Ha de ser 3.10+
git --version       # Qualsevol versió recent
```

**Nota:** UV es verificarà automàticament durant el Setup.

---

## 🚀 Instruccions d'Instal·lació

### **Pas 1: Clonar el repositori**
```bash
git clone https://github.com/jcm-tech/formacioagents.git
cd formacioagents
```

### **Pas 2: Obrir a Cursor**

1. Obre **Cursor**
2. `File` → `Open Folder...`
3. Selecciona la carpeta `formacioagents/`

### **Pas 3: Executar el Setup**

1. Obre el notebook `00_setup_crewai.ipynb`
2. Segueix les instruccions pas a pas
3. Executa totes les cel·les amb `Shift+Enter`

El Setup farà automàticament:
- ✅ Instal·lar UV (gestor de dependències)
- ✅ Crear l'entorn virtual `.venv`
- ✅ Instal·lar totes les dependències (CrewAI, Gemini, Gmail API, etc.)
- ✅ Configurar API Keys
- ✅ Verificar que tot funciona

**⏱️ Temps estimat:** 10-15 minuts

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

Aquest material és propietat de **JCM Technologies, SAU** i està destinat exclusivament a ús intern per a formació del personal del Departament de R+D.

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