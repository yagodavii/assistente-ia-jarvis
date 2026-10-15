# 🤖 JARVIS AI Assistant

Assistente local com Inteligência Artificial desenvolvido para conectar **linguagem natural, comandos de voz, orquestração de IA, controle de navegador e automação de workflows** em um único sistema de produtividade.

O projeto explora como agentes de IA podem transformar a intenção do usuário em ações reais, como abrir ferramentas, controlar fluxos no navegador, executar comandos locais, gerar documentos e automatizar tarefas do dia a dia.

---

## 🎯 Problema resolvido

Muitas tarefas repetitivas no computador ainda exigem interação manual, como:

- Abrir ferramentas e aplicativos
- Navegar entre sistemas
- Pesquisar informações
- Executar comandos
- Gerar documentos
- Controlar fluxos no navegador
- Alternar manualmente entre diferentes ferramentas de IA

O JARVIS foi criado para reduzir esse atrito, permitindo que o usuário interaja com um assistente local através de **voz e texto**, enquanto o sistema cuida da execução, orquestração e fallback entre diferentes ferramentas de IA.

---

## 💼 Aplicações do projeto

Esse tipo de assistente pode ser adaptado para cenários como:

- Assistentes internos de produtividade
- Automação de workflows com IA
- Operações de suporte
- Automação de tarefas de back-office
- Automação de processos via navegador
- Ferramentas de produtividade para desenvolvedores
- Geração de documentos e PDFs
- Orquestração entre diferentes modelos de IA

O principal valor está em reduzir tarefas manuais repetitivas e criar uma ponte entre **o raciocínio da IA e ações reais executadas em sistemas**.

---

## 🚀 Principais funcionalidades

- Interação por voz em tempo real
- Ativação através da wake word `Jarvis`
- Execução de comandos locais para aplicativos, URLs e tarefas do sistema
- Controle e automação do navegador
- Suporte à análise de tela
- Geração de PDFs
- Utilitários para workflows com documentos
- Claude Code como principal engine de raciocínio e desenvolvimento
- Codex CLI como mecanismo de fallback
- Retorno automático ao Claude quando o uso volta a estar disponível
- Orquestração entre diferentes ferramentas de IA
- Automação de workflows de produtividade

---

## 🧠 Arquitetura conceitual

O fluxo principal do assistente segue uma estrutura semelhante a:

```text
Usuário
   ↓
Voz / Texto
   ↓
Reconhecimento e normalização
   ↓
Interpretação da intenção
   ↓
Orquestração de IA
   ↓
Seleção de ferramenta ou ação
   ↓
Execução local / Navegador / Ferramenta
   ↓
Resultado
   ↓
Resposta ao usuário
```

A proposta é permitir que o assistente não apenas responda perguntas, mas também **transforme comandos em ações reais**.

---

## 🛠️ O que foi desenvolvido

A estrutura do assistente foi projetada e implementada incluindo:

- Fluxo de comandos por voz
- Normalização de comandos
- Tratamento de intenção
- Lógica para execução de tarefas locais
- Helpers para automação de navegador
- Orquestração de ferramentas de IA
- Fluxo de fallback entre Claude e Codex
- Configuração de ambiente
- Documentação
- Regras de segurança para comandos locais
- Proteções para operações potencialmente destrutivas

---

## 🗣️ Interação por voz

O JARVIS suporta comandos de voz em tempo real.

A ativação ocorre através da palavra:

```text
Jarvis
```

Depois da ativação, o sistema processa o comando, interpreta a intenção e direciona a solicitação para o fluxo correspondente.

Exemplos de ações:

- Abrir aplicativos
- Abrir URLs
- Executar comandos locais
- Iniciar automações
- Controlar fluxos no navegador
- Acionar ferramentas de IA

---

## 🧩 Orquestração de IA

O projeto utiliza diferentes ferramentas de IA dentro de um mesmo fluxo.

### Claude Code

Utilizado como principal engine para:

- Raciocínio
- Desenvolvimento
- Análise
- Apoio à execução de tarefas

### Codex CLI

Utilizado como mecanismo de fallback quando o uso do Claude não está disponível.

O sistema também possui lógica para retornar automaticamente ao Claude quando a ferramenta volta a estar disponível.

---

## 🌐 Automação de navegador

O JARVIS possui helpers para controle e automação de navegador.

Isso permite explorar fluxos como:

