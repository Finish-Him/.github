# Governança da conta Finish-Him

Meta-repositório dos projetos pessoais de Moisés Costa. Ele documenta o portfólio técnico da conta e hospeda arquivos comunitários que podem ser herdados por outros repositórios.

## Visão geral

| Item | Definição |
|---|---|
| Status | Ativo |
| Tipo | Governança e índice |
| Código executável | Não |
| Repositórios acessíveis na conta | 19 |
| Organização empresarial | [Msc-Company-Org](https://github.com/Msc-Company-Org) |
| Organização pública | [Detran-RJ](https://github.com/Detran-RJ) |

## Projetos por domínio

### Inteligência artificial e conhecimento

| Repositório | Objetivo |
|---|---|
| `atlas-v2` | Agente RAG com WhatsApp |
| `whatsapp-vault` | Curadoria privada de conversas exportadas |
| `aprovai` | IA aplicada a concursos |
| `jarvis` | Assistente pessoal de voz |
| `polymarket-edge` | Pesquisa e paper trading |
| `awesome-claude-skills` | Repositório público de terceiros mantido como fork/cópia de referência |

### Portfólio e aplicações

| Repositório | Objetivo |
|---|---|
| `Finish-Him` | Perfil público |
| `portfolio` | Portfólio sincronizado |
| `finish-him-showcase` | Projetos demonstrativos |
| `landing-ia` | Landing profissional |
| `msc-company-workspace` | Workspace interno MSC |
| `nextjs-dashboard-app` | Template legado consolidado em `web-starters` |
| `web-starters` | Starters web reutilizáveis |

### Dados e jogos

| Repositório | Objetivo |
|---|---|
| `dota2-analytics` | Dashboard e predição de Dota 2 |
| `game-meta-db` | Base pessoal de metagame |
| `poker` | Estudos de estratégia para torneios |

### Ferramentas e governança

| Repositório | Objetivo |
|---|---|
| `.github` | Este índice |
| `workspace-meta` | Estado e auditorias do workspace |
| `developer-tools` | Dashboards e configurações de desenvolvimento |

## Arquivos comunitários

Quando presentes nos caminhos suportados pelo GitHub, estes arquivos podem definir padrões para repositórios que não possuam configuração própria:

- `CONTRIBUTING.md`;
- `SECURITY.md`;
- templates de issue;
- template de pull request.

`CODEOWNERS` não é herdado a partir do `.github` de uma conta pessoal. Cada projeto que precisar dessa regra deve manter seu próprio arquivo.

## Regras de organização

- produtos empresariais canônicos pertencem à [Msc-Company-Org](https://github.com/Msc-Company-Org);
- projetos do Detran-RJ pertencem à [Detran-RJ](https://github.com/Detran-RJ);
- esta conta mantém identidade profissional, experimentos e ferramentas pessoais;
- novos repositórios devem possuir propósito, estado, execução, segurança e destino claramente documentados.

## Atualização do índice

```bash
gh repo list Finish-Him --limit 100 \
  --json name,description,isArchived,visibility
```

Revise este documento quando um projeto for criado, migrado ou arquivado.
