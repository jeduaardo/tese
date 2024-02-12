#########################################################
#                Problemas - Benchmark                  #
#   Experimentos para validação em problemas benchmark  #
#           José Eduardo H. da Silva - 12/02/2024       #
#########################################################

Dados dos problemas benchmark da categoria experimentais de Pratapa et al. (https://www.nature.com/articles/s41592-019-0690-6).

Diretórios: prefixo h indica dataset de Humanos e prefixo m de camundongos. 
hESC
hHep
mDC
mESC
mHSC-E
mHSC-GM
mHSC-L

Subdiretórios:
500nTF
500TF
1000nTF
1000TF


Arquivos em cada diretório:
- ExpressionData.csv: arquivo de dados de expressão gênica contendo todos os genes. Cada linha é iniciada pelo nome do gene (espécie) e os demais valores são as concentrações. As colunas são as células/tempo de simulação.
- PseudoTime.csv: arquivo de pseudotime. A primeira coluna é o nome da célula e a segunda coluna é o valor de tempo.
- PROBLEMA-REFERENCIA-network.csv: rede ground-truth. Primeira coluna é o regulador e a segunda coluna é o alvo. PROBLEMA é o nome do problema e REFERENCIA é a rede de referência. Essas redes de referência contemplam TODOS os genes, independentemente da configuração selecionada.- ExpressionData.csv: arquivo de dados de expressão gênica considerando todos os genes disponíveis.
- GeneOrdering.csv: arquivo de ordenação de importância de cada gene em termos de regulação. Genes com maior p-valor são ditos diferencialmente expressos.
- ESPECIE-tfs.csv: arquivo que contém os fatores de transcrição (TFs) a depender da espécie (h - Humanos e m - Camundongos).

Arquivos em cada subdiretório:

- PROBLEMA_CONFIG_REFERENCIA-network.csv: São as redes de referência, considerando o PROBLEMA, na configuração CONFIG, em relação à rede de referência REFERENCIA. Os significados são os mesmos da rede de referência presente no diretório principal.
- PROBLEMA_CONFIG_REFERENCIA-ExpressionData.csv: arquivos de expressão gênica contendo somente as espécies da configuração CONFIG do problema PROBLEMA. A REFERENCIA não faz diferença neste caso, tendo em vista que os genes são os mesmos para cada configuração.

CONFIGS:
500nTF - 500 genes sem considerar fatores de transcrição
500TF - 500 genes considerando fatores de transcrição
1000nTF - 1000 genes sem considerar fatores de transcrição
1000TF - 1000 genes considerando fatores de transcrição

Detalhes sobre esses problemas e os papers de referência estão apresentados na tese e os dados estão publicamente disponíveis no repositório de Pratapa et al. (https://zenodo.org/records/3701939).

NOTA: Os arquivos de expressão gênica completos dos problemas hESC e mESC foram removidos devido à limitação de tamanho de arquivos (máximo de 100MB). Estes arquivos estão disponíveis no repositório de Pratapa et al.

NOTA2: Para o problema mESC, o nome dos genes apresentados no arquivo de expressão gênica original não estão de acordo com o formato utilizado pelo próprio Pratapa para a geração dos conjuntos de dados. Por esse motivo, o diretório do mESC contém arquivos com _Upper, que significa que todos os genes estão em caixa alta. Ver Notas Importantes.txt para maiores informações.