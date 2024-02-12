#########################################################
#                Problemas - Benchmark                  #
#   Experimentos para validação em problemas benchmark  #
#           José Eduardo H. da Silva - 12/02/2024       #
#########################################################

Dados dos problemas benchmark da categoria curated de Pratapa et al. (https://www.nature.com/articles/s41592-019-0690-6).

Diretórios: 
GSD
HSC
mCAD
VSC

Subdiretórios: Em cada um dos diretórios são apresentados 30 subdiretórios que seguem a nomenclatura seguinte.
PROBLEMA-2000-DATASET-DROPOUT

Onde: PROBLEMA é o nome do problema, 2000 é o número de células, DATASET é o identificador (inteiro) do dataset e DROPOUT é a taxa de dropout (50% ou 70%). Os subdiretórios sem o identificador de dropout indicam 0% de dropout.

Arquivos em cada subdiretório:
- ExpressionData.csv: arquivo de dados de expressão gênica. Cada linha é iniciada pelo nome do gene (espécie) e os demais valores são as concentrações. As colunas são as células/tempo de simulação. NGENES é a quantidade de genes do problema e problema é o identificador da rede.
- PseudoTime.csv: arquivo de pseudotime. A primeira coluna é o nome da célula e a segunda coluna é o valor de tempo.
- refNetwork.csv: rede ground-truth. Primeira coluna é o regulador, segunda coluna é o alvo e a terceira coluna é o tipo de regulação (+ = ativação / - = inibição).

Detalhes sobre esses problemas e os papers de referência estão apresentados na tese e os dados estão publicamente disponíveis no repositório de Pratapa et al. (https://zenodo.org/records/3701939).