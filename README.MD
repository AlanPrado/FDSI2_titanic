# Resumo

Essa visualização apresenta dados sobre o desastre do navio Titanic que
naufragou em 15 de abril de 2011.

A visualização contempla dados de idade, cidade de embarque, e condições
economicas sobre todos os passageiros presentes no desastre com exceção da
tripulação.

Foi identificado uma correlação entre a probabilidade de sobreviver e
o preço do bilhete, o gênero e a idade. Prioridade para mulheres e crianças
fazia parte do protocolo de evacuação da epoca. Entretanto, o preço pago pelo
bilhete não fazia parte do protocolo. Esta ação acabou favorecendo os passageiros
de Cherbourg uma vez que pagaram preços acima da média.

# Links

* Versão [inicial](https://public.tableau.com/shared/RKYF4WWJG?:display_count=yes)
* Versão [final](https://public.tableau.com/shared/YPP2DFYFF?:display_count=yes)

# Design

## Codificação e Cores

A maior parte dos gráficos utiliza categorias diferentes, e para realçar as
Informações foram utilizados paletas para dados qualitativos.

No gráfico de timeline do naufragio foi utilizado paletas para dados qualitativos
para destacar os principais eventos.

No grafico das principais familias afetas pelo naufragio foi utilizado uma
paleta sequencial para realçar a diferença de quantidade de mortes.

No grafico que mostra o itinerário do Titanic foi utilizado uma paleta
divergente para mostrar a transição de uma cidade para outra.

Em alguns momentos foram utilizados o tamanho para realçar a proporção entre os
dados comparados.

Foram utilizados formas para destacar elementos. A principal vantagem de
utilizar forma foi permitir a visualização de elementos sobrepostos.

## Tipos de gráficos

Para visualizar distribuições foram utilizados gráficos de caixa, histograma,
barras.

Para visualizar tendência foram utilizados gráficos área e linha utilizando
linhas de tendência quando necessário.

Para verificar a relação entre os dados foram utilzados gráficos de pizza e
barra empilhados. A escolha entre um e outro dependendia do que gostaria de se
comparar.

Gráficos com duas medidas que seriam comparados com o todo, utilizavam
o gráfico de pizza.

O gráfico de barra empilhado foi utilizado para comparar
proporções de dados de tipos diferentes com mais de três medidas.

Também, foi utilizado um gráfico de bullet com o intuito de comparar medidas
em diferentes agrupamentos.

O gráfico de mapa contou com um elemento rota para mostrar o itinerário do navio.

## Estrutura da História

Os dados são apresentados progressivamente e a cada etapa é acrescentado um novo
dado ou um novo relacionamento.

A proposta foi criar uma foto antes do acidente e uma após o acidente para
entender quem foi priorizado no resgate do com relação às caracteristicas fisicas
e economicas.

A estrutura da apresentação foi divida da seguinte forma:

Texto - Introdução
Gráfico - Relação do preço por classe
Gráfico - Relação de idade por sexo
Gráfico - Relação de preco por cidade
Gráfico - Relação de familias por cidade de embarque
Texto - Acidente
Gráfico - Relação de sobreviventes por idade e sexo
Gráfico - Relação de sobreviventes por preço do bilhete
Gráfico - Relação de sobreviventes por classe
Gráfico - Relação de sobreviventes por familia
Texto - Conclusão

## Manipulação de Dados

Foi necessário criar algumas colunas de campo calculado, como por exemplo a
coluna de preço por pessoa, onde foi divido o preço pago no bilhete pelo número
de pessoas que utilizaram aquele bilhete.

Foi necessário, também, configurar os dados geográficos de latitute e longitude.

Finalmente, varios aliases foram cadastrados.

# Comentários

## [Forum](https://discussions.udacity.com/t/coleta-de-feedback-projeto-final-tableau-titanic-alanprado/501511/4)

- Na parte “A inauguraçãofoi um sucesso…” gostei bastante das visualizações mas acredito que o boxplot seja muito avançado para um público sem conhecimentos estatísticos. Creio que a visualização seria bem mais efetiva se utilizasse outra ferramenta;
O objetivo era destacar os outliers, e por isso a escolha foi mantida.

- Na parte " A juventude se destaca…" não gostei muito do gráfico de pizza para a distribuição de homens e mulheres, embora eu ache que seja soó minha perseguição padrão contra gráficos de pizza;
Manter o gráfico de pizza tornava a visualização consistente com a versão do mesmo gráfico para sobreviventes.
Entretanto, caso fosse alterado a segunda visualização ficaria muito poluida.

- Na parte “A partida”: gostei bastante, embora preferiria modificar o # por n ou quantidade;
Os textos foram alterados.

- Na parte “O preço da sobrevivência” achei a 2a visualização bonita mas tive dificuldade de entender o que as linhas significavam.
Foi acrecentado uma legenda e textos explicativos.

## Pessoas que eu conversei pessoalmente

- Segundo gráfico da relação de sobreviventes por classe confusa. Tamanho atrapalhou a leitura.
Foi removido a codificação de tamanho e feito os ajustes da sessão anterior.
Além disso foi acrescentado uma ferramenta de destaque para mostrar a relação
entre os gráficos.
- A sessão de naufrágio ficou com muito texto e não chama a atenção.
Foi alterado para um gráfico de timeline.
- Gráfico de familias e preço por classe ficou com muitos dados.
Foi criado uma sessão separada para mostrar a relação das familias afetadas pelo
desastre e adicionado gráficos para explicar a relação dos sobreviventes por
classe.

## Revisor

- Textos nos tooltips precisam ser alterados para que fiquem mais claros para o leitor.
Foram revisados todos os tooltips.
- Inclua um título na história que demonstre para o leitor o que será mostrado
Foi adicionado um titulo na historia.

# Recursos

## Informações Históricas

* https://pt.wikipedia.org/wiki/RMS_Titanic
* https://www.rina.org.uk/lifeboats.html

## Dados
* http://biostat.mc.vanderbilt.edu/wiki/pub/Main/DataSets/titanic.html
* http://biostat.mc.vanderbilt.edu/wiki/pub/Main/DataSets/Ctitanic3.html#pclass
* http://biostat.mc.vanderbilt.edu/wiki/Main/DataSets

## Visualização de dados
* http://kb.tableau.com/articles/howto/creating-a-gantt-chart-with-shapes-for-small-time-increments
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/annotations_marklabels_move.html
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/bkimages.html
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/buildexamples_gantt.html
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/buildexamples_scatter.html
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/custom_geocoding.html
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/filtering_global.html
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/help.htm#maps_geographicroles.html
* http://onlinehelp.tableau.com/current/pro/desktop/en-us/viewparts_marks_marktypes_gantt.html
* http://onlinehelp.tableau.com/current/pro/desktop/pt-br/calculations_percentages_options.html
* http://onlinehelp.tableau.com/current/pro/desktop/pt-br/formatting_specific_titlecaption.html#Format_tooltips
* https://community.tableau.com/docs/DOC-1353
* https://community.tableau.com/thread/122001
* https://community.tableau.com/thread/135387
* https://community.tableau.com/thread/136984
* https://community.tableau.com/thread/138308
* https://community.tableau.com/thread/145015
* https://community.tableau.com/thread/147392
* https://community.tableau.com/thread/148797
* https://community.tableau.com/thread/204534
* https://community.tableau.com/thread/223243
* https://community.tableau.com/thread/226139
* https://onlinehelp.tableau.com/current/pro/desktop/en-us/qs_bullet_graphs.html
* https://onlinehelp.tableau.com/current/pro/desktop/en-us/maps_howto_origin_destination.html
* https://onlinehelp.tableau.com/current/pro/desktop/pt-br/buildexamples_maps.html
* https://onlinehelp.tableau.com/current/server/en-us/csvguidelines.htms

## Copyright e Licença
Code and documentation copyright 2017-2017 Code released under the [MIT License](https://github.com/AlanPrado/FDSI2_titanic/blob/master/LICENSE)

## Autor

### Autor Original e lider de desenvolvimento

- Alan Thiago do Prado (aprado.cnsp@gmail.com)
