# Finish-Him `.github` (meta-repo)

Este é o **meta-repo da organização `Finish-Him`** no GitHub.

Contém configurações compartilhadas que se aplicam a **todos os repos da org**:

- **`CODEOWNERS`** (raiz) — define quem revisa PRs por repo (GitHub auto-assign).

## Sobre Finish-Him

Organização pessoal/profissional do Moisés Costa para projetos paralelos:

- Aplicações OAB (`aprovai`, `aprovai-oab`)
- Análise de dados / Dota / Polymarket
- Apostas / banca (`agenda-barber-salao`, `gm-bank-invest`, `sporting-villa`)
- Portfolio / sites pessoais (`portfolio`, `fast-baterias`, `msc-labs-landing`, `web-starters`)
- Vaults / conhecimento (`concurso-vault`, `whatsapp-vault`, `atlas-v2`, `awesome-claude-skills`, `ia-em-producao`)
- Tooling interno (`pi-backup-config`, `msc-ai-playbook`)

## Setup

Para usar como `.github` repo oficial no GitHub:

```bash
# 1. Criar repo no GitHub: Finish-Him/.github (public)
# 2. Push:
cd /c/Users/Moises\ e\ Naiara/workspace/2-Codigo/Finish-Him/.github
git remote add origin https://github.com/Finish-Him/.github.git
git push -u origin main
```

## Estrutura

```
.github/                  # este repo
├── CODEOWNERS            # assignment de reviewers
├── README.md             # este arquivo
└── (futuro) PULL_REQUEST_TEMPLATE.md
└── (futuro) workflows/
```
