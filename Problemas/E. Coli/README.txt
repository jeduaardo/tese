##########################################
#          Problemas - E. Coli           #
#   Experimentos para modelos booleanos  #
# José Eduardo H. da Silva - 12/02/2024  #
##########################################

Dados dos problemas utilizados para comparação entre modelos booleanos e baseados em técnicas de computação evolucionista. Os dados também são derivados da competição DREAM4.

Diretórios: os valores indicam a quantidade de genes envolvidos.
16
32
64

Arquivos em cada diretório:
- Ecoli-PROBLEMA_dream4_timeseries.tsv: arquivos originais de expressão gênica. O PROBLEMA é o identificador da rede.
- Ecoli-PROBLEMA_goldstandard.tsv: arquivos originais da rede ground-truth. O PROBLEMA é o identificador da rede.
- Ecoli-PROBLEMA-NGENES-ExpressionData.csv: arquivo de dados de expressão gênica. Cada linha é iniciada pelo nome do gene (espécie) e os demais valores são as concentrações. As colunas são as células/tempo de simulação. NGENES é a quantidade de genes do problema e PROBLEMA é o identificador da rede.
- Ecoli-PROBLEMA-NGENES-PseudoTime.csv: arquivo de pseudotime. A primeira coluna é o nome da célula e a segunda coluna é o valor de tempo. NGENES é a quantidade de genes do problema e PROBLEMA é o identificador da rede.
- Ecoli-PROBLEMA-NGENES-refNetwork.csv: rede ground-truth. Primeira coluna é o regulador, segunda coluna é o alvo e a terceira coluna é o tipo de regulação (+ = ativação / - = inibição).


Detalhes sobre esse modelo e os papers de referência estão apresentados na tese.