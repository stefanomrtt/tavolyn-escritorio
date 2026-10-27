# Escritório da Tavolyn

Agentes de IA que trabalham como funcionários da Tavolyn. Vocês conversam com o **gerente**, que delega cada tarefa ao setor certo. No Habblaud (https://habblaud.localhost), cada agente aparece como um personagem trabalhando.

## Como usar

1. No app do Claude, abra uma sessão nova na pasta `tavolyn-escritorio`. Ela já começa como o gerente.
2. Peça em português, como pediria a um gerente de verdade. Exemplos:
   - "Revise o fechamento de caixa e me diga se tem algum risco."
   - "Escreva um manual de abertura de caixa para a Pizzaria Italia."
   - "Prepare uma proposta comercial para uma hamburgueria com delivery."
3. Acompanhe no Habblaud e aprove por lá o que os agentes pedirem.

No terminal, o mesmo escritório abre com `claude` dentro desta pasta.

## Equipe

| Agente | Setor | IA | Intensidade |
|---|---|---|---|
| gerente | Gerência | Opus | média |
| arquiteto | Desenvolvimento | Opus | alta |
| programador | Desenvolvimento | Sonnet | média |
| testador | Desenvolvimento | Haiku | baixa |
| devops | Infraestrutura | Sonnet | média |
| suporte | Suporte | Haiku | baixa |
| comercial | Comercial | Sonnet | média |
| financeiro | Financeiro | Haiku | baixa |

Cada agente é um arquivo em `.claude/agents/`. Para mudar a função, o modelo (`model`) ou a intensidade (`effort`) de alguém, edite o arquivo dele. Para contratar alguém novo, crie um arquivo no mesmo formato e acrescente o agente na tabela do `gerente.md`.

## Pastas

| Pasta | Conteúdo |
|---|---|
| `empresa/` | Memória da empresa: visão geral, clientes, decisões |
| `tarefas/quadro.md` | O que está em andamento, pendente e concluído |
| `setores/` | O que cada setor produz |
| `.claude/agents/` | A equipe |
| `.claude/agent-memory/` | O que cada agente aprendeu trabalhando |

Pode abrir esta pasta no **Obsidian** para ler e editar a memória da empresa com mais conforto (opcional).

## Segurança

Os agentes não mexem em produção, não enviam mensagens a clientes e não gastam dinheiro sem um sócio aprovar. Não guarde senhas nem chaves nesta pasta: ela vai para o GitHub.
