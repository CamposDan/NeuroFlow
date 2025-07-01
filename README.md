# NeuroFlow

> Automatize o primeiro contato com leads usando IA e ganhe escala, personalização e agilidade.

## 📊 Descrição Resumida

O NeuroFlow é um projeto criado para resolver um dos principais gargalos das áreas de marketing e vendas: a demora ou falta de personalização no primeiro contato com leads. 

Com base em uma arquitetura low-code usando **n8n**, **OpenRouter (IA generativa)**, **SMTP (Gmail)** e **Google Sheets**, criamos um fluxo automatizado que:

- Recebe dados de um novo lead
- Gera uma mensagem personalizada com IA
- Envia o e-mail automaticamente
- Registra o contato em planilha ou CRM leve

## 💚 Stack de Tecnologia

- [n8n](https://n8n.io) (automatização visual dos fluxos)
- [OpenRouter](https://openrouter.ai) (API de IA generativa)
- [Gmail SMTP](https://gmail.com) (envio automático de e-mails)
- [Google Sheets](https://sheets.google.com) (registro dos leads)

## 🔧 Funcionamento

O fluxo segue os seguintes passos:

1. **Webhook**: recebe os dados de um novo lead (nome e e-mail)
2. **HTTP Request**: envia prompt para o OpenRouter com base nos dados do lead
3. **E-mail**: a resposta gerada é enviada automaticamente para o lead via Gmail SMTP
4. **Registro**: salva os dados do lead + status de envio no Google Sheets

## 🏛️ Problemas que resolvemos

- Contato lento ou ineficaz com novos leads
- Baixa personalização no primeiro e-mail de boas-vindas
- Falta de registro automatizado das interações iniciais
- Dependência de mão de obra humana para processos repetitivos

## ✨ Benefícios

- Respostas automáticas em segundos
- IA personalizada com linguagem comercial
- Registros em planilha prontos para funil
- Pode ser integrado a qualquer tipo de captura de lead (formulário, CRM, landing page)

## 🎨 Demonstração Visual

Veja abaixo a representação visual do fluxo montado no n8n:

![Fluxo n8n NeuroFlow](./fluxo-n8n.png)

## 📄 Como Executar

1. Clone este repositório
2. Importe o JSON de workflow no seu ambiente n8n
3. Configure suas credenciais:
   - OpenRouter API Key
   - SMTP (Gmail com senha de app)
   - Planilha no Google Sheets (se desejar salvar os dados)
4. Dispare um teste via webhook com e-mail e nome fictício
5. Verifique a chegada do e-mail e o registro na planilha

## 🌍 Casos de uso

- Agências digitais
- Times comerciais B2B
- SaaS em onboarding
- Cursos online e EAD
- Freelancers e consultorias

## 🚀 Roadmap (Evolução futura)

- Integração com CRMs como HubSpot ou Pipedrive
- Tradução automática com IA para leads internacionais
- Disparo via WhatsApp com API oficial
- Interface frontend simples para disparo manual via link

---

Feito com ❤️ para mostrar que IA pode ser simples, útil e poderosa.

---

**Licença**: MIT

