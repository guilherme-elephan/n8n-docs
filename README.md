# 🐘 Integração Elephan + n8n

Automatize seus workflows conectando a Elephan ao n8n.

Com essa integração, você pode:
- Monitorar reuniões automaticamente  
- Reagir a sentimentos negativos  
- Enviar resumos por email ou Slack  
- Integrar com CRM, planilhas e outras ferramentas  

---

## 🚀 Pré-requisitos

Antes de começar, você precisa:

- Conta ativa na Elephan  
- Conta no n8n  
- Uma API Key da Elephan  

---

## 🔑 1. Gerar API Key na Elephan

1. Acesse a plataforma Elephan  
2. Vá em **Configurações → API / Integrações**  
3. Clique em **Gerar nova API Key**  
4. Copie a chave gerada  

> ⚠️ **Importante:**  
> Guarde sua API Key com segurança. Ela dá acesso aos seus dados.

---

## ⚙️ 2. Configurar credencial no n8n

No n8n:

1. Acesse **Credentials**  
2. Clique em **New Credential**  
3. Escolha **Generic Credential Type**  
4. Selecione **Bearer Auth**  

Preencha:
Authorization: Bearer SUA_API_KEY
Substitua `SUA_API_KEY` pela chave gerada na Elephan.

---

## 📥 3. Importar workflows

1. Baixe os arquivos `.json` fornecidos  
2. No n8n, clique em **Import Workflow**  
3. Selecione o arquivo desejado  
4. Associe a credencial criada  

---

## 🔄 Workflows disponíveis

### Workflows base

- **Sync Transcribes** → Lista reuniões  
- **Sync Users** → Lista usuários  
- **Sync Prompts** → Lista prompts  

### Workflows de exemplo

- **Alert Negative Sentiment** → Envia alerta quando uma reunião possui sentimento negativo  
- **Send Summary Email** → Envia automaticamente o resumo da reunião por email  

---

## ▶️ 4. Executar automação

1. Abra o workflow desejado  
2. Clique em **Execute Workflow** para testar  
3. Ative o workflow para execução automática  

---

## 💡 Exemplos de uso

### 🔴 Alerta de sentimento negativo

Sync Transcribes → Filtrar NEGATIVE → Enviar Email/Slack


---

### 📩 Envio automático de resumo


Sync Transcribes → Extrair resumo → Enviar Email


---

### 📊 Registro em planilha


Sync Transcribes → Google Sheets


---

## 🔐 Segurança

- Nunca compartilhe sua API Key  
- Utilize apenas em ambientes confiáveis  
- A Elephan aplica rate limiting nas requisições  

---

## 🛠️ Troubleshooting

### Não retorna dados

- Verifique se a API Key está correta  
- Confirme que o endpoint está acessível  

### Workflow não executa

- Verifique se o workflow está ativo  
- Teste manualmente com **Execute Workflow**  

---

## 📌 Observações

- Os workflows base fornecem os dados  
- Os exemplos mostram como usar esses dados  
- Você pode adaptar os fluxos conforme sua necessidade  

---

## 🎯 Conclusão

Com essa integração, você pode automatizar completamente o fluxo de análise de reuniões da Elephan dentro do n8n, conectando com email, Slack, CRM e outras ferramentas.
