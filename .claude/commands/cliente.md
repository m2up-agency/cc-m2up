---
name: cliente
description: Cria pasta de novo cliente com briefing pré-estruturado. Entrevista o usuário sobre o cliente e preenche o briefing automaticamente. Use quando o usuário disser "novo cliente", "adicionar cliente", "criar pasta do cliente X" ou chamar /cliente.
---

# /cliente — Cadastrar Novo Cliente

## O que fazer

Guiar o usuário numa entrevista sobre o novo cliente e criar a pasta com o briefing já preenchido.

## Fluxo

**0. Verificar se tem arquivo de briefing**

Antes de perguntar qualquer coisa, checar se o usuário mencionou um arquivo ou se existe algum arquivo recente em `dados/` (PDF, DOCX, TXT, MD). Se sim, ler o arquivo e extrair as informações automaticamente, pulando as perguntas que já foram respondidas.

**1. Fazer as perguntas abaixo** (pode agrupar em blocos temáticos pra não parecer um interrogatório):

**Identificação:**
- Nome da empresa/marca?
- E-mail do contato?
- Site e landing pages?

**Objetivo e processo comercial:**
- Qual o objetivo com os anúncios? (leads, vendas, tráfego, branding)
- Como realiza as vendas? (WhatsApp, formulário, ligação, e-commerce, consultivo)
- Quem faz o atendimento? Qual o WhatsApp de contato?

**Produto e mercado:**
- Quais os principais serviços/produtos?
- Por que as pessoas compram? O que diferencia?
- Como a marca se posiciona em preço? (média / acima / abaixo / premium / baratão)
- Tem alguma promoção ou oferta especial pra destacar?

**Público e geografia:**
- Perfil do cliente ideal? (idade, renda, sexo, região, estilo de vida)
- Para qual região vende?
- Qual o ticket médio? (faturamento ÷ nº de vendas)
- Em quais horários e dias prefere veicular os anúncios?

**Campanha:**
- Qual o orçamento mensal de mídia?
- Quais plataformas? (Meta Ads, Google Ads ou ambos)
- Quais os 5+ diferenciais pra destacar nos anúncios?

**Concorrência:**
- Quais os 3 principais concorrentes?
- Tem alguma empresa que admira como referência?

**Materiais:**
- Tem pasta no Drive com criativos, logo e identidade visual? (link)
- Tem acesso ao domínio/hospedagem? (se aplicável)

**2. Com as respostas, criar a pasta e o briefing:**

- Pasta: `clientes/[nome-do-cliente-em-kebab-case]/`
- Arquivo: `clientes/[nome-do-cliente-em-kebab-case]/briefing.md`
- Usar o template de `clientes/_modelo/briefing.md` preenchido com as respostas

**3. Confirmar o que foi criado** mostrando o caminho da pasta e um resumo do briefing.

**4. Perguntar:** "Quer que eu já adicione a conta de anúncio no contas.yaml das skills?"
- Se sim, perguntar o account ID (Meta: act_XXX / Google: número da conta) e adicionar em `~/.claude/skills/[skill]/contas.yaml`
