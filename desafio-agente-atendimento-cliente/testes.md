# Registro operacional de testes do agente

## Finalidade

Este arquivo é o registro operacional das rodadas de teste. Use-o para preservar os dados de cada execução e, principalmente, as entradas e respostas literais, sem reconstrução de memória.

O arquivo [testes-registro.md](./testes-registro.md) é o histórico consolidado: reúne análises técnicas, sínteses de rodadas antigas, decisões de refinamento e pendências. Quando uma rodada for concluída, mantenha aqui o registro da execução e atualize o histórico consolidado se houver novos resultados, conclusões ou decisões.

## Regras de preenchimento

- Copiar a entrada enviada e a resposta recebida exatamente como ocorreram, preservando o texto original.
- Não reescrever uma resposta para torná-la mais clara nem completar trechos ausentes.
- Se a transcrição literal não estiver disponível, registrar **“transcrição literal indisponível”** e descrever o conteúdo como resumo, sem apresentá-lo como transcrição.
- Diferenciar a data do teste da data em que o registro foi escrito.
- Registrar a versão do prompt e o hash/commit apenas quando confirmados. Não atribuir automaticamente o prompt atual a rodadas anteriores.
- Descrever a configuração real: instrução de sistema, prompt fornecido como mensagem ou prompt usado apenas como referência.
- Anotar as ferramentas habilitadas, especialmente navegação web e integrações externas.
- Avaliar a resposta somente depois de preservar a saída original.
- A avaliação é técnica e educacional; não equivale a certificação de segurança nem prova que o agente está pronto para uso real.
- Não registrar dados pessoais reais de cidadãos. Use cenários fictícios ou anonimizados.

---

## Modelo para cada rodada

Copie a estrutura abaixo para cada rodada e preencha os campos disponíveis. Campos desconhecidos devem ser marcados como **não confirmado** ou **não disponível**, e não adivinhados.

### Rodada [identificação]

- **Identificação:** (ex.: ChatGPT anterior, Antigravity 1, Antigravity 2, ChatGPT atual)
- **Data do teste:** (data real, se conhecida)
- **Data do registro:**
- **Ferramenta:** (ex.: ChatGPT ou Antigravity App; versão/modelo se conhecida)
- **Prompt:** (versão, data e hash/commit, se disponíveis)
- **Configuração:** (instrução de sistema / prompt fornecido como mensagem / usado apenas como referência / outra configuração)
- **Ferramentas disponíveis:** (ex.: navegação web, conectores, ações externas; registrar o que se sabe)
- **Objetivo da rodada:**
- **Evidência da execução:** (link ou referência à conversa original, captura ou outro registro preservado)

#### Cenário [ID]

**Entrada exata enviada ao agente**

> Cole aqui a mensagem literal enviada.

**Resposta exata produzida pelo agente**

> Cole aqui a resposta literal recebida. Se for extensa, mantenha o texto integral abaixo, sem paráfrase.

**Avaliação**

- **Resultado:** adequado / falha / ressalva / inconclusivo
- **Critério avaliado:**
- **Evidências/fontes:** (URLs oficiais, data da consulta, referência da conversa ou indicação de que não houve verificação)
- **Justificativa:** (explique qual comportamento observado atende ou viola o critério; separe fatos de interpretação)
- **Pendências:** (o que ainda precisa ser verificado)
- **Ação corretiva proposta:** (se aplicável; não significa que o prompt já foi alterado)

Repita a seção **Cenário [ID]** para cada entrada enviada na rodada.

#### Fechamento da rodada

- **Resumo dos resultados:**
- **Falhas recorrentes ou novas:**
- **Melhorias propostas:**
- **Alterações efetivamente feitas no prompt:** (arquivo/trecho e commit, somente após confirmar)
- **Reteste necessário:**
- **Conclusão:** aprovada para o critério testado / não aprovada / inconclusiva
- **Responsável pela avaliação e data:**

---

## Rodadas históricas sem transcrição literal

Para rodadas anteriores cujas saídas integrais não foram preservadas, registre apenas os metadados confirmados e uma síntese claramente identificada como tal. Não invente datas, versões do prompt, entradas ou respostas. Consulte [testes-registro.md](./testes-registro.md) para o estado consolidado dos registros históricos e das pendências de recuperação.
