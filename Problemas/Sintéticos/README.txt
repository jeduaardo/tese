#########################################################
#                Problemas - Benchmark                  #
#   Experimentos para validação em problemas benchmark  #
#           José Eduardo H. da Silva - 12/02/2024       #
#########################################################

Dados dos problemas benchmark da categoria sintético de Pratapa et al. (https://www.nature.com/articles/s41592-019-0690-6).

Diretórios: 
dyn-BF
dyn-BFC
dyn-CY
dyn-LI
dyn-LL
dyn-TF

Significados:
BF - Bifurcating
BFC - Bifurcating Converging
CY - Cycle
LI - Linear
LL - Linear Long
TF - Trifurcating

Subdiretórios: Em cada um dos diretórios são apresentados 50 subdiretórios que seguem a nomenclatura seguinte.
PROBLEMA-NCELULAS-DATASET

Onde: PROBLEMA é o nome do problema, NCELULAS é o número de células (100, 200, 500, 2000 e 5000), DATASET é o identificador (inteiro) do dataset.

Arquivos em cada subdiretório:
- ExpressionData.csv: arquivo de dados de expressão gênica. Cada linha é iniciada pelo nome do gene (espécie) e os demais valores são as concentrações. As colunas são as células/tempo de simulação. NGENES é a quantidade de genes do problema e problema é o identificador da rede.
- PseudoTime.csv: arquivo de pseudotime. A primeira coluna é o nome da célula e a segunda coluna é o valor de tempo.
- refNetwork.csv: rede ground-truth. Primeira coluna é o regulador, segunda coluna é o alvo e a terceira coluna é o tipo de regulação (+ = ativação / - = inibição).

Detalhes sobre esses problemas e os papers de referência estão apresentados na tese e os dados estão publicamente disponíveis no repositório de Pratapa et al. (https://zenodo.org/records/3701939).