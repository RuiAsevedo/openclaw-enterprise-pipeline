# Autonomous AI Agent for Intelligent Media Curation
## Framework OpenClaw & Integração com Large Language Models (LLMs)

### 1. Visão Geral
Este repositório documenta o desenvolvimento e a implementação de um agente de inteligência artificial autônomo projetado para otimização de fluxos de trabalho (pipelines) de mídia digital. O sistema utiliza o framework **OpenClaw** para orquestrar a interação entre modelos de linguagem de larga escala (LLMs), ferramentas de navegação web e utilitários de sistema operacional Linux.

### 2. Arquitetura do Sistema
A solução foi arquitetada em uma instância de computação em nuvem (**GCP/Ubuntu**), priorizando a modularidade e a autonomia decisória do agente.

* **Orquestração de Inteligência:** Utilização do modelo **Gemini 1.5 Pro** via Google AI Studio, permitindo o raciocínio complexo sobre diretrizes de curadoria.
* **Camada de Conectividade:** Integração com a **Brave Search API** para extração de dados em tempo real e indexação de metadados da web.
* **Interface de Comando e Controle (C2):** Implementação de um gateway via Telegram Bot para monitoramento remoto e submissão de prompts assíncronos.

### 3. Componentes Técnicos e Ferramentas
O ecossistema de autonomia baseia-se na integração sinérgica das seguintes tecnologias:

| Componente | Tecnologia | Função |
| :--- | :--- | :--- |
| **Runtime** | Node.js / Python | Execução do framework de agentes |
| **Media Processing** | `yt-dlp` & `ffmpeg` | Extração e manipulação de fluxos de vídeo/áudio |
| **Automation** | Chromium (Headless) | Navegação e interação com o DOM para validação de licenças |
| **Persistence** | Systemd Service | Gerenciamento de daemon para alta disponibilidade do sistema |

### 4. Metodologia de Autonomia
O agente opera sob uma política de segurança **Full Autonomy (Mode: Allow)**, permitindo a execução de comandos de nível administrativo (`sudo`) sem intervenção humana para:
* Provisionamento dinâmico de dependências (instalação de pacotes).
* Gestão de sistemas de arquivos e limpeza de diretórios temporários.
* Roteamento de requisições através de proxies de navegação internos.

### 5. Casos de Uso
O projeto foca na validação da autonomia de agentes em tarefas de:
1.  **Curadoria Inteligente:** Filtragem de conteúdo sob parâmetros legais específicos (Creative Commons).
2.  **ETL de Mídia:** Extração, Transformação e Carga de dados audiovisuais para canais automatizados.

### 6. Infraestrutura e Integrações de API
O ecossistema de autonomia foi expandido através de protocolos de autenticação e comunicação de nível empresarial:

* **Cloud Hosting:** Provisionamento de VM em **Google Cloud Platform (GCP)** com otimização de recursos para execução de agentes de IA.
* **Interface C2 (Command & Control):** Implementação de bot via **Telegram API** para monitoramento de logs e controle remoto assíncrono.
* **Social Data Pipeline:** Integração com **Meta Graph API** para automação de interações e coleta de dados em redes sociais.
* **Autenticação Segura:** Implementação de fluxos **Google OAuth 2.0** para acesso seguro a serviços de terceiros e gerenciamento de permissões.

---
**Desenvolvido por Rui Asevedo (Charlie)** *Estudante de Tecnologia em Gestão da TI | Foco em AI Engineering*
