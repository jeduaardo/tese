#########################################
#          Problemas - DREAM4           #
#   Experimentos para organismos reais  #
# José Eduardo H. da Silva - 12/02/2024 #
#########################################

Dados dos problemas da competição DREAM4 (https://www.synapse.org/#!Synapse:syn3049712/wiki/74630).

Diretórios: os valores 10 e 100 indicam a quantidade de genes e o último valor identifica o dataset (1 a 5).
DREAM4_10_1
DREAM4_10_2
DREAM4_10_3
DREAM4_10_4
DREAM4_10_5
DREAM4_100_1
DREAM4_100_2
DREAM4_100_3
DREAM4_100_4
DREAM4_100_5

Arquivos em cada diretório:
- ExpressionData_DREAM4_NGENES_PROBLEMA.csv: arquivo de dados de expressão gênica. Cada linha é iniciada pelo nome do gene (espécie) e os demais valores são as concentrações. As colunas são as células/tempo de simulação. NGENES é a quantidade de genes do problema e problema é o identificador da rede.
- PseudoTime.csv: arquivo de pseudotime. A primeira coluna é o nome da célula e a segunda coluna é o valor de tempo.
- refNetwork.csv: rede ground-truth. Primeira coluna é o regulador, segunda coluna é o alvo e a terceira coluna é o tipo de regulação (+ = ativação / - = inibição).
- DREAM4_GoldStandard_InSilico_SizeNGENES_PROBLEMA.tsv: arquivo original da rede ground-truth disponibilizado pela competição.
- insilico_sizeNGENES_PROBLEMA.tsv: arquivo original de expressão gênica disponibilizado pela competição.

Detalhes sobre esse modelo e os papers de referência estão apresentados na tese e os dados estão publicamente disponíveis no site da competição.