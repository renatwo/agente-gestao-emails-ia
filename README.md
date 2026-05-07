# Agente de Gestão de E-mails com IA

Projeto de automação com n8n, Gmail, Google Vertex AI e Telegram para gestão inteligente de e-mails.

## O que o projeto faz

- Verifica novos e-mails no Gmail.
- Analisa assunto e conteúdo com IA.
- Classifica por categoria.
- Aplica etiquetas inteligentes no Gmail.
- Marca e-mails urgentes com estrela.
- Envia notificações no Telegram.
- Cria rascunhos de resposta para revisão humana antes do envio.
- Permite consultar e-mails via Telegram em um segundo workflow sob demanda.

## Categorias utilizadas

- Trabalho
- Financeiro
- Urgente
- Newsletter
- Cursos
- IA
- Publicidade
- Spam/Suspeito

## Workflows

### 1. Agente de Gestão de E-mails

Arquivo:

```text
workflows/agente-gestao-email-vertex-ai-com-rascunho.public.json
```

Responsável por receber novos e-mails, classificar com IA, aplicar labels, marcar urgentes com estrela, criar rascunhos e enviar notificações.

### 2. Chat Telegram para consultar e-mails

Arquivo:

```text
workflows/chat-telegram-consultar-emails.public.json
```

Responsável por responder perguntas feitas pelo Telegram, buscar e-mails no Gmail e resumir os resultados com IA.

## Stack utilizada

- n8n
- Gmail API
- Google Vertex AI
- Telegram Bot
- Google OAuth2
- JavaScript
- API REST

## Segurança

Este repositório foi preparado para publicação e não contém tokens, senhas, client secrets, service accounts, chat IDs reais ou credenciais reais.

Antes de usar, substitua os placeholders nos workflows:

```text
REPLACE_WITH_TELEGRAM_CHAT_ID
REPLACE_WITH_GOOGLE_CLOUD_PROJECT_ID
REPLACE_LABEL_ID_TRABALHO
REPLACE_LABEL_ID_FINANCEIRO
REPLACE_LABEL_ID_URGENTE
REPLACE_LABEL_ID_NEWSLETTER
REPLACE_LABEL_ID_CURSOS
REPLACE_LABEL_ID_IA
REPLACE_LABEL_ID_PUBLICIDADE
REPLACE_LABEL_ID_SPAM_SUSPEITO
```

Depois de importar no n8n, selecione suas próprias credenciais:

- Gmail OAuth2
- Google OAuth2 API
- Google Vertex AI
- Telegram API

## Autor

Projeto desenvolvido por Renato Alves Queiroz.
