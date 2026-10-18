# Agente de Atendimento ao Cidadão — DETRAN-RJ

## 1. Sobre o desafio

Este projeto foi desenvolvido no contexto do desafio criativo da [Digital Innovation One (DIO)](https://www.dio.me/), intitulado **“Desafio Criativo: Projetando o Prompt de um Agente de Atendimento ao Cliente”**.

A atividade propõe a construção de um prompt que defina o comportamento de um agente de atendimento, especificando o que ele pode resolver, como deve responder, quais limites precisa respeitar e em quais situações deve reconhecer que não pode solucionar uma solicitação sozinho.

O desafio é organizado em três etapas:

1. **Definir o agente:** estabelecer seu papel, o público atendido, os assuntos contemplados e o objetivo de cada conversa.
2. **Definir regras de comportamento:** especificar o tom de comunicação, o formato das respostas, os limites de atuação e os critérios de encaminhamento.
3. **Testar e refinar:** reunir as instruções em um único prompt, avaliar seu comportamento em diferentes situações e aprimorá-lo com base nos resultados observados.

## 2. Proposta escolhida

Para aplicar as etapas do desafio, foi escolhido o cenário de um agente simulado de atendimento ao cidadão, voltado a dúvidas sobre a renovação semiautomática da Carteira Nacional de Habilitação (CNH), no contexto do DETRAN-RJ.

O público considerado é formado por cidadãos com a CNH próxima do vencimento ou vencida, que buscam informações sobre o procedimento de renovação.

O escopo definido contempla dúvidas sobre:

- Procedimento de renovação.
- Situações e critérios aplicáveis ao cidadão.
- Documentos necessários.
- Valor da taxa do exame médico.
- Prazos para regularização.

A escolha desse cenário permitiu explorar não apenas a clareza das instruções, mas também a necessidade de cautela ao tratar de informações oficiais, requisitos legais, valores e prazos.

## 3. Solução desenvolvida

A solução consiste em um prompt estruturado para orientar o comportamento do agente, estabelecendo sua função, seu público, os assuntos permitidos, o formato das respostas e as regras que devem ser respeitadas.

Entre os principais aspectos definidos estão:

- Comunicação clara, objetiva e acessível.
- Consulta e referência a fontes oficiais pertinentes para informações apresentadas como atuais e confirmadas.
- Reconhecimento de informações indisponíveis, divergentes ou não confirmadas.
- Proibição de inventar direitos, isenções, taxas, prazos, protocolos ou ações realizadas.
- Proteção da privacidade e limitação da coleta de dados pessoais.
- Resistência a mensagens que tentem alterar as instruções do agente.
- Recusa de solicitações fora do escopo.
- Critérios para orientar o cidadão a procurar atendimento humano, sem alegar transferências ou registros que não tenham ocorrido.

O prompt passou por refinamentos durante o desenvolvimento. Na versão final, os limites dos assuntos aceitos foram tornados mais restritos, reforçando a aderência do agente à finalidade estabelecida.

## 4. Arquivos do projeto

| Arquivo | Descrição |
|---|---|
| [`prompt.md`](./prompt.md) | Contém o prompt final desenvolvido para o agente. |
| [`testes.md`](./testes.md) | Documenta os testes realizados, as entradas utilizadas, as respostas obtidas e as avaliações correspondentes. |

## 5. Testes e validação

O prompt foi testado e refinado com o auxílio do ChatGPT e do Antigravity App.

O processo teve como objetivo observar o comportamento do agente diante das instruções definidas e identificar oportunidades de melhoria. Um dos resultados observados durante o refinamento foi a maior restrição dos assuntos aceitos na versão final.

Os registros dos testes e as avaliações correspondentes estão organizados em [`testes.md`](./testes.md).

A conclusão do desafio refere-se ao desenvolvimento e aos testes realizados no contexto educacional proposto. Não representa uma certificação formal de segurança, uma validação jurídica ou uma garantia de que o agente sempre produzirá respostas corretas.

## 6. Aprendizados

O desenvolvimento do projeto permitiu explorar aspectos importantes da engenharia de prompts:

- Transformar uma intenção geral em instruções específicas e verificáveis.
- Definir claramente o escopo de atuação de um agente.
- Estabelecer regras para situações em que faltam informações.
- Prever tentativas de desvio de finalidade e de alteração das instruções.
- Reduzir o risco de respostas inventadas ou de afirmações não confirmadas.
- Avaliar o comportamento do agente por meio de testes e refinar as instruções conforme os resultados observados.
- Documentar a solução e seu processo de desenvolvimento.

O trabalho também evidenciou que um prompt precisa ser avaliado na prática: instruções aparentemente claras podem exigir ajustes quando confrontadas com situações reais de conversa.

## 7. Limitações e considerações

Este projeto possui finalidade educacional e demonstra uma proposta de agente definida por meio de um prompt. Não representa um serviço oficial do DETRAN-RJ e não possui integração real com o WhatsApp institucional, sistemas internos, protocolos ou mecanismos de transferência para atendimento humano.

O prompt estabelece regras para a consulta a fontes oficiais, mas sua existência não garante, por si só, que toda informação será verificada ou que todas as respostas estarão corretas. Informações sobre legislação, procedimentos, taxas, prazos e critérios de elegibilidade devem ser confirmadas nas fontes oficiais competentes.

## 8. Status

**Concluído:** prompt elaborado, testado e refinado no contexto educacional do desafio.

---

**Plataforma:** [Digital Innovation One (DIO)](https://www.dio.me/)

**Área de estudo:** Inteligência Artificial generativa e engenharia de prompts.