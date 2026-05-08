# claude-skill-builder

Documentação e guia para criar, auditar e otimizar **skills do Claude Code** seguindo as práticas oficiais.

Skills são instruções reutilizáveis que ficam em `.claude/skills/[skill-name]/SKILL.md` e são carregadas pelo Claude quando você invoca via `/slash-command` ou descreve a tarefa em linguagem natural.

## Conteúdo

| Arquivo | O que tem |
|---|---|
| [`skill-builder.md`](./skill-builder.md) | Skill operacional (`/skill-builder`). Guia o processo de criação de uma nova skill via *Discovery Interview* (6 rodadas), checklist de auditoria pra skills existentes e template de exemplo. |
| [`reference.md`](./reference.md) | Referência técnica completa: todos os campos de frontmatter, matriz de controle de invocação, padrões avançados (subagents, hooks, dynamic context), passagem de argumentos e troubleshooting. |

## Como usar

1. Copie `skill-builder.md` pra `.claude/skills/skill-builder/SKILL.md` no seu projeto.
2. Copie `reference.md` pro mesmo diretório (a skill referencia ele pra detalhes técnicos).
3. Invoque com `/skill-builder` quando quiser criar ou auditar uma skill.

## Quando usar cada modo

- **Construir skill nova** → a skill roda uma entrevista guiada antes de escrever qualquer arquivo.
- **Auditar skill existente** → checklist em 4 dimensões (frontmatter, conteúdo, integração, qualidade).

## Fonte

Baseado na documentação oficial: https://code.claude.com/docs/en/skills