- Abrir páginas
- Navegar entre interfaces
- Executar ações repetitivas
- Automatizar processos web
- Integrar IA com ações no navegador

---

## 🖥️ Execução de tarefas locais

O assistente também pode executar tarefas diretamente no computador.

Exemplos:

- Abrir aplicativos
- Abrir URLs
- Executar comandos
- Acionar scripts
- Iniciar fluxos automatizados
- Executar tarefas previamente definidas

Operações sensíveis devem respeitar as regras de segurança definidas no projeto.

---

## 📄 Documentos e PDFs

O projeto possui suporte para geração de PDFs e utilitários relacionados a workflows com documentos.

Isso permite explorar cenários como:

- Geração automatizada de documentos
- Criação de PDFs
- Automação de tarefas documentais
- Integração entre IA e geração de arquivos

---

## 🔐 Segurança

Um dos desafios do projeto foi permitir automação local sem transformar o assistente em um executor irrestrito de comandos.

Foram consideradas práticas como:

- Manter código gerado por IA sob validação humana
- Tratar comandos destrutivos com cuidado
- Manter credenciais fora do repositório
- Utilizar variáveis de ambiente
- Evitar versionamento de arquivos locais ou sensíveis
- Criar regras para execução segura de comandos

---

## 🧪 Principais desafios técnicos

Alguns dos principais desafios encontrados durante o desenvolvimento foram:

- Mapear comandos naturais de voz para ações confiáveis
- Tratar diferentes variações de entrada falada
- Manter código gerado por IA sob validação humana
- Gerenciar fallback entre diferentes ferramentas de IA
- Evitar execução insegura de ações destrutivas
- Manter credenciais sensíveis fora do repositório
- Estruturar o projeto para permitir evolução para workflows mais agentic

---

## ⚙️ Stack utilizada

- Node.js
- Express
- OpenAI API
- Anthropic SDK
- Claude CLI
- Codex CLI
- Puppeteer
- Python
- Speech Recognition
- Voice Commands
- Browser Automation
- Workflow Automation

---

## 📋 Requisitos

Para executar o projeto:

- Node.js 18+
- Python 3.11+
- OpenAI API Key
- Claude Code CLI instalado e autenticado
- Codex CLI instalado e autenticado
- Google Chrome

---

## ▶️ Como executar

Instale as dependências:

```bash
npm install
```

Inicie o projeto:

```bash
npm run start
```

Por padrão, o servidor ficará disponível em:

```text
http://localhost:3000
```

---

## 🔑 Variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
OPENAI_API_KEY=your_openai_key
```

Adicione também outras credenciais locais necessárias para o seu ambiente.

> ⚠️ Nunca envie tokens, chaves ou credenciais para o repositório.

---

## 🛡️ Proteção de informações sensíveis

O repositório foi configurado para evitar o versionamento de arquivos sensíveis ou específicos da máquina, incluindo:

- `.env` e variações locais de ambiente
- `node_modules/`
- Logs
- Arquivos locais de memória e histórico
- Conteúdo gerado no workspace
- Documentos pessoais
- Arquivos locais de projetos

---

## 📈 Possibilidades de evolução

A estrutura atual permite futuras evoluções relacionadas a:

- Memória persistente
- RAG com documentos locais
- Agentes especializados
- Arquiteturas multiagentes
- Integração com sistemas corporativos
- Execução de workflows complexos
- Observabilidade de agentes
- Integração com novos modelos de IA
- Integração com APIs e serviços externos
- Expansão dos comandos por voz
- Novas automações de navegador
- Novos mecanismos de fallback
- Aprovação humana para operações sensíveis

---

## 🧠 O que este projeto demonstra

Este projeto demonstra experiência prática em:

- Inteligência Artificial aplicada
- Integração com LLMs
- Agentes de IA
- Orquestração de ferramentas de IA
- Automação de processos
- Automação de navegador
- Node.js
- Python
- Reconhecimento de voz
- Execução de tarefas locais
- Tratamento de intenção
- Integração com APIs
- Fallback entre ferramentas
- Segurança em automações
- Desenvolvimento de sistemas orientados por IA

---

## 🎯 Objetivo do projeto

O objetivo do JARVIS é explorar como **Inteligência Artificial, automação e engenharia de software** podem ser combinadas para transformar linguagem natural em ações reais.

Mais do que apenas responder perguntas, o projeto busca criar um assistente capaz de:

**entender → interpretar → selecionar ferramentas → executar → retornar resultados**
