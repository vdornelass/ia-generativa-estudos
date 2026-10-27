# Roadmap: Engenharia de Prompt (Prompt Engineering - PT-BR)

> Baseado no roadmap oficial do **roadmap.sh/prompt-engineering**, traduzido e estruturado em português para estudo e consulta no NotebookLM.

## Roadmaps Relacionados
- Roadmap de Engenheiro de IA
- Roadmap de IA e Ciência de Dados
- Roadmap de MLOps
- Roadmap de Red Teaming em IA
- Roadmap de Engenharia de Prompt
- Roadmap de Agentes de IA

---

## 1. Introdução
- **LLMs e como eles funcionam?**
- **O que é um Prompt?**
- **O que é Engenharia de Prompt?**

### Modelos Oferecidos por Provedores
- **OpenAI** (GPT-4o, o1, o3, etc.)
- **Google** (Gemini)
- **Anthropic** (Claude)
- **Meta** (Llama)
- **xAI** (Grok)

### Terminologia Comum
- **LLM (Large Language Model)**
- **Tokens**
- **Janela de Contexto (Context Window)**
- **Alucinação (Hallucination)**
- **Agentes (Agents)**
- **Prompt Injection**
- **Pesos / Parâmetros do Modelo (Model Weights / Parameters)**
- **Fine-Tuning vs Engenharia de Prompt**
- **IA vs AGI (Artificial General Intelligence)**
- **RAG (Retrieval-Augmented Generation)**

---

## 2. Configuração de LLMs (LLM Configuration)

### Parâmetros de Sampling (Amostragem)
- **Temperatura (Temperature)**: Controla a aleatoriedade / criatividade vs determinismo da resposta.
- **Top-K**: Limita a amostragem aos K tokens mais prováveis.
- **Top-P (Nucleus Sampling)**: Limita a amostragem aos tokens cuja probabilidade acumulada atinge P.

### Controle de Saída (Output Control)
- **Max Tokens (Limite de Tokens)**: Define o tamanho máximo da resposta gerada.
- **Stop Sequences (Sequências de Parada)**: Define strings que interrompem a geração assim que produzidas.

### Penalidades de Repetição (Repetition Penalties)
- **Penalidade de Frequência (Frequency Penalty)**: Penaliza tokens proporcionalmente a quantas vezes já apareceram.
- **Penalidade de Presença (Presence Penalty)**: Penaliza tokens que já apareceram pelo menos uma vez, incentivando novos tópicos.

### Saídas Estruturadas (Structured Outputs)
- Geração garantida em formatos estruturados como **JSON (JSON Schema)**, **XML**, **Markdown**, **CSV**, etc.

---

## 3. Técnicas de Prompting (Prompting Techniques)

### Técnicas Base e Contextuais
- **Zero-Shot Prompting**: Pedir a tarefa diretamente sem exemplos prévios.
- **One-Shot / Few-Shot Prompting**: Fornecer 1 ou alguns exemplos de entrada/saída no prompt.
- **System / Role / Contextual Prompting**:
  - **System Prompting**: Define instruções globais e comportamento do modelo.
  - **Role Prompting**: Atribui uma persona ou papel especialista ao modelo.
  - **Contextual Prompting**: Fornece contexto de domínio e informações de fundo relevantes.

### Técnicas de Raciocínio Avançado
- **Step-back Prompting**: Faz o modelo abstrair conceitos e princípios gerais antes de responder ao caso específico.
- **Chain of Thought (CoT) Prompting (Cadeia de Pensamento)**: Instrui o modelo a raciocinar passo a passo antes da resposta final.
- **Self-Consistency Prompting**: Gera múltiplos caminhos de raciocínio (CoT) e seleciona a resposta mais consistente por votação.
- **Tree of Thoughts (ToT) Prompting (Árvore de Pensamentos)**: Explora múltiplos ramos de raciocínio com busca e auto-avaliação.
- **ReAct Prompting (Reason + Act)**: Intercala passos de raciocínio verbal (Thought) com chamadas de ação/ferramentas (Action) e observação (Observation).

### Engenharia de Prompt Automática (Automatic Prompt Engineering - APE)
- **Usar LLM para gerar Prompts**: Utilizar modelos de linguagem para criar, testar, avaliar e otimizar prompts automaticamente.

---

## 4. Segurança: AI Red Teaming
- **AI Red Teaming**: Testes adversariais para identificar vulnerabilidades, jailbreaks, vazamento de prompt e comportamentos inseguros.
- Trilha complementar: *Roadmap de AI Red Teaming*.

---

## 5. Boas Práticas de Prompting (Prompting Best Practices)
- Forneça exemplos **few-shot** para a estrutura ou estilo de saída que você precisa.
- Mantenha seus prompts **curtos e concisos**.
- Peça **saída estruturada** se ajudar (ex: JSON, XML, Markdown, CSV, etc.).
- Use **variáveis / placeholders** nos seus prompts para facilitar a configuração e reuso.
- Priorize dar **instruções mais claras** em vez de apenas acumular restrições negativas.
- Controle o **comprimento máximo da saída** (*Max Output Length*).
- Experimente diferentes **formatos de entrada** e estilos de escrita.
- Ajuste o **sampling** (`temperature`, `top-k`, `top-p`) equilibrando determinismo vs criatividade.
- Proteja contra **prompt injection**; sanitize e valide o texto enviado pelo usuário.
- **Automatize a avaliação (evals)**; integre testes unitários para validar as saídas do modelo.
- **Documente e rastreie versões de prompts** (*prompts como código*).
- Otimize para **latência e custo** em pipelines de produção.
- Documente **decisões, falhas e aprendizados** para futuros desenvolvedores.
- Delimite diferentes seções do prompt com **crases triplas (` ``` `)** ou **tags XML** (ex: `<contexto>...</contexto>`).

---

## 6. Melhorando a Confiabilidade (Improving Reliability)
- **Prompt Debiasing (Redução de Viés)**: Técnicas para mitigar vieses de posição, frequência ou exemplos no prompt.
- **Prompt Ensembling**: Combinar respostas de múltiplos prompts diferentes para a mesma tarefa.
- **Auto-Avaliação do LLM (LLM Self-Evaluation / LLM-as-a-Judge)**: Usar um LLM para verificar, criticar e pontuar a saída gerada.
- **Calibrando LLMs (Calibrating LLMs)**: Ajustar a distribuição de probabilidades e confiança das respostas do modelo.

---

## Próximos Passos
- Continue aprendendo com: **Roadmap Engenheiro de IA** e **Roadmap Agentes de IA**.
