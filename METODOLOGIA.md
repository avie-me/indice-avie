# Metodologia — Índice Avie v4

Versão publicada em **18/10/2026**, com observações até **18/10/2026**. Fonte: [seção de método e dados publicados pela Avie](https://avie.me/recursos/estatisticas-atendimento-whatsapp-clinicas). Este repositório reproduz agregados públicos; não disponibiliza os registros individuais.

## Universo e exclusões

Dois consultórios brasileiros: um pediátrico e um de saúde mental de adultos. Foram usados horários de recebimento e envio, origem do envio (IA, equipe ou automação), duração das chamadas ao modelo e registros de encaminhamento. Foram excluídos números de teste, da equipe e bloqueados, conversas marcadas como não paciente, figurinhas e reações.

Os dados não identificam paciente, profissional ou clínica. As amostras e as janelas diferem entre métricas; elas estão declaradas em cada linha do CSV e em cada descrição do JSON. Não se deve somar os denominadores das métricas.

## Definições

- **Conversa:** começa quando chega uma mensagem depois de mais de 6 horas sem nenhuma troca naquele chat.
- **Primeira resposta:** primeira mensagem enviada que não é lembrete nem automação, até 48 horas depois do início da conversa. Na fase com IA ligada, a medição principal inclui a primeira resposta da IA **ou da equipe**; não é um número exclusivo da IA.
- **Leitura e escrita da IA:** do início da leitura da conversa até o texto final da resposta. Não corresponde ao tempo total de espera do paciente. Na versão 4, a IA escreveu em modo de teste, sem enviar, a resposta a mensagens reais de pacientes do consultório pediátrico, com o mesmo modelo e a mesma configuração do atendimento; o tempo soma a leitura, as consultas à agenda e ao cadastro e a escrita. As respostas no WhatsApp incluem o ritmo de digitação configurado pela clínica.
- **Fora do horário comercial:** antes das 8h, a partir das 18h, sábados e domingos, no fuso America/Sao_Paulo. Esta é a definição usada no estudo, não o horário individual de funcionamento de toda clínica.
- **Encaminhamento:** conversa passada à médica ou à equipe. Em saúde mental de adultos, 41 de 69 conversas tiveram encaminhamento (59,4%, arredondado a uma casa decimal), com 85 encaminhamentos no total. Conversas e encaminhamentos são unidades diferentes.

## Períodos e amostras

| Medição | Pediátrico | Saúde mental de adultos |
|---|---|---|
| Primeira resposta com a IA ligada | 26/09–16/10/2026 · 283 conversas | 29/09–16/10/2026 · 104 conversas |
| Primeira resposta só humana, antes da IA | Não publicada | 06/07–26/09/2026 · 185 conversas |
| Leitura e escrita da IA | 14/10–18/10/2026 · 246 respostas | Não medida nesta versão |
| Horário das mensagens | 26/09–16/10/2026 · 2.249 mensagens | 06/07–16/10/2026 · 2.465 mensagens |
| Conversas com encaminhamento | Não publicada | 29/09–16/10/2026 · 69 conversas |

A medição de leitura e escrita desta versão usa o modelo gpt-6-luna, em uso desde 22/09/2026, e é posterior ao período da primeira resposta. A próxima versão mede de novo a primeira resposta.

## Limites da interpretação

A fase anterior à IA vem do histórico do WhatsApp sincronizado quando o consultório conectou a Avie. Esse histórico é parcial nos primeiros meses, e só entram conversas respondidas em até 48 horas. A fase com IA tem cerca de três semanas; as conversas do último dia tiveram menos de 48 horas de observação.

Não houve experimento controlado nem seleção aleatória de consultórios. Os períodos diferem e os números não demonstram causalidade isolada. Não são média de mercado, estimativa de todos os consultórios, garantia de resposta ou promessa de conversão, redução de faltas ou receita.

Os motivos de encaminhamento publicados na página original foram agrupados a partir das notas de encaminhamento, sem trechos de mensagens de pacientes. Grupos com menos de 5 casos não aparecem separados. Esse detalhamento e referências externas de conversão não integram os oito agregados distribuídos aqui.

## Versionamento e licença

A versão 1 permanece íntegra em `historico/v1-agosto-2026/`, incluindo suas limitações originais. A versão 3 permanece íntegra em `historico/v3-outubro-2026/`. A versão 2 é citada na página original, mas não teve arquivo publicado neste repositório. A versão 3 amplia o período e distingue primeira resposta de leitura/escrita. A versão 4 mantém a primeira resposta da versão 3 e mede de novo a leitura e escrita. Não compare os 10 segundos da versão 1 com os 49 ou 58 segundos da versão 3 como se fossem a mesma métrica.

Na próxima atualização, versão, data, períodos, método e arquivos devem mudar juntos. Licença: [CC BY 4.0](LICENSE), com atribuição à Avie e link para a fonte original.
