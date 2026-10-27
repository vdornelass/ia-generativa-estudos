# 🧠 Estudos de IA Generativa: Prompt Engineering & AI Agents

Repositório central de estudos, roadmaps visuais, fontes para o **NotebookLM**, notebooks interativos (`.ipynb`), anotações, exemplos de código e projetos práticos em **Engenharia de Prompt** e **Agentes de IA**.

---

## 🔗 Meu Caderno no NotebookLM
- **Link do NotebookLM**: `[Cole aqui o link do seu caderno no NotebookLM](https://notebooklm.google.com/)`
- As fontes dos roadmaps em Markdown e PDF ficam em [`notebooklm/fontes/`](./notebooklm/fontes/) e [`roadmaps/`](./roadmaps/).

---

## 📂 Estrutura do Repositório

```text
ia-generativa-estudos/
├── roadmaps/                        # Diagramas visuais (.excalidraw e .pdf em PT-BR)
│   ├── prompt-engineering-roadmap-pt.excalidraw
│   ├── prompt-engineering-roadmap-pt.pdf
│   ├── ai-agents-roadmap-pt.excalidraw
│   └── ai-agents-roadmap-pt.pdf
│
├── notebooklm/                      # Integração e materiais do Google NotebookLM
│   ├── fontes/                      # Roadmaps em .md prontos para subir no NotebookLM
│   └── resumos-gerados/             # Espaço para guias e resumos exportados do NotebookLM
│
├── anotacoes/                       # Caderno de anotações em Markdown (em construção)
├── exemplos-codigo/                 # Scripts e notebooks (.ipynb) práticos (em construção)
└── projetos/                        # Projetos práticos da trilha (em construção)
```

---

## 🗺️ Progresso nos Roadmaps

### Parte 1: Engenharia de Prompt ([PDF](./roadmaps/prompt-engineering-roadmap-pt.pdf) | [Excalidraw](./roadmaps/prompt-engineering-roadmap-pt.excalidraw))
- [ ] **1. Introdução & Terminologia**: Tokens, Janela de Contexto, Alucinação, Pesos/Parâmetros, Fine-Tuning vs Prompt Eng., RAG
- [ ] **2. Configuração de LLMs**: Temperature, Top-K, Top-P, Max Tokens, Stop Sequences, Frequency & Presence Penalty, Structured Outputs
- [ ] **3. Técnicas Base**: Zero-Shot, One-Shot / Few-Shot, System / Role / Contextual Prompting
- [ ] **4. Técnicas de Raciocínio**: Step-back, Chain of Thought (CoT), Self-Consistency, Tree of Thoughts (ToT), ReAct
- [ ] **5. Automação & Confiabilidade**: Automatic Prompt Engineering (APE), Prompt Debiasing, Prompt Ensembling, Self-Evaluation, Calibração
- [ ] **6. Boas Práticas & Red Teaming**: Delimitadores (XML / ` ``` `), Variáveis, Versionamento de Prompts, Sanitização contra Prompt Injection

### Parte 2: Agentes de IA ([PDF](./roadmaps/ai-agents-roadmap-pt.pdf) | [Excalidraw](./roadmaps/ai-agents-roadmap-pt.excalidraw))
- [ ] **1. Pré-requisitos & Fundamentos de LLMs**: Python/Backend, Git, APIs REST, Streaming, Modelos Open vs Closed Weight
- [ ] **2. Agentes de IA 101**: O Loop do Agente (Percepção → Raciocínio → Ação → Observação)
- [ ] **3. Ferramentas (Tools)**: Definição de Tools, JSON Schema, Execução de Código, Busca Web, APIs
- [ ] **4. Model Context Protocol (MCP)**: Hosts, Clientes, Servidores MCP Locais e Remotos
- [ ] **5. Memória do Agente & RAG**: Curto vs Longo Prazo, Episódica vs Semântica, Embeddings, Bancos Vetoriais, Sumarização
- [ ] **6. Arquiteturas de Agentes**: Agente RAG, ReAct, CoT, Planejador-Executor, Grafo (DAG), ToT
- [ ] **7. Construindo Agentes**: Loop Manual (do zero), Function Calling Nativo, Frameworks (LangGraph, LangChain, LlamaIndex, CrewAI, AutoGen)
- [ ] **8. Avaliação e Observabilidade**: Evals (LangSmith, DeepEval, Ragas), Logs Estruturados, Tracing (Langfuse, Helicone, OpenLLMetry)
- [ ] **9. Segurança e Ética**: Prompt Injection/Jailbreaks, Sandboxing de Tools, Redação de PII/LGPD, Guardrails, Red Teaming

---

## 🚀 Configuração do Ambiente Local

1. **Crie e ative um ambiente virtual Python**:
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```
2. **Instale as dependências**:
   ```powershell
   pip install -r requirements.txt
   ```
3. **Configure suas variáveis de ambiente**:
   ```powershell
   Copy-Item .env.example .env
   ```
