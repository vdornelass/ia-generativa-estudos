# Roadmap: Agentes de IA (AI Agents - PT-BR)

> Baseado no roadmap oficial do **roadmap.sh/ai-agents**, traduzido e estruturado em português para estudo e consulta no NotebookLM.

## Roadmaps Relacionados
- Roadmap de Engenheiro de IA
- Roadmap de IA e Ciência de Dados
- Roadmap de MLOps
- Roadmap de Red Teaming em IA
- Roadmap de Engenharia de Prompt

---

## 1. Aprenda os Pré-requisitos
- **Desenvolvimento Backend Básico** → *Roadmap de Backend para Iniciantes*
- **Uso de Git e Terminal** → *Roadmap de Git e GitHub*
- **Conhecimento de APIs REST** → *Roadmap de Design de APIs*

---

## 2. Fundamentos de LLMs

### Entenda o Básico
- **Respostas com vs sem Streaming**
- **Modelos de Raciocínio (Reasoning) vs Padrão**
- **Fine-tuning vs Engenharia de Prompt**
- **Embeddings e Busca Vetorial**
- **Entenda o Básico de RAG (Retrieval-Augmented Generation)**
- **Precificação de Modelos Comuns**

### Famílias de Modelos e Licenças
- **Modelos de Pesos Abertos (Open Weight)** (ex: Llama, Mistral, Qwen, DeepSeek)
- **Modelos Proprietários (Closed Weight)** (ex: GPT, Claude, Gemini)

### Modelos Transformer e LLMs
- **Mecânica dos Modelos**:
  - **Tokenização**
  - **Janelas de Contexto (Context Windows)**
  - **Precificação Baseada em Tokens**
- **Controles de Geração**:
  - **Temperatura (Temperature)** e **Top-p**
  - **Penalidade de Frequência (Frequency Penalty)**
  - **Penalidade de Presença (Presence Penalty)**
  - **Critérios de Parada (Stopping Criteria / Stop Sequences)**
  - **Comprimento Máximo (Max Length / Max Tokens)**

---

## 3. Agentes de IA 101 (Fundamentos de Agentes)
- **O que são Agentes de IA?**
- **O que são Ferramentas (Tools)?**

### Loop do Agente (Agent Loop)
1. **Percepção / Entrada do Usuário**
2. **Raciocínio e Planejamento**
3. **Ação / Chamada de Ferramenta (Tool Call)**
4. **Observação e Reflexão**

### Exemplos de Casos de Uso
- **Assistente pessoal**
- **Geração de código**
- **Análise de dados**
- **Web Scraping / Crawling**
- **NPC / IA para Jogos**

---

## 4. Engenharia de Prompt para Agentes
- **O que é Engenharia de Prompt**
- **Escrevendo Bons Prompts**:
  - Seja específico no que você quer
  - Forneça contexto adicional
  - Use termos técnicos relevantes
  - Use exemplos no seu Prompt (Few-Shot)
  - Itere e teste seus Prompts
  - Especifique tamanho, formato, etc.
  - Trilha dedicada: *Roadmap de Engenharia de Prompt*

---

## 5. Ferramentas / Ações (Tools & Actions)

### Definição de Ferramenta (Tool)
- **Nome e Descrição** claros para o LLM saber quando invocar
- **Schema de Entrada / Saída** (JSON Schema / Pydantic / Zod)
- **Tratamento de Erros** e retorno amigável para o agente se recuperar
- **Exemplos de Uso**

### Exemplos de Ferramentas
- **Busca na Web (Web Search)**
- **Execução de Código / REPL (Code Interpreter / Sandbox)**
- **Consultas a Banco de Dados (SQL / NoSQL / Vetorial)**
- **Requisições de API (REST / GraphQL)**
- **E-mail / Slack / SMS**
- **Acesso ao Sistema de Arquivos (File System)**

---

## 6. Model Context Protocol (MCP)
- **Criando Servidores MCP**
- **Componentes Principais**:
  - **Hosts MCP**
  - **Cliente MCP**
  - **Servidores MCP**
- **Modos de Implantação (Deploy)**:
  - **Desktop Local (stdio)**
  - **Remoto / Nuvem (Cloud - SSE / Streamable HTTP)**

---

## 7. Memória do Agente (Agent Memory)
- **O que é Memória do Agente?**
- **Memória Episódica vs Semântica**

### Tipos de Memória por Duração
- **Memória de Curto Prazo (Short-Term Memory)**: Dentro do Prompt / Histórico da sessão atual.
- **Memória de Longo Prazo (Long-Term Memory)**: Banco Vetorial / SQL / Armazenamento Customizado.

### Mantendo a Memória
- **RAG e Bancos de Dados Vetoriais**
- **Armazenamento de Perfil do Usuário**
- **Sumarização / Compressão de Contexto**
- **Estratégias de Esquecimento (Forgetting / TTL / Relevância)**

---

## 8. Arquiteturas de Agentes

### Arquiteturas Comuns
- **Agente RAG (Agentic RAG)**
- **ReAct (Raciocinar + Agir / Reason + Act)**
- **Cadeia de Pensamento (Chain of Thought - CoT)**

### Outros Padrões de Arquitetura
- **Planejador-Executor (Planner-Executor)**
- **Agentes em Grafo (DAG / State Graph)**
- **Árvore de Pensamentos (Tree of Thoughts - ToT)**

---

## 9. Construindo Agentes

### Manual (do zero / From Scratch)
- Chamadas diretas à API do LLM
- Implementando o loop do agente manualmente
- Parsing da saída do modelo
- Tratamento de erros e Rate-limit

### "Function Calling" Nativo do LLM
- **OpenAI Function Calling**
- **OpenAI Assistants / Agents API**
- **Gemini Function Calling**
- **Anthropic Tool Use**

### Construindo com Frameworks
- **LangChain**
- **LlamaIndex**
- **Haystack**
- **AutoGen**
- **CrewAI**
- **Smolagents / Smol Depot (e LangGraph)**

---

## 10. Avaliação, Testes e Observabilidade

### Avaliação e Testes (Evals)
- **Métricas para Acompanhar** (taxa de sucesso, precisão de tool call, latência, custo)
- **Testes Unitários de Ferramentas**
- **Testes de Integração de Fluxos (Trajetórias)**
- **Avaliação Human-in-the-Loop**
- **Frameworks de Avaliação**:
  - **LangSmith**
  - **DeepEval**
  - **Ragas**

### Depuração e Monitoramento
- **Logs estruturados e Tracing**
- **Ferramentas de Observabilidade**:
  - **LangSmith**
  - **Helicone**
  - **LangFuse**
  - **OpenLLMetry**

---

## 11. Segurança e Ética em Agentes de IA
- **Prompt Injection / Jailbreaks**
- **Sandboxing e Permissões de Tools (Least Privilege)**
- **Privacidade de Dados + Redação de PII (LGPD)**
- **Guardrails de Viés e Toxicidade**
- **Segurança + Testes de Red Team**

---

## Trilhas Relevantes para Continuar
- **Engenheiro de IA**
- **IA e Ciência de Dados**
