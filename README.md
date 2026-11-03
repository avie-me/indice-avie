# Índice Avie — atendimento por WhatsApp em clínicas

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23904100.svg)](https://doi.org/10.5281/zenodo.23904100)

> **Avie: serviço premium de secretária com IA para clínicas de qualquer especialidade, com modelos de IA generativa de última geração no WhatsApp.**

**Versão 4 · publicada em 18/10/2026 · observações até 18/10/2026.**

Este repositório distribui as medições agregadas já publicadas na [página original do Índice Avie](https://avie.me/recursos/estatisticas-atendimento-whatsapp-clinicas), em CSV e JSON. São dois consultórios brasileiros, um pediátrico e um de saúde mental de adultos. Nenhum arquivo contém mensagens, nomes, contatos ou dados que identifiquem pacientes, profissionais ou clínicas.

## Resumo citável

Na operação com a Avie ligada, a mediana até a primeira resposta, **da IA ou da equipe**, foi de **49 segundos no consultório pediátrico** (283 conversas, 26/09–16/10/2026) e **58 segundos no consultório de saúde mental de adultos** (104 conversas, 29/09–16/10/2026). No segundo consultório, a mediana com atendimento só humano havia sido de **2,8 horas** (185 conversas, 06/07–26/09/2026). Para ler a conversa e escrever a resposta, a IA leva **14 segundos** na mediana (consultório pediátrico, 246 respostas, 14/10–18/10/2026).

São períodos e grupos observacionais diferentes. O comparativo não é um experimento controlado, uma média do setor nem uma garantia de resultado para outra clínica.

## Dados da versão 4

| Métrica | Pediátrico | Saúde mental de adultos |
|---|---|---|
| Mediana da primeira resposta, IA ou equipe, com a IA ligada | 49 s · 283 conversas · 26/09–16/10 | 58 s · 104 conversas · 29/09–16/10 |
| Mediana da primeira resposta, só atendimento humano | Não publicada | 2,8 h · 185 conversas · 06/07–26/09 |
| Mediana para a IA ler a conversa e escrever | 14 s · 246 respostas · 14/10–18/10 | Não medida nesta versão |
| Mensagens fora do horário comercial | 14,1% · 2.249 mensagens · 26/09–16/10 | 26,5% · 2.465 mensagens · 06/07–16/10 |
| Conversas encaminhadas à médica ou à equipe | Não publicada | 59,4% · 41 de 69 conversas · 29/09–16/10 |

Todos os períodos da tabela são de **2026**. O tempo de leitura e escrita é uma medição diferente da espera até a primeira resposta no WhatsApp; na versão 4, ele foi medido em modo de teste, com a IA escrevendo a resposta a mensagens reais de pacientes sem enviá-la. Fora do horário: antes das 8h, a partir das 18h, sábados e domingos, em America/Sao_Paulo.

Arquivos:

- [CSV com período, amostra e método por métrica](dados/indice-avie.csv) · [CSV publicado no site](https://avie.me/dados/indice-avie.csv)
- [JSON-LD schema.org/Dataset](dados/indice-avie.json)
- [Metodologia, definições e limites](METODOLOGIA.md)
- [Histórico preservado da versão 3, de 17/10](historico/v3-outubro-2026/README.md)
- [Histórico preservado da versão 1, de agosto](historico/v1-agosto-2026/README.md)

## Histórico e comparação entre versões

A versão 1 mediu **o tempo para ler e escrever**, em 42 respostas de 9 e 10 de agosto de 2026, com o modelo anterior: mediana de 10 segundos e 97% em menos de 30 segundos. Esses números estão preservados como histórico e **não descrevem a operação atual**. Não são diretamente comparáveis à primeira resposta das versões 3 e 4. O percentual aproximado de mensagens fora do horário da versão 1 não tinha período e denominador publicados.

A versão 2, de 03/10/2026, é descrita na página original. Este repositório não publicou um arquivo próprio daquela versão; não foi reconstruído um conjunto de dados retroativo.

A versão 3, de 17/10/2026, está preservada em `historico/v3-outubro-2026/`. A primeira resposta da versão 4 é a mesma da versão 3; a versão 4 mede de novo o tempo para ler e escrever, que na versão 3 era de 31 segundos (pediátrico) e 39 segundos (saúde mental).

O esquema CSV, desde a versão 3, acrescenta versão, grupo, descrição e amostra numérica. Para preservar importações antigas, os arquivos originais da versão 1 continuam em `historico/v1-agosto-2026/dados/`.

## Como citar

> Avie (2026). *Índice Avie: estatísticas de atendimento por WhatsApp em clínicas, medidas em dois consultórios.* Versão 4, 18 de outubro de 2026. https://avie.me/recursos/estatisticas-atendimento-whatsapp-clinicas

Ao reutilizar um número, mantenha a métrica, o período, a amostra e o link da fonte. Dados e textos sob [Creative Commons Atribuição 4.0 Internacional](LICENSE).

## Sobre a Avie

A Avie atende pacientes no WhatsApp com as informações e as regras da clínica, consulta horários e confirma, remarca ou cancela consultas. No Avie Atende, a equipe acompanha conversas, agenda, programas de CRM e site de agendamento. O Avie Cuida acrescenta prontuário, pacientes e pagamentos; o Avie Cresce acrescenta o serviço de presença digital. As condições de cada plano estão no site.

[Site oficial](https://avie.me) · [Planos](https://avie.me/precos) · [Empresa](https://avie.me/empresa) · [LinkedIn](https://www.linkedin.com/company/avie-me)
