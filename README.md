# 🧠 Segundo Cérebro: Automação de Workflows com n8n e Docker

## 🎯 Objetivo
Dominar a implantação e configuração do n8n autohospedado utilizando contêineres Docker, capacitando a automação de workflows, integrações de APIs e orquestração de processos em engenharia de software.

## 📚 Fontes Utilizadas
- **Deploy | n8n Docs:** Fonte primária para configuração do ambiente e persistência de dados.
- **Manuals | Docker Docs:** Base técnica para comandos e gerenciamento das redes de contêineres.
- **N8N + Docker Setup Tutorial (2026):** Demonstração prática da configuração inicial e levantamento do serviço.
- **How To Build An Agent With n8n And Docker:** Abordagem prática sobre a criação de fluxos avançados e integração de Agentes de IA.

## 🤖 Diretriz de Comportamento (Prompt)
"Comporte-se como um Engenheiro de Software Especialista em DevOps e Automação de Processos. Forneça explicações técnicas, estruturadas e práticas sobre n8n e Docker, baseando-se estritamente nas fontes fornecidas. Utilize exemplos de linha de comando, estruturação de arquivos e boas práticas."

## 💬 Interações com a IA
*(Nota: Os prints com as provas das citações documentais destas respostas estão anexados nos arquivos deste repositório).*

**Pergunta 1: Como configurar o mapeamento de rede para integrar o n8n no Docker com serviços locais como o Ollama?**
**Resposta da IA:** É necessário exportar a variável `OLLAMA_HOST="0.0.0.0"` para que o serviço aceite conexões vindas das pontes (*bridge networks*) do Docker. Dentro das credenciais do n8n, deve-se apontar para o IP real da interface de rede da máquina hospedeira (ex: 192.168.1.X:11434).

**Pergunta 2: Quais são os componentes obrigatórios e opcionais ao construir um nó de AI Agent no n8n?**
**Resposta da IA:** O nó do agente de IA precisa de componentes conectados a ele para não ficar inativo. A memória (memory) e as ferramentas (tools) são opcionais. No entanto, é obrigatório adicionar e conectar um modelo de chat (chat model) clicando no sinal de adição (+).

## 🔗 Link do Notebook (Segundo Cérebro)
https://notebook.google.com/notebook/701332a7-18ed-4f5e-a3c3-113984a328c6
