# cc-m2up — Workspace Claude Code

Workspace pré-configurado da **m2up** para gestão de tráfego pago com Claude Code.
Skills de Google Ads, GA4 e Meta Ads prontas pra usar.

---

## Como instalar

### Opção 1 — Via prompt (mais fácil)

Com o Claude Code aberto em qualquer pasta, copie e cole esse prompt:

```
Instala pra mim o repositório https://github.com/m2up-agency/cc-m2up.git na pasta atual, abre ela e roda /setup
```

O Claude faz tudo: clona o repositório, entra na pasta e inicia a configuração.

---

### Opção 2 — Via terminal

**1. Clone o repositório**
```bash
git clone https://github.com/m2up-agency/cc-m2up.git
cd cc-m2up
```

**2. Abra no VS Code**
```bash
code .
```

**3. Abra o terminal integrado** (Ctrl + ` no Windows / Cmd + ` no Mac) e rode:
```bash
claude
```

**4. Chame o setup**
```
/setup
```

---

O Claude vai te fazer algumas perguntas e configurar o sistema pro seu negócio. Em 5 minutos você tem tudo pronto.

---

## O que vem no kit

**Skills prontas pra usar:**
- `/setup` — configura o sistema pro seu negócio (comece por aqui)
- `/iniciar` — carrega o contexto do negócio no começo de cada sessão de trabalho
- `/syncar` — salva o trabalho no GitHub (commit + push, configura na primeira vez)
- `/atualizar` — varre o projeto e atualiza os arquivos de contexto que ficaram desatualizados
- `/novo-projeto` — cria pasta de projeto novo com CLAUDE.md dedicado
- `/mapear` — entrevista sobre processos e cria skills personalizadas

**Skills de tráfego (instalar separadamente):**
- [google-ads-m2up](https://github.com/m2up-agency/google-ads-m2up) — Google Ads via API
- [ga4-m2up](https://github.com/m2up-agency/ga4-m2up) — Google Analytics 4
- [meta-ads-m2up](https://github.com/m2up-agency/meta-ads-m2up) — Meta Ads via SDK
- **ads-m2up** — Diagnóstico, relatório e auditoria *(disponível no curso)*

**Pastas geradas pelo `/setup`:**
- `_contexto/` — contexto do seu negócio e preferências
- `marca/` — guia de identidade visual da sua marca
- `templates/ferramentas/catalogo.md` — APIs, CLIs e MCPs disponíveis pra usar em skills

**Pasta `dados/`:**
- Drop zone pra arquivos que você quer analisar (CSV, XLSX, TXT, PDF)
- Use com `/analisar-dados dados/seu-arquivo.csv`

---

## Ficou travado?

Dúvidas: fala com a equipe m2up.
