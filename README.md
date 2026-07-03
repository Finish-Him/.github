# Finish-Him `.github` (meta-repo)

Meta-repo da conta GitHub **Finish-Him** (projetos pessoais de Moises Costa). Serve como índice dos repositórios da conta e como local para *community health files* padrão (templates de PR/issue, `SECURITY.md` etc.), que o GitHub aplica automaticamente aos repos da conta que não tenham os seus próprios.

Não há código aqui: sem stack, sem build, sem deploy — apenas Markdown.

> **Nota sobre CODEOWNERS:** o GitHub **não** propaga `CODEOWNERS` a partir do repo `.github` de conta de usuário (não é um community health file suportado). O arquivo que existia aqui era decorativo e foi removido em 2026-07. Repos que precisarem de code owners devem manter o próprio arquivo em `<repo>/.github/CODEOWNERS`.

## Repositórios da conta (2026-07-03)

Fonte: `gh repo list Finish-Him`. 29 repositórios — todos privados, exceto onde indicado.

### Meta / documentação

| Repo | Notas |
|------|-------|
| `.github` | Este repo (público). Índice da conta e community health files. |
| `Finish-Him` | README de perfil (público). |
| `workspace-meta` | Meta-docs do workspace local (CLAUDE.md, ARCHITECTURE.md, notas de produção). |
| `workspace-docs` | Documentação visual do workspace em HTML. Privado (contém IPs de infra). |
| `sessoes-ai-2026-docs` | Docs de sessões de IA 2026. |

### Educação / concursos (AprovAI)

| Repo | Notas |
|------|-------|
| `aprovai` | Plataforma de IA para concurseiros brasileiros. |
| `aprovai-oab` | Base de produto do vertical OAB (visão, roadmap, marketing, conteúdo). |
| `concurso-vault` | Vault Obsidian de estudos para concurso (backup). |

### Dados / apostas

| Repo | Notas |
|------|-------|
| `dota-oracle` | Análise de dados de Dota 2. |
| `dota2-dashboard` | Dashboard de Dota 2. |
| `polymarket-edge` | Engine de dados + modelo de edge para apostas na Polymarket (Dota 2 + Copa 2026). |
| `gm-bank-invest` | Gestão de banca / investimentos. |
| `sporting-villa` | Projeto de apostas esportivas. |

### Sites / landing pages

| Repo | Notas |
|------|-------|
| `portfolio` | Site/portfolio pessoal. |
| `fast-baterias` | Landing page de delivery de baterias com wizard de agendamento. |
| `msc-labs-landing` | Landing MSC Labs (treino de modelos custom / inferência gerenciada). |
| `landing-ia` | Landing de autoridade — funil Google Ads para o guia de IA. |
| `web-starters` | Starters/templates web (Next.js + Supabase). |

### IA / agentes / conhecimento

| Repo | Notas |
|------|-------|
| `atlas-v2` | Agente RAG com WhatsApp, UI na Vercel e API na VPS. |
| `awesome-claude-skills` | Lista curada de Claude Skills (público). |
| `whatsapp-vault` | Curadoria e política do corpus WhatsApp (105 conversas, 91 mil mensagens). |
| `msc-ai-playbook` | Playbook de IA da MSC: decisão estratégica API+RAG, pesquisas, arquitetura, roadmap. |

### Tooling / ambiente

| Repo | Notas |
|------|-------|
| `pi-backup-config` | Backup do ambiente Pi: prompts, temas, configs, extensions, scripts. |
| `coding-harness` | Harness pessoal de coding agents (fork do harness-msc). |
| `providers` | Configs de providers. |

### MSC (inbound)

| Repo | Notas |
|------|-------|
| `msc-company` | Inbound — canônicos da MSC vivem na org `MSC-Company-Org`. |
| `msc-company-workspace` | Dashboard interno da MSC Company (auth, métricas de tokens, painel de investidores). |

### Arquivados

| Repo | Notas |
|------|-------|
| `hermes-bot` | Bot Telegram integrado ao Hermes Agent. |
| `ia-em-producao` | Guia em português para levar agentes de IA/RAG/LLMs a produção (público). |

## Estrutura

```
.github/
├── README.md     # este arquivo (índice da conta)
└── .gitignore
```

Futuro possível: `PULL_REQUEST_TEMPLATE.md`, `ISSUE_TEMPLATE/`, `SECURITY.md`, `FUNDING.yml` — esses sim são propagados pelo GitHub como padrão para os demais repos da conta.

## Como atualizar o índice

```bash
gh repo list Finish-Him --limit 100 --json name,description,isArchived,visibility
```

Atualize as tabelas acima quando repos forem criados, renomeados, arquivados ou mudarem de visibilidade.

## Contexto

A conta Finish-Him é uma das três usadas no workspace local (`2-Codigo/Finish-Him/`), ao lado das orgs `MSC-Company-Org` (holding MSC) e `Detran-RJ` (GovTech). Repos de produto da MSC que nasceram aqui tendem a migrar para `MSC-Company-Org` (ex.: `agenda-barber-salao`, hoje canônico lá).
