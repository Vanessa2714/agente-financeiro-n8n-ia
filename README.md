# Agente Autónomo de Gestão Financeira (n8n + LLM + Telegram)

# Visão Geral do Projeto
Desenvolvimento de uma solução end-to-end de automação inteligente para gestão e registo de dados financeiros. O sistema recebe mensagens de texto via Telegram, utiliza um modelo de linguagem (LLM) para extração de entidades e categorização, e armazena os dados processados automaticamente em uma planilha.

# Tecnologias & Ferramentas
* *Orquestração de Fluxos:* n8n (Docker / WSL 2)
* *Inteligência Artificial:* OpenAI GPT / Google Gemini (Prompt Engineering com saída em JSON estrito)
* *Integração & Mensagaria:* APIs / Webhooks de integração com Telegram
* *Dados:* JSON

# Como Funciona a Solução
1. *Entrada de Dados:* O utilizador envia uma mensagem natural no Telegram (ex: "Gastei R$ 45 no almoço hoje").
2. *Processamento Inteligente (LLM):* O prompt estruturado interpreta a intenção, identifica o valor, a categoria e a data, convertendo a mensagem para um formato JSON validado.
3. *Automação & Persistência (n8n):* O fluxo no n8n encaminha os dados para a base de dados/planilha e envia uma confirmação imediata ao utilizador no Telegram.

#  Impacto & Resultados
* *Zero entrada manual de dados:* Eliminação da necessidade de preenchimento manual de formulários.
* *Redução de tempo:* Processamento e registo executados em menos de 3 segundos por transação.
* *Escalabilidade:* Arquitetura modular pronta para integração de novas métricas e relatórios financeiros.

---
Desenvolvido por Vanessa Batista
