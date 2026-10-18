# Metodologia

Texto baseado na seção de método da página pública https://avie.me/recursos/estatisticas-atendimento-whatsapp-clinicas (atualizada em 19/08/2026).

- **O que medimos:** os registros do próprio sistema da Avie na operação de uma clínica real (consultório médico que atende famílias pelo WhatsApp). Nenhum dado identifica paciente.
- **O que os números são:** medições daquela operação, no período indicado em cada um. Não são média de mercado nem promessa de resultado.
- **O que os números não são:** amostra estatística do setor. Uma clínica, um período. Publicamos porque preferimos um número real e auditável a uma estatística de terceiros sem fonte.
- **Técnica:** logs de geração de resposta e horário de recebimento das mensagens.

## Detalhe por métrica

| Métrica | Como foi medida |
|---|---|
| 97% das respostas em menos de 30 s | 42 respostas medidas em produção com o modelo GPT-5.6 Luna, 9 e 10 de agosto de 2026. |
| Mediana de 10 s | Mediana das mesmas 42 respostas. |
| ~20% das mensagens fora do expediente | Distribuição por horário das mensagens recebidas no atendimento real da mesma clínica. |

## Como interpretar o tempo de resposta

É o tempo que a IA leva para **ler a conversa e escrever a resposta**. A entrega no WhatsApp segue um ritmo de digitação humano, configurável pela clínica, e mensagens sensíveis podem aguardar revisão da equipe — por desenho, não por lentidão.

## Referência externa (não faz parte do conjunto de dados)

A página original também cita o estudo *Lead Response Management* (Velocify / ICE Mortgage Technology): +391% de conversão quando o primeiro contato acontece em até um minuto. É dado de terceiro, não de clínicas, e por isso não entra nos arquivos de `dados/`.

## Atualizações

Quando houver medição nova, os arquivos são atualizados e a data muda junto.
