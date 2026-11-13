# Melhorias e análises planejadas

Este documento registra o que pode ser melhorado nos testes e como vamos avaliar se as mudanças funcionam. Não descreve resultados de pessoas: não há respostas, nomes ou códigos de respostas aqui.

Versão do documento: 13/11/2026.

## 1. Situação atual

- Os testes são instrumentos de orientação e **não foram validados cientificamente**.
- Os pesos do cálculo foram escolhidos por critério. A ordem de prioridade é: notas de interesse e habilidade (0 a 5) decidem a ordem; marcações de "gosto", "não gosto" e áreas entram como ajuste pequeno.
- As escolhas em pares somam 0,2 por escolha à dimensão associada. Esse valor também é um critério, sem estudo que o confirme.
- As profissões de destaque (75) e as 20 extras foram selecionadas à mão a partir das listas oficiais CBO e CPP.

## 2. Análises previstas (com dados reais)

As análises só são feitas com respostas de pessoas que aceitaram participar, de forma anonimizada. Veja a seção 5.

| Análise | O que mede | Como fazer | Critério de atenção (proposta inicial) |
|---|---|---|---|
| Consistência interna por dimensão | Se os 5 itens de cada dimensão RIASEC medem o mesmo traço | Alfa de Cronbach por dimensão | Abaixo de 0,70 indica que os itens precisam ser revistos |
| Reteste | Se o perfil se mantém ao longo do tempo | Responder de novo após 2 a 4 semanas e comparar o perfil e as cinco primeiras profissões | Perfil igual em boa parte dos casos; medir a concordância |
| Itens fracos | Perguntas que não separam as pessoas | Ver a distribuição de cada item; itens com quase sempre a mesma nota | Itens com maioria de respostas nos extremos devem ser reescritos |
| Escolhas em pares | Peso real de cada escolha | Estimar o peso por modelo de escolha (por exemplo, Bradley-Terry) | Substituir o valor fixo de 0,2 se os dados indicarem outro valor |
| Sensibilidade do ranking | Quanto a lista de profissões muda com pequenas mudanças nas respostas | Simular alterações de uma nota por vez e medir quantas profissões saem do top 5 | Mudança de uma nota deve mexer no máximo em uma ou duas posições |
| Validade convergente | Se o resultado se parece com instrumentos já validados | Aplicar um instrumento de referência com permissão, e comparar | Correlações positivas e coerentes com a teoria |

## 3. Melhorias propostas

### 3.1 Sem depender de dados (podem ser feitas agora)

1. **Coerência do perfil (hexágono de Holland).** As letras RIASEC estão em um hexágono, e letras vizinhas são mais parecidas. Se as duas primeiras letras não forem vizinhas, mostrar uma nota explicando que o perfil pode ser mais difícil de interpretar.
2. **Aviso de indefinição.** Se a diferença entre a primeira e a segunda dimensão for pequena, dizer que o perfil ainda não está definido, em vez de apresentar a ordem como certa. O limite exato deve ser definido depois da coleta de dados.
3. **Alerta de padrão de resposta.** Se a pessoa usa o mesmo valor na maioria das perguntas, ou marca "Não sei" em muitas delas, o resultado deve avisar que pode não representar bem a pessoa.
4. **Explicação das marcações.** Deixar claro, no próprio resultado, que "gosto" e "não gosto" têm peso pequeno.
5. **Revisão de linguagem.** Medir o nível de leitura dos textos (há índices adaptados ao português) e simplificar os trechos mais difíceis, especialmente nas perguntas para jovens.

### 3.2 Dependem de dados

6. **Pesos e limites.** Revisar os pesos (0,15, 0,10, teto de 2 e 0,2 dos pares) com base na consistência, no reteste e na sensibilidade.
7. **Congruência entre perfil e profissão.** Trocar a média simples por uma medida de semelhança entre o perfil da pessoa e o código RIASEC de cada profissão, como distância ou índice de congruência. Isso é mais coerente com a teoria RIASEC, mas precisa ser comparado com a fórmula atual antes de ser adotado.
8. **Normas.** Com uma amostra grande, comparar a pessoa com outras pessoas da mesma faixa etária, e não só com uma escala fixa de 0 a 5.
9. **Itens reescritos.** Substituir os itens que se mostrarem fracos na análise.

### 3.3 Acessibilidade e experiência

10. **Leitura em voz alta** das perguntas, como opção.
11. **Versão com menos blocos por vez**, para quem prefere pausar com frequência.
12. Manter o progresso salvo no navegador, com aviso antes de qualquer ação que apague respostas (já existe).

## 4. Critérios para aceitar uma mudança

- A mudança precisa ter uma razão registrada neste documento.
- Deve ser testada com os dados disponíveis antes de ser publicada.
- Se a mudança alterar o resultado de quem já fez o teste, o código de respostas da versão anterior deve continuar sendo lido, e o resultado deve indicar que foi recalculado.
- Toda mudança de fórmula ou de pergunta gera uma nova versão do código de respostas.

## 5. Dados, consentimento e privacidade

- Antes de coletar qualquer resposta para análise, é preciso um **termo de consentimento** que explique o uso dos dados, quem tem acesso e por quanto tempo serão guardados.
- Para menores de 18 anos, o consentimento deve vir de um responsável legal.
- O código de respostas contém o **nome e a idade** da pessoa. Antes de qualquer análise, esses campos devem ser removidos, e cada pessoa recebe um identificador aleatório.
- Os dados brutos devem ficar fora do repositório público.
- As análises devem ser feitas sobre o conjunto anonimizado, e os resultados publicados devem ser agregados, sem permitir identificar ninguém.

## 6. Ordem sugerida

1. Revisar o termo de consentimento e o plano de guarda dos dados.
2. Fazer as melhorias da seção 3.1, porque não dependem de dados.
3. Coletar respostas anonimizadas e fazer as análises da seção 2.
4. Ajustar pesos, itens e fórmulas com base nos resultados.
5. Fazer o reteste com um grupo menor.
6. Revisar este documento e publicar uma nova versão dos testes, com a versão do código atualizada.

## 7. Revisão por especialistas

Os documentos técnicos para psicólogos e psiquiatras (adultos e jovens) são mantidos fora do repositório público, por serem confidenciais. As sugestões recebidas deles devem ser registradas aqui, sem identificar quem as enviou, quando houver necessidade de sigilo.
