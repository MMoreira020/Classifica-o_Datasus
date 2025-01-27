Análise de Dados de Óbitos com Modelos de Classificação

Este projeto utiliza dados do Datasus para analisar óbitos por capítulos da CID-10 no período de 2015 a 2020 e também Nasciemntos no mesmo período. Aplicamos técnicas de classificação utilizando modelos como Random Forest e Naive Bayes para categorizar os anos com diferentes níveis de óbitos e identificar padrões significativos nos dados.

Sumário

    1. Descrição do Projeto

    2. Estrutura dos Dados

    3. Pré-Processamento

    4. Modelos Utilizados

    5. Visualizações e Resultados

    6. Como Executar


1. Descrição do Projeto:

Este projeto tem como objetivo explorar dados sobre óbitos por capítulos da CID-10 no Brasil, realizando as seguintes etapas:

    1.1 Carregamento e limpeza dos dados: Arquivos CSV contendo informações de óbitos por município e ano.
    1.2 Transformação dos dados: Geração de uma coluna de categorias baseada no total de óbitos.
    1.3 Aplicação de algoritmos de classificação: Random Forest e Naive Bayes.
    1.4 Otimização e validação: GridSearchCV para otimizar hiperparâmetros e validação cruzada para avaliar o desempenho.

2. Estrutura dos Dados:

Os dados utilizados foram extraídos do Datasus e possuem os seguintes campos principais:

    2.1 Colunas: Capítulos da CID-10 representando causas de óbito.
    2.2 Linhas: Anos 2015 a 2020.
    2.3 Valores: Número de óbitos por causa.

    Adicionalmente, os capítulos da CID-10 foram mapeados para suas descrições para facilitar a compreensão.

3. Pré-Processamento:

As principais etapas de pré-processamento incluem:

    3.1 Renomeação das colunas: Mapear os capítulos da CID-10 para suas respectivas descrições.
    3.2 Transposição do DataFrame: Facilitar a análise e manipulação.
    3.3 Normalização dos dados: Aplicação de StandardScaler para padronizar as variáveis.
    3.4 Criação de categorias: Segmentação dos municípios em categorias de baixo, médio e alto número de óbitos.

4. Modelos Utilizados:

    4.1 Random Forest
    Otimização de hiperparâmetros com GridSearchCV.
    Identificação das variáveis mais importantes para a classificação.

    4.2 Naive Bayes
    Simplicidade e eficiência em cenários com grandes conjuntos de dados categóricos.

5. Visualizações e Resultados:

O projeto inclui as seguintes visualizações:

    5.1 Matriz de confusão: Avaliação do desempenho dos modelos.
    Importância das variáveis: Identificação dos capítulos da CID-10 mais relevantes para a classificação.

    5.2 Resultados Obtidos:

    Métricas: Relatórios de classificação com precisão, recall e F1-score.
    Validação cruzada: Desempenho médio e desvio padrão para os modelos.

6. Como Executar:

    6.1 Clone este repositório:
    git clone https://github.com/MMoreira020/Classifica-o_Datasus.git

    6.2 Instale os pacotes necessários:
    pip install -r requirements.txt

    6.3 Execute o script principal:
    python main.py




